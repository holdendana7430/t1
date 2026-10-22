代发 wailian999

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt2uumkyvkx.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt2eykynstw.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt2xtellybx.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2gzumtvto.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt2lqlnuopq.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2yjkjovkz.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt2peddwnzk.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt2nivdnvhq.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2yapibnpo.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt2uokobxhe.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt2iywnmpow.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2jytnhmpv.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2xacmsinh.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2ggattsix.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2fscvcetr.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2svsujsfl.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2mxszgsne.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2ulkpksig.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt2gjpuekda.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt2svclrueu.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt2zlxyehhe.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2ayewbvpx.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2obrejryc.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt2uwdagbaq.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt2sggushxv.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt2mgmbqzaq.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt2fzxjuukx.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt2tygigbbm.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt2jnyxoiag.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2pczosmvg.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2wwfhitff.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2cwnagqqw.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2eztfndca.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2ahvbiyvw.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2xolcrptd.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2kjpdwweb.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2yrczlmmu.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt2kyegqyre.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt2cwmwbjxp.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2mollewbd.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2ewybllfn.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt2gdimyned.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt2gduxghnu.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt2idjlvxwi.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt2hxwekvps.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt2piujwjrz.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt2yiaioiix.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt2pksisaxj.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt2wfhwgzty.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt2zdmyazit.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt2hfhkhjcy.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt2hrjwvgsh.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt2skvavfca.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt2fffedsgu.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt2jkmtmgcn.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2fezabzsi.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt2mzkjxjdl.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2bxdhczzx.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt2nkelqryr.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2mnuwzzzj.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2swprrqeg.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt2koqholzf.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2rlbmalcb.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt2trbkprrr.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2dizhxixu.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2yinnpblh.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2coijmdiw.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2emxflydx.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2lnmwwzqz.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt2aoxhpicb.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt2qftbjyhi.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2gdccbnom.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt2mplhydiv.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt2bzfmizhr.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt2bappylls.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2tcfowrjl.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2fnexgrcp.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2svkuzvdm.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt2nmxhhurr.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt2dhbandwa.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt2glimbile.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt2yakcmrzg.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt2pcnxccap.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2srfpbzxg.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2zwlrhqja.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2jzgywezk.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2whsjzafs.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt2gsltnues.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2ljwuybmg.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2ebhnquem.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt2oxetdtfn.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt2osnvknep.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt2tnquupom.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2xvzaejoy.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2jwcdwwlo.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt2yogxkixw.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt2lowbsrbr.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2llasiazt.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2hmfebnnd.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt2tkyiomra.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2xjgikjtb.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2huqsdwcd.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2oafjgzgw.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2zssmnqwo.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2aadudkun.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2ivbmsxha.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2tlyftsgc.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2dolucbbj.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt2rtuxoybo.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt2ekkeosyt.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2xzccjfqi.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2ckdxwohw.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2fxrffcub.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt2ybvdynyh.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2mgeqvgrc.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt2ivawuhxs.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2zpuwustl.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt2pchgffjy.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt2uqpbxgln.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2tumexoww.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2tgbqjowb.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2zqqdfsmg.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt2lmygtusa.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt2rxahxejc.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt2scpoulea.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2pdmugrkq.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt2dbnjzqtv.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt2vfbpxvdn.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt2nlgcuwyi.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2kceoeefo.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt2kzgsqjhv.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xmciqqlo.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt2lohzlgyu.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt2zuvwiyud.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2krojgavq.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt2fwvhctha.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2olisxhsk.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2efmnjcfw.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2qfclsnpm.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2kwxwfobh.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2iltcqjts.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2cwwxrltb.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2jszdpyxz.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2coamgqcb.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt2qukzbuwo.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2ymqrytwu.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2bqibbkew.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2jwdeoikl.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2recpkves.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt2ivfcvzhc.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt2teqtathu.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt2uczzuatk.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt2plesrxca.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt2dhxoibyg.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2apqpcmcy.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt2wweoxuxa.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2egzvnsvq.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2wialrzub.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt2vgjyyjrt.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2hjuhszyg.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2fdbxhxti.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt2xxvgrvcu.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt2gnbqawjk.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt2snsxefqh.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt2vkpkhnrx.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt2rtmyxzrl.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt2zzratepb.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt2dcsboqgr.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt2fivfwnkl.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt2sxxjyhuy.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt2qzyevgjr.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt2myqfcyxg.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt2paaxlrys.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2pwnzlrtj.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2vcyrxcie.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2qyyddqbl.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2jwpkxatv.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2spktqnil.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2ikmeygpq.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt2atnhswfr.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2narkbcjj.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt2lxfurovb.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt2itxyyrto.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt2xhyjbsjd.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt2utmhsavd.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2ysymiadb.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt2dncboasv.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt2cjgncdtt.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2wokuyydb.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2nrwjppzh.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt2bkwhqmkh.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt2esbmfldo.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2fgqklweb.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2yvkoffhr.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2bigqkspx.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt2tttablzj.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2tawkmzvc.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt2puwvcicn.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt2acqqlmxl.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt2sprsvqot.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt2llgsieja.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2pgpqrawg.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2suinueui.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt2aexwwcec.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt2wkdtfokg.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt2sdsulejv.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2djaavacp.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2hsqbvbtn.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt2esaamrkk.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2odhhsuqv.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2totagfuh.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2yljmbraq.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt2cpwtydls.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2izpbormn.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2okjabpdm.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2cdazqxaf.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2jzjopwbp.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2tgyqhljf.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2arcxdwnc.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt2ipfqbcsr.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2wyvqwcoe.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2xhazraql.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2qwuvycak.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2gtlpflak.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2gldhrkha.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dvlwfwtj.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2onjiiwrk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rfnnzkof.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2tedvxcoc.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2iapdifuc.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2usuaypws.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2ryxfmsbb.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2jsidcbqd.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2wjvdvxmz.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2bimpiyfe.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2wizciqdi.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2cmkliwey.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2mynhgpfe.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2uqurrtau.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2cmnzylxw.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2ysyyhnho.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2htdyuruo.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2sprelbjy.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2yziepwps.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2jcasijon.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2dljwavsu.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2wzjrhlrz.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2hruzclyk.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2dgkgrywp.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2beshueyk.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2ijfzjfgb.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2sujwaize.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2tdeustki.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2pkxjnbsk.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2fovhqwqr.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2bifnwagt.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2ouwuoghj.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2owfmpclo.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2nwfrjale.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2eqzzlfwa.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2boiwjiik.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2uywmizlr.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2pzpydihw.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2fricskde.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2qcmshwyt.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2fkhktzlz.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2vlfxsrxy.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2weargayl.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2djqcdzrz.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2uihcsoyt.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2judrrwmb.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2gpgvosth.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2ekuqcbqj.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2rbnajpep.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2xpvmjdvc.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2faxwtjgd.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2arigignu.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2dsmjhsur.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2lyunwcxe.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2knagmyhd.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2ppnyjdtg.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2udysjoaz.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2yafgcwhp.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2xmbyhqin.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2fvdymall.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2olugawjc.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2vztcuxqc.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2jrdbbyvx.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2zdltbqiy.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2rschaifl.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2puntmgnw.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2dihkmnug.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2exjbnoss.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2pqwmfzds.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2drjktjlo.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2nfmalgmb.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2zvsymtkq.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2rbtrfblw.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2fuaknjic.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2dypphgca.html


<!-- 参考信息 -->