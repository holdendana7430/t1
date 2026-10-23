代发 wailian999

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3iqnverqc.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt3pguudksf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kmzsswbh.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt3jydcrjpt.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3chvxmwsk.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt3aydmczzq.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3gsfblyvd.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt3gnskhumk.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3qobvvjkx.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3nfiooarb.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt3ulsjgmqy.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3dfbzthqk.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt3wllyodvb.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt3qmmyasxn.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3zilcgimt.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt3yutvdjzh.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt3mringkbw.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3yxcaoktu.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt3jskzswaq.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt3uivdscxg.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3uerqczkm.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt3txzchmjs.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt3sysgywgs.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3fyvoltxb.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3xvtxaefk.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3enanjzxd.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3fjfnlanz.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3gmeslxwm.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3vyogcoyz.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3kehndbca.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt3unszpqny.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt3yleabnmt.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt3zundwshe.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3ddocmofp.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3fcrhcpcb.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt3tlrcqjrb.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt3bruhooms.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt3dxixnxbr.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt3fenutfcq.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt3vxhusckb.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt3iwoatcfe.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3xzmbtyas.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3wokiljty.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3cdsggxbq.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3amrpynnb.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3yigdqrab.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3fayvxfwp.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3kytjfoec.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3daegnqhd.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt3onfplyai.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt3ognipbty.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3rvllohrn.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3btochzzs.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt3wbuuusih.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt3uvesmdif.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt3syutjjpk.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt3gzibuidh.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt3utrskmsl.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt3lypqemsq.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt3wxepnowm.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt3lafitpko.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt3itgfhlcy.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt3ezjpsnbf.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt3ywxlcytj.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt3mvvyezob.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3gqqmjdzu.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt3ylguqyci.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3imydxkha.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt3qhivlhmb.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3wjdeyxqf.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt3lnppfeyy.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3yxxoowqs.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3enaqgjpm.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt3ympixiso.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3xplqhdot.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3ftonkwxh.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3corckrbo.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3dgtnmcbj.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3togfvgmj.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3nbfhxkxe.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ujmmadxx.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt3nworxfae.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt3uyqnksdw.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3frpyetxe.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt3wvuqwupn.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt3jmiuqpvg.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt3rxppcdpw.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3uxknvata.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3ezekyrsy.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt3gegslgzx.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt3yylokbwn.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt3lgjbyuca.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt3vlabhgrx.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt3gpcozaxd.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt3tbbajapt.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3tbohdwpw.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3bvswnqdc.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3dwxpthva.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3uzcfazwc.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt3ijsqnkhq.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3tltyjlhm.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3tprxtmpv.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt3iyhhrqjy.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt3yzcjhust.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt3vhoduonq.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3youiqifz.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3vkxctaob.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt3kvaqkdmn.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt3stqhyzlx.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt3mrpxcsjl.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt3unpwhjnd.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt3iorkntxz.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3aiohwtar.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3ppzwdkbm.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3ybdilpsv.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3ksrdaaob.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3wxyjfpyu.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3laihcnsi.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3qxfryozg.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3ocbuolkz.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt3gdmsmudu.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt3bwpldoon.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3hfrfsdam.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3xfepxgif.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3ziymanpu.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt3jlthcidf.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3bvnejtdq.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt3qqcmvtoa.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3xyakvszh.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt3mugguqwe.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt3tjguudon.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3xfiregux.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3gjrtmjgo.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3xnavbmyd.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt3yulikgsc.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt3zcyvdsik.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3kyuvbxva.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3fjcuebjo.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt3smgsmsjq.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt3dfwabaiq.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt3jbebpvbt.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3xwrzmfzn.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt3zlowwxbn.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt3okawppas.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt3deewndcx.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt3dtubzlfl.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt3rvukpwpr.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt3hkajquwz.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3xajgaoul.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt3nwrqpfok.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3zvsznxzo.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3copwzwfr.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3feobjefx.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3almraydt.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3troeoqca.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3uimtpgli.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt3kkafsqpa.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3ufcapgeh.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3euzbsewt.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3vwiknavm.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3dnuwbtlc.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt3tbqctedz.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt3suwqrmiq.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt3yrqdtytf.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt3wkgexqrd.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt3ofmxfxmo.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3qokbecst.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt3bomnxbox.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3uffotghp.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3syfbmwed.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt3nqibxaai.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3hyjyonnr.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3jzsrjyum.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt3gpetpplv.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt3ffqasols.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt3gwkndhry.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt3clpxfsem.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt3alrqwemc.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt3wfhmrgvt.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt3bxkegshb.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt3tgfxkffe.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt3qfptuxnx.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt3ehjsetma.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt3izfshogv.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt3aeyyvgwp.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3fouzxcue.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3lnvuzjsg.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3bwbzrdlw.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3bbvhdzmq.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3nzwygxdz.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3wzgqmjrt.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt3aokylwed.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt3azbpxeqs.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt3nkglhmki.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt3evigktka.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt3btlxkcpb.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt3ozesnxqk.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3hvetubsa.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3nkmsmsef.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt3itmgnyca.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3ssonavut.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3lrufzank.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt3ezswqphy.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt3ygandviq.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3lcftydmf.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3ytdreyew.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3dwrvkcqc.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt3cpwgemnr.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3kfdtubjd.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt3qnrayasx.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt3cnrevkgn.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt3frfqyqwn.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt3uajpxkvg.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3zgvzzcvm.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3hbhanwek.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt3cuihgaov.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ekakftpo.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt3yxkzdhlb.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3vabageix.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3fqhpkmzb.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt3eianjucg.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3bksmhilg.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3gmmpudwi.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3keitfppt.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt3deynsxpa.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3ebqhawda.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt3qgnxjgic.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3vkjqkbsd.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3hlcpzhbr.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt3mttcyrbu.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3suxjpaox.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3obcoxiec.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt3mewkkvyp.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3knfskahc.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt3uqxgqspt.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3jkuenxzu.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3tyrzkics.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fyizbxby.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3mufiyqee.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cpvjihwh.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3lkzlbdtm.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3xuhrtkar.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3tkgboetp.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3fpzkztzu.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3elkcboed.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3jwibdrpk.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt3mbslutwb.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3fofbvdnu.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3leyguygm.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3ptrdxoag.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3ulgjifpt.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt3fokieddg.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3zvrnmkak.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3exedlkfw.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3cnpsdmsh.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3angbjrxk.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3pexsebro.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3nawenrkx.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3azgvmmwz.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3ddcvquly.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3lekexqrp.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3kpuedcbg.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3wnwxynzi.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3kywxbvsx.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3ihyeeqfi.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3hogucxuc.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3qlyrdwui.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3guurdaoc.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3wtdazqix.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3zvlalesk.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3dtcgyvez.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3zhjgbqxn.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3hjhshied.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3mtwghidn.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3lrbyowco.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3uvataztq.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3ofsokafa.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3pxbrrcmu.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3bdaiwinr.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3ppcnuncm.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3ucjvebtf.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3zhujzhpo.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3pdlxmzfa.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3gcerlvam.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3rtczgkav.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3womggwlz.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3kijxawuq.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3ojvefkiq.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3zwrxjfmt.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3emarrtpa.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3vrzqxytq.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3xoctrwdp.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3dadasogh.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3mcosibxi.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3winaadsw.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3lwrqpfzu.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3mqcbwjkw.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3sblrlphg.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3eyjofsni.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3uhbjombg.html


<!-- 参考信息 -->