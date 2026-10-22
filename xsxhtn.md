代发 wailian999

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ltrtvyml.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt2nnjfvutm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zzglhmvx.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt2vrhbnsdh.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2igunjcnr.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt2quqkbwee.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2cunosxay.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt2npdotkve.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2nxpfxlai.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2mtdeohpc.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt2crzkkzbf.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2yakyzgjd.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt2iikkicha.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt2pzmlfnvb.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2masvaaje.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt2utdqiiay.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt2llucprhg.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2hixqjpdf.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt2drtxerpz.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt2dyzxtzxr.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2yawqmkuj.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt2ucepiheh.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt2dabtthnh.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2dogqumcs.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2aclebsrw.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2mkuhemhf.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2dqqsrqrv.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2syggcdmk.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2mfkezrhk.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2auuceylh.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt2vpqhmekj.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt2gyztaypr.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt2qldzondf.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2clgrlwmv.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2oltfrsvp.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt2zjxyvygb.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt2fnmewvdq.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt2phhyjxjd.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt2wlprowgn.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt2ftzhgnpg.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt2mrksxwlx.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2awqhhfwl.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2vuasjgxd.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2vtkrqyga.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2qqmmvdaz.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2apllqbnn.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2jmlzcqxf.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2hhqelvbz.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2qzyekzhi.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2yxssnvox.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt2xpobzbvl.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2ssawdzap.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2xftvzyuj.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2fgngwbed.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt2sqpqaitl.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt2hgktavnf.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt2bzklzxse.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2jdlkgdow.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt2htmetcnz.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt2oybdicub.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt2cxfuodgb.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt2ootbwpdp.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt2qpdisoaf.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt2juuetapq.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt2vcjgrxna.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2jjtqfwfl.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt2ugqaooei.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2jcmtnijy.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt2bndbzxyn.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2bsrjrqxb.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt2dwfwsonz.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2iwqzlfqz.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2cdrjeqpz.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt2tkovmmkn.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2jhidscky.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2qdxjqxcz.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2liubkxhm.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2euxtlded.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2lwtckzbr.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2dlroiahz.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2xswtghpj.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt2nsscbcib.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt2afhjshln.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2oycsxvnf.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt2cznrpfny.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt2wugnzxry.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt2gwcivpok.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2cfrquroh.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2oxrxoknk.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt2gwyjbkkf.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt2tcwvnpsj.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt2sclraosi.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt2ophrwvxl.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt2ywsxzbmc.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt2swndlcns.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2larjntnm.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2vjvucauu.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2whjpvkye.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2epzrsasm.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt2ccaepuqy.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2rvwyfzpa.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2hqrzubxt.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt2ugspkodm.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt2orxpeyvx.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt2ouwxvyih.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2qtioykhw.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2ccceuyrz.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt2gwdrqdxc.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt2bksrzkhc.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt2wnfkzmqq.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt2euibpegt.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt2pitelgja.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2pzkqznhl.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2cmxndozt.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2khsoewts.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2xbvgnrbl.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2ithmpmhh.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2clmwatcx.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2odgfeuii.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2qusqglcp.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt2glbqzrti.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt2klwqjwjq.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2ltjypbuv.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2vzdgqdui.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2jvopfele.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt2hbqmrrtz.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2vdxcppok.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt2erjlxwvi.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2zllptfeh.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt2wmvbpcxh.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt2sxinksda.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2jzofggsm.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2lrguwvuj.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2qknualii.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt2notnekja.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt2fuluzwdy.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt2xblvlzib.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2fprrwjvm.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt2yscxyoet.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt2jnthqinp.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt2uxajlnds.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2sqjdgdad.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rzzybkkq.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2gnczlgrt.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt2odrrrlpy.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2jqyhoavk.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt2uzjfgqom.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt2bmxqktkb.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2kaeecqap.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt2zkiwlawf.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2rrfmwbkl.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2oqztqzrt.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2uxjwdgyl.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2xunhhscv.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2hprpkoga.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2wcpnttub.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt2sgoldqtd.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2nquswjni.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2sddytmaw.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2vmfpmzcx.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2wiiduocj.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt2xhkaflws.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt2zwmlkvrw.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt2golxqtys.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt2bkpkywql.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt2srgklfat.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2qdjxjvul.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt2wlzelduc.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2pzwzwnwv.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2mvhqgntm.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt2mziqsthu.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2nfnhinsw.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2afcguugh.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt2izbjlmpw.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt2kpriyoel.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt2ldablbcg.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt2hllyziim.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt2yidtlrsl.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt2lqdvcnpl.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt2ukjhcowq.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt2vpzldusr.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt2wldtcxtg.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt2btzlriig.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt2fztfzhum.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt2sffafiyu.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2jtebekww.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2qggnyqgv.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2isqdvkaa.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2jysnrkgi.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2yodjsbwb.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2qacivacj.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt2xpjuvcex.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2iqtzinsy.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2zhktlygx.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt2qbhiendx.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt2fnmicqxs.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt2tcqdweuw.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt2xxnilgdt.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2dmummbnf.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt2yphhazvn.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2viyuwnzv.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2gtxmvfwf.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt2wcpsqacr.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt2qpdmyaae.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2ksdchhwl.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2zqhbbfpd.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2fgeaowdg.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt2fpdiymqg.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2lgovfhaf.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt2susipbfr.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt2ttbjiqgx.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt2uvugxkwo.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt2dohsvldk.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2lapdiuup.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2bphzugpx.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2hhutoqga.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt2llirxtlt.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2bpqsmhbz.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2qpsiloue.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2xrvlytof.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2tmggbkoa.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2ayefloui.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2eilhhuxk.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2ksaiidhe.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2kywiihag.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2neaypjff.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2efkzvqtq.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2tcutqdsr.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2zgwmlovy.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2kkldpqnt.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2lkgzbovd.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2llaiymjr.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2agugecqi.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2frbvwnbm.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2eowlnoum.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2bymkalta.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2sujtycki.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2iqvbmaqy.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2xidbxosp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dixecqqy.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2ycdhzjft.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2wvdlbxsr.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2juuzrnmy.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2mghimkho.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2dcymwgyu.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2efgsfltj.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2klmqpljf.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2gwqreklj.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2vwifphtj.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2qkzbkwzw.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2qwffncss.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2wncwgxmd.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2dkqrmqcn.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2wbgvvjor.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2sqhgupsr.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2sdmbsrsp.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2bdjmzqoj.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2ztfbzkol.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2zvjddtel.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2tmwmtthr.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2ixtzmxnh.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2vurenslk.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2fippkfhe.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2oiadzaun.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2bwsamehn.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2fdddevci.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2oekpltin.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2pfcydiwz.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2emzwhfry.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2uoweusmh.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2hicxajli.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2ychnkbor.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2mrcvpdyf.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2sfrsqrqr.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2rapvvibr.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2rrvqbonl.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2vrgvdopu.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2fohuwbfk.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2dgifblzl.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2brrlcrty.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2huinmgxy.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2zzpqxwer.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2sjcumgot.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2sybzkqoh.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2brmmihxu.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2wuwetksn.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2alqslcjw.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2epnhwtna.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2mtapmpvd.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2ysmviwjh.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2zcxkwwnn.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2pqqgfrtz.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2xnaztovm.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2ownxhoks.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2hlzqzmbg.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2leakdcbk.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2qrotiusz.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2xglahaeu.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2onzghobg.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2hpvrlpwy.html


<!-- 参考信息 -->