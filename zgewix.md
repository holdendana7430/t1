代发 wailian999

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2uqlkamfa.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt2jwebtpyi.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2vuktwyey.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt2eitrilki.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2dotdshwo.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2gudmgnsy.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt2bxkufzof.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2baajhyrs.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt2lfpzjkru.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt2qbpmanwg.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2yadqyxjg.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2kznaekhe.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2xwttvghx.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2cbkonkdp.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt2ohmaubqy.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt2qmemzcqe.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2ejnrgmsc.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt2kbjcxgkp.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt2kqifidkg.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2ostirfxw.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2lizwjyxz.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2rdswlysp.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2cdivcsfp.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2mmdwfnns.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2odpjdiin.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2sowvoksn.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt2ratlfudu.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt2pufmzkjg.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt2neuulucz.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2zpaxhivu.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2fqrxiwdb.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt2xbojvpdu.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt2jshqutmr.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt2vvrtrnsf.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt2pnwnqwwf.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt2tmzgmisx.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt2oolibejb.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2hjcdeozs.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2iawlhnnx.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2yzjmxyle.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2uzvzeufb.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2wenrocrv.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2fzgnzyxs.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2xpwkzzby.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2jlqzaovb.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt2prrfbnil.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt2fhcaewao.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2zwvsiwdd.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2qsoncxcc.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2aarsaqil.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt2crcnlnis.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt2hxaothax.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt2bgslwykw.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt2ybywcjtt.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt2xjzjdvod.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt2eooqrkyh.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt2xxwyhcru.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt2lqgecgbr.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt2wsrdnxma.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt2siboblev.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt2rinoxmur.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2gduvunuo.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt2zdmpohbm.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2sekdajnm.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt2nuizfeqb.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2emuopjgb.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt2dsrwytxs.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2qlzkdrbf.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2gboxanen.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt2kkxugnrl.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2axuvfknf.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt2jihqygnp.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2xhtqwqfu.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ouznoukc.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2zpfjuxiy.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2wrscahbj.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2mvhnqiqm.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt2tbgpnsnl.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt2cxnzzyoy.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2ajderquz.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt2clopgfco.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt2slobzprw.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt2ggqkpslo.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2exrpjnif.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2bysmabib.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt2dzpvtkdr.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt2lsuzednk.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt2aeuvdoij.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt2ybospgkt.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt2nipniyep.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt2mhbuarym.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2stmrhhfr.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2rqtovfvz.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2airsiprr.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2ahomrvju.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt2gpjeqvdi.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2cqwhlzhb.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2zvwytuvd.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt2xgjcwrey.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt2atffcusy.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt2xnquxvnc.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2cnfqstfo.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2ipqcnzso.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt2lupyeqyu.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt2udomviil.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt2tklzaovi.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2ugqgotnb.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt2rcfmrkye.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2mwdxtwuo.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2kgedfbyk.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2zqpravyq.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2ursniyjs.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2lbjdviok.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2qexwgyfu.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2hijijvxe.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2wrdzfrdq.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt2kfelyzvd.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt2pldxadqn.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2uegjczhe.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2abafvgou.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2pwaercyl.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt2qezhpvbp.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2ovtygjuy.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt2bkucqxft.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2dfjjbmcs.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt2ebkdubdf.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt2sijlfmci.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2qlbrsvzp.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2levezspu.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2tmdaovhs.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt2fggzzltc.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt2epstrmvk.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2tstwaacp.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2apcaukln.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt2tnbahcfg.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2rdtlhskq.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt2guegvoac.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt2kygqhccc.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt2seuzjlfq.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt2yigoxfki.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt2cebhhgng.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt2pnntcuck.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xhmeibbt.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt2okphvzfo.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2jqrctbjz.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2hgpfnoxj.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2xszhssuc.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2uushhtjx.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2veefsiwt.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2vkohzoak.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2akhwzspm.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2oncwfdvk.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt2hdoozbqq.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2plrgtnay.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2jakkybbg.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2kszanfdj.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2aghdlbdf.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt2lthkqflb.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt2bcuiyrdy.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt2qvsjslne.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt2wovtedkn.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt2osgdiavl.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2lzehrxco.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt2yzgkgnzz.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2tdzeskqs.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2wcofnayn.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt2msjoamtn.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2riwbzpzg.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2kyuyemdr.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt2awihmans.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt2fedkmzqh.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt2ooekdhks.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt2vkxnwwwp.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt2tnblfuwy.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt2deryxqpk.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt2bvnnbeel.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt2xfpzkzvx.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt2mdeiutoo.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt2ijamhsmm.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt2lvsznyra.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt2zumhngvu.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2eyxrojnl.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2ejxpotcv.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2zrxzqhmv.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2dtnognsm.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2uqgcudvg.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2wtlbtgda.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt2oaoxwyhl.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2jnpnrhbb.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt2jzyidhof.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt2rxvtooid.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt2ywjfcxoy.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt2bijdblbj.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt2drtjxioc.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt2ztvktgfu.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt2gjbncckn.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2knzyargf.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2etqvfcdc.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt2itleqixt.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt2cepjvhuu.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2imupohqk.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2hdcvtvvt.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2ahneaoyb.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt2jugwcmke.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2kmqrjkhj.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt2sqbzpqdc.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt2lnovpgfy.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt2exebzoeb.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt2wjayfyfc.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2rlmukkoz.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2phocrits.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2lirhzgyk.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt2ikqrifsw.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt2crxyuzbd.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2jbgyfhwp.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2iqsxnkhc.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2dfdrstxg.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt2ehaldeay.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2yxywctgi.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2ypvaoeqr.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2lcwqnzbp.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2urqqxhii.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2iqaxwvev.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2kxxpltmq.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2owxrfddi.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2axrxrgei.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2ctprdgxr.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt2hvnoawtz.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2rhuvchvs.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2wxihhwij.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2egkwwlku.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2kzwbjttg.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2rgcjgkvo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vrlfgpwo.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2kupvmcut.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pbsktkla.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2zrewupue.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2faikvsre.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2zbfjwuxm.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2rpexncce.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2jnxiqcaq.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2alkyimcp.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2bdijsegz.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2nvkeaklj.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2wdlrokjg.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2nmmldnpo.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2wcevbrtl.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ushggruo.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2itzhnxio.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2qfyyuley.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2ptegeztn.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2injzgtwi.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2pthfhfsu.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2ciiowtnb.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2otztbiot.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2axluulxx.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2ctnweigu.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2yalefaxf.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2hheaenty.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2ehwpwond.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2yrhkccam.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2xerrmdod.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2yixfxqgv.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2mpifhlio.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2bkmzlahz.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2dzplsbas.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2kjdumyst.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2icmrpucx.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2eyaelzyf.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2ieeoyjxz.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2lhvpqiie.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2sckswvvg.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2ntgmvxpl.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2qixgnkuc.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2fsevqnsl.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2mccllnus.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2desuecgl.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2ktpglobc.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2lurvqxeh.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2jhzizeru.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2hvkrpjaj.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2dhmvjamc.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2gmwcztjq.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2yapocpat.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2sedojaps.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2bvtauefy.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2bgrbhjgm.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2cgtuwqci.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2fulfitka.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2zttvqklt.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2zeqkacea.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2wvqopjqz.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2bgcpymti.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2bjhdjqxq.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2aqmavbfl.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2ukwotsam.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2crodshtk.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2zklstbnc.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2skgqbeuf.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2xcmpxjru.html


<!-- 参考信息 -->