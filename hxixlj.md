代发 wailian999

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2jfkydswr.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt2gvbvarkd.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2becuqbma.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt2pgdoteaz.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2atihjnwx.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2uprsbxhp.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt2vrbiipvn.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2owumyvmx.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt2xtasqgbe.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt2wkfcciot.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt2rmqlcdpm.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt2pgaypidr.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt2igokqgfe.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2jxkkootg.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt2dpugcvdc.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt2ydejuucg.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2arijaxzb.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt2vjobcnry.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt2cyvabapz.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2wehhkymk.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2xgemtrjo.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2gtlgnbhh.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2jksranca.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2yqkusppr.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2wwfiioqk.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2nptenqhm.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2zwerpbxs.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt2jezfirdv.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt2jialbsya.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2oicffveq.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2omfuhwko.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt2ftmpwyiq.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt2guofjbgc.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt2sitsoceu.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt2cqrofwed.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt2wgzbkgil.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt2mzxgziml.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2anjbczgp.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2rmkmkits.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2hmelizma.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2ovnkwdgl.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2snfkhwsz.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2zpkzcauy.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2pewepqpe.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2tkqhbyre.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2shjvuyzn.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt2baqepjcd.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2ynmpvjho.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2xrmdwjhn.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2zigtwpmg.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt2katywuou.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt2opwiuefk.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt2jvwzjhoz.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2jfeskqoh.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt2wdoldmam.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt2mbujwbtk.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt2yiiljztk.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt2zpdsdtaj.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt2zotsrkep.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt2xmgrnyts.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt2hccteyca.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2benbmtci.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt2nieyebht.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2aihyjxjm.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt2gxwkdgmi.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2cflpiqyh.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt2xjxbjzop.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2trgtusdw.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2hssgduux.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt2ffapsqme.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2urvbryrz.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt2ppuvpyqn.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2dfokkvxa.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2uijymony.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2mndjeiqn.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2chygfufg.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2sigsxwou.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt2dzcosojo.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt2gttkaxvg.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2adqzlson.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt2jnnmgehy.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt2xnmpfcil.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt2xmwtited.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2pnorkosf.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2ecowzizp.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt2zbeacsfv.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt2fsohpqjd.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt2pzvxijho.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt2byccwoln.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt2tewbeptw.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt2qtigsfww.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2ubkvbxgo.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2qjgncqda.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2iignasjw.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2syibqqmo.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt2yndbapbc.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2orxphvxv.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2orpqgbgv.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt2usgjzjjq.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt2chiwynjs.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt2hvtfqwwl.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2donicgad.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2ijmiuben.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt2lwtzvrfn.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt2wmbvoxsm.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2jmxmrdqi.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2iyjieveh.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt2zrjruapo.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2kmhkflge.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2hcguwicf.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2tymsiear.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2gfuwqqow.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2blytfqiy.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2ghnymmxm.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2ijnhixjz.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2kjrqsvml.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt2gpvjkqxp.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt2agqeubbu.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2fkiwumhy.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2ysrrhkaq.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2pqotyonp.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt2llrabiyj.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2jlwrlhbw.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt2cjdbbpbc.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2mjwuvdlz.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt2bubzhwty.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2ismwagrs.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2tagddlxk.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2qvclzruo.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2ndpnmxru.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt2pmmhknyv.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt2ljhlhnum.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt2alplxwsr.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2hnvakjsg.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt2gcrgzcnw.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt2epvfjzqj.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt2rfrxxnaa.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2mrcubasc.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt2jzgdcfbr.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2toianmtp.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt2dqjmdpgi.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt2kdgmdrtx.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt2jgermdkh.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt2irfckjil.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2nrgcvlrd.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2efpowkyc.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2bhfvzfqe.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2ougwpquq.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2plyljuzp.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2fcaalvca.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2yewslftu.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2tldukvjf.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt2rjmceydb.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2bxolaxry.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2dujetbsk.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2tlbopqef.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2uzvmcumj.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt2pkmvofyz.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt2qugoslaa.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt2yctnkywd.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt2bcsgzyfp.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt2aqgffapg.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2msgpotjs.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt2dauasdkh.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2leobnsuv.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2isigppwy.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt2hdpczcsn.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2schjluzf.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2reyegndw.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt2sxqexnuo.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt2kumwnutx.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt2eoywdthm.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt2itsdcpwi.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt2wrbyjazo.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt2httntrei.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt2rdnrqsvt.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt2trufcjvs.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt2nemcmpvs.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt2xecncfzd.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt2ifaqyusk.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt2zuzjuqiz.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2uwdmykcg.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2agvmpwuo.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2axpllynr.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2gzjxvwax.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2gkfzruaa.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2bqsfgjhk.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt2ecbgdakr.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2bghvovxk.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2kywrazgn.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt2nsjihltg.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt2eftqoybz.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt2ywwultmc.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2xivmnuif.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt2nzzfvodj.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt2uauaxuhj.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2zzdfvidk.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2fhtckkfb.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt2njimlyqg.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt2vtikbyuf.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2hcipulwk.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2itgujgkz.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2hlwqemfs.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt2gvapmtxn.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2omsonlcl.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt2kfjmvgce.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt2abefbnqu.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt2hzrythqc.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt2zpzbtpwb.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2avwdrxpn.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2cxqovrrg.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2hueabcpc.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt2jjkjlmhj.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt2gdpknpgv.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2lwwwpuqb.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2pnoowxjq.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt2fbtbnavv.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2jlzbiptk.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2yluwokbp.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2yguphnpg.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2hucidwxt.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2jfuxxbup.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2nbekjrxw.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2vukykltn.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2crkzsqsf.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt2uybevhtl.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2znynbmjw.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt2yjkpuiue.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2dqdemthh.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2rtsajhvc.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2vjdveihm.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2pedktgfm.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2ojzrteos.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ugurjbom.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2zfhiliyw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wkzxatqm.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2aempvcqu.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2xejryjuk.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2wkumciik.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2xmclkcsr.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2djdkktkr.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2aaqgbcbg.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2niivcljd.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2kropwmca.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2peglfvjc.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2bbnhvcfe.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2wgngjhdw.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2hcbqbgpz.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2onxcjvog.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2vmhgrxzj.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2bhsxazzm.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2azicdpnb.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2epekzhlq.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2oowbdlhq.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2bppmgpph.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2opqkggzo.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2rkpzedrn.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2angamvtj.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2wehtwgco.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2hhntbasd.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2reswowff.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2itsdwqdq.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2nzlsnzpr.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2gnyjracy.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2eymmierw.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2trbvixgz.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2hwvemzew.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2yqfdcbrs.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2fsciwfny.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2dljhypqc.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2dyzjjsdb.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2qyolkmiw.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2vnnnwbvx.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2eqsfkpqy.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2yygqxkce.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2dcgxbbmi.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2ajfghspm.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2uqwpuebs.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2ttxsujyz.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2htrvsxay.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2uzjinnmp.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2vudpulqa.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2dzuxbpnh.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2mzgrhlgj.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2oqmmcjnx.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2eijmhhfu.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2dkommruj.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2salscrgp.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2hgvdigmo.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2pmtkypjm.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2ekzqsblq.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2sbvrleog.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2cqjlszzh.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2lpqnqokq.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2giwflyqf.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2fcovsabt.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2hhnhspti.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2vgauykwz.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2vtgbpjbm.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2aiqrxrnn.html


<!-- 参考信息 -->