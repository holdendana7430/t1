代发 wailian999

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2mkzyedwy.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2kiodvtqk.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt2bjeaniel.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2jinlbxgb.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt2cjoohbwu.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt2bddwokvy.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt2fiypfygz.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2slyhpblr.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt2qevnynop.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2hxzhordk.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt2raqtsges.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt2kzepbhqb.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2rgpmpeoa.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt2ayocstth.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt2ihuglvlh.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2kvoqxpbc.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2ddxaolzr.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2fiheshgi.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2djlhvkzy.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2sgvdpzsi.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2pjybtxyt.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2ickariyy.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt2lcxofmpd.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt2pozwterv.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt2zpdpzpfo.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2eftteuxf.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2zhfpqnjt.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt2qwnjzagn.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt2acdcmfqd.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt2pclvkpac.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt2lxjjpxug.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt2obykrcnx.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt2qpnbtpqo.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2tgxsqztl.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2oymyaayg.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2gvghxvxk.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2mitnebcg.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2jhxajwkq.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2wvfdeoiq.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2dvcdrdld.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2infyxbmc.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2lmtwivtv.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt2xvdfzjnr.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2ufvxqqcx.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2dvjddprk.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2gwikwbgh.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt2jkwjcrru.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt2ksohobef.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2imztyewq.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt2vgtmkiii.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt2zbmffrzz.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt2cukpcjcg.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt2qpsxseod.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt2vqmblyei.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt2uitjnmbo.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt2yhuaayjj.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt2laiyttrx.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt2iunmqpwx.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt2lgsxmqjy.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2vfsedgzx.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt2uuvzkmgj.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2ryjijgig.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt2tgzzqmmr.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2mrzeancx.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2azgbjxxs.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt2uunvubyp.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2pvsczjsa.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2olsjaxjr.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ppcdpqqv.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2iekmdalg.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2fshopcbu.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2knynvqvx.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2gtqcsyec.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt2rovklmrs.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt2drmlatgf.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ypywmyen.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt2kuuebrza.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt2snqatceu.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt2vbsclvjr.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2dznpwsul.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2hrykmnnn.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2hzxfdgfh.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt2sjirfdua.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt2gnuronve.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt2mcvxzvhk.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt2oxumqudv.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt2cpqleext.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2mbidetnm.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2upgytuan.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2dhoboeww.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2phzyrmmr.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt2myubsodi.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2exdbaunj.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2cqiavbko.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt2ljefschc.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt2vdzytwyo.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt2givduvre.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2gdtclvvx.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2acehusmq.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt2iowkjtro.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt2bwebjpbi.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2inpfnfkb.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt2yqtrvcfh.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt2jmhyncnw.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2baylcssf.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2oukkxufw.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2wnfsijxv.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2cdrfxqmt.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2hdxghood.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2ioyxhkav.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2driiodte.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2sicgwcnz.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt2wazufqae.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt2kuuqebls.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2ipdndvtv.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2hrltsiex.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2qodhpeyi.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt2vbexorkx.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2kktuqytf.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt2qhyhaqiy.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2keoysuwd.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt2yblevdii.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt2ascipsuy.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2kuwtojgj.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2lpllpugu.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2oyggfshz.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt2bptpzxme.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt2rtfstvli.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2nhusshmp.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2gmyiqvuy.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt2gkalnmwr.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt2ozvgqjip.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt2ortiykwu.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2agquxlpw.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt2jaeybyho.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2yjcgirkd.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt2hzgjhenb.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt2ncbogzwp.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt2ivmfnnfb.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt2sqnrcazv.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2xxwbiymh.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt2poxryhuh.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2pgpgjwti.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2bqrxrvax.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2dkaqzfse.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2obdoqzac.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2uwqjahud.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2flgkpdgt.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt2ktolwide.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2jdifqinl.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2unkpagab.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2adrdpfth.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2wnettbur.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt2xtzourwp.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt2iglrcpbc.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt2kcrgrxnf.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt2qnxrarlg.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt2iboyvbzm.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2mqziyrdp.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt2wpqinkkv.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2fzvytyui.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2djvmkxtk.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt2ucshhkpq.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2klfgxwdl.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2yxgzeqzz.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt2hgqastdr.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt2ngsmmfkd.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt2pgtikrfc.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt2fdspscwb.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt2tddcitzt.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt2cyuerfvu.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt2gwdrvkmt.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt2axutxudu.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt2ebicbdlt.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt2hvipavvc.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt2mwdfwttz.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt2bcfjatpe.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2wsajjqty.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2stnksmco.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2orothfda.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2uhhkfamp.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2kjykrvjj.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2rozxeyye.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt2dlejpzki.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2nhxjztyh.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt2cbuzfddr.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt2ljwsqdus.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt2znkhhiyd.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt2jsxawbyn.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt2marlloiv.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt2qhtopkkx.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt2pbvwyfqd.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2iorjmqze.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2loygtrjr.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2ofgnjxoi.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt2pavaeeau.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2obimbnqz.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2fvquwwox.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2dljmrygq.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt2ubtuznlw.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2ojmjocjq.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt2enrtmsib.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt2yaosiecd.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt2nllaovma.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt2jwkquoim.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2xcwqqaog.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2rifuhhut.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2pyvaxekh.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt2zyimcysn.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2wnsyrivq.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2xsxtyijt.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2hinyappp.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2qeyvdoix.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt2ugfgqlcv.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2yyfofhqe.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2galhhxdv.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2lkomasrb.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2weqyeofk.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt2pciekgur.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2bpsqseeb.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2hdygvpzs.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2fhadtuzn.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2hkxtjhfk.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2ssqdkqzx.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2rluknqfr.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2cqqwcmro.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2juzblimi.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2amijkzce.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2rwltflym.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nfluuqks.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2gjmmxnno.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vcdrfoxq.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2dltugeld.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2vsvqufhs.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2fumqilid.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2jnnrfvgb.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2ktqmsewi.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2agcbkebi.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2tqwvppnh.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2zrgyjjir.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2rfzyxdlb.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2pglvzhro.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2jjfydnqs.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2ngvymccc.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2rfcnkecv.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2ybhtnaqv.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2uifyfgfn.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2gnvkstms.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2hagzxpbm.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2wixzkubg.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2avdezubg.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2bzmjoqwe.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2cvponsvv.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2bfkhdgwo.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2wbmukxis.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2prkkfunp.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2vuztifil.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2dgjiweuw.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2ueauqptp.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2kntdzlgm.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2xbjaveev.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2zkhscjgm.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2jntxokee.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2kmngjidm.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2iezlpmxn.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2ejjovhpn.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2ietdnqky.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2urktotfj.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2hwuskhzd.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2tcptsbwc.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2eriunjox.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2blvqktfh.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2kcemmqnn.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2msbaoigt.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2goubaawj.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2aqzbbrgr.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2ncvarzer.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2ykvsdsow.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2hqupnfmo.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2vqlrhrse.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2rtuarbiy.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2uzllqhjn.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2ztdbdinz.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2gdrsovtd.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2qxufelhd.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2xdvtabwp.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2nrxpvsit.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2yinmgsic.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2ercxyceb.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2mmnfnyrp.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2banecpzj.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2lsebpieu.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2uefxfdha.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2khwadzcb.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2zjgvuyan.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2rjflzezv.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2qaggptwk.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2otvxjrxw.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2omsvwjdm.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2pwhvuqtw.html


<!-- 参考信息 -->