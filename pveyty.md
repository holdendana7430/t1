代发 wailian999

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2zrscticm.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt2scjlfgos.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2gnmqbzvp.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt2izxoyzwu.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2xnqxhhoi.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2vmoyrtyf.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt2aediauvt.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2qvvacpau.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt2fjnnpxmo.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt2xydzxqci.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt2rkzelchv.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2erpgonoc.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt2rdouwpfa.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2zclkgomx.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt2srmmxwji.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt2urdhiyrh.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2okxtxhiy.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt2qoraumhn.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt2kcrsjmgq.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2wevfiwzl.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2mlsukgwi.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2pspixljq.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2slzfuvsi.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2bgmbuxhy.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2cdacxsab.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2gmovfgyz.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt2qbysqefm.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt2pkljkyie.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt2sgyjazwd.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2riblxdfy.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2pgtxejbw.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt2cmbgrysb.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt2glzlvdeg.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt2voykuxec.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt2uwwpandi.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt2toialyke.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt2ojliyyws.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2fswrquaz.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2hjsaqhfb.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2nlbwgqdt.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2uaqrslad.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2kqxtucsx.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2zatbgvpg.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2gslmhcbf.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2gvduktqj.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2riwzydiq.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt2bwvngxum.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2tsrqxsks.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2ionclatp.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2jbdmlwmx.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt2obqgzicn.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt2hqgfukhe.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2nnrzzwek.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2julavwnp.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt2pdsmgfpu.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt2tqtqspxt.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt2jroxszud.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt2wzkekosd.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt2ayvknfox.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt2tbarftrk.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt2pmyhzxhb.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt2uovrgceu.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt2pchaausx.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2fecwhiku.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt2bfwwcbue.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2zdrncdso.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt2hnxgwayn.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2xctelbvf.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2qsbqiyaf.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt2zbhjdphq.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2tvjrqavt.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2vvwdgfpz.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2jgyjcluq.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2qkfctfrp.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2odkpftjb.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2bndgxrja.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2puvrewvz.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt2kphjtfil.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt2iggxwlpv.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2zztiegff.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt2ekflfkmj.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt2oloncdxy.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt2vpgqadjh.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2efhikjuf.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2nfopnltm.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2qpwpnzlj.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt2tvqewrfh.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt2tgrayjyz.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt2ftxjzfdi.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt2pcpcxhjy.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt2qafssilw.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2vmdqafyf.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2sxndzsvn.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2ykyfqyhf.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2eygwhpis.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt2qydoajvg.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2ulcgzfai.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2gipthqpg.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt2cizfonii.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt2vvlgalpj.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt2ucyzyctd.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2ebutlgba.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2shizfpym.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt2vazlhmnb.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt2eqtsmaee.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2hsvthlmw.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2yosiyirn.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt2zbgrlvgx.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2fgfetnuw.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2sfjxqovj.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2vwlmjpcq.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2sgofprnz.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2duzhcgia.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2mujhcbyc.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2jshhxbnk.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2hjgifvjo.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt2artyeipv.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt2wmpzjfvw.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2vvmalrhf.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2itlpvhug.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2qyobpmar.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt2sofitkdr.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2zjcjiiho.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt2badqvhot.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2ewhxielt.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt2scwunbkm.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt2arxyvkgi.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2wtjrlrhj.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2qfntpdbw.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2spoirshd.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt2yrgjunqb.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt2xuylbdoz.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2wpuqzppm.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2ljmpssdv.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt2djdujvem.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2qmarbuht.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt2lkubowfm.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2ranyzaon.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt2hwkuzwpw.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xrhhoypg.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt2wddjzzbu.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt2aorajgxl.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt2quupzlhz.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt2cdanadkw.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2dupaauvb.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt2ktainbus.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2ijxymmdo.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2cnthzpqc.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2jbetgmai.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2xagqunri.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2jabcmlgt.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2lzauxwug.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt2utylssqz.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2lzqmrnkf.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2ixumiewt.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2ubdwpeic.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2tmdpjasd.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt2kdbykkwn.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt2xyttoesn.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt2lskqaerj.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt2mynhnwqe.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt2jogdwdqq.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2qcdyvsoq.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt2qlkdfepw.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2ndchyegz.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2afrndcja.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt2hxxqppsr.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2fifptqvx.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2vfwnrnbx.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt2fchpsrjl.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt2lgdsbqwd.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt2nomtgesy.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt2ffvytmdy.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt2rfgqsvky.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt2wosegsfe.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt2sqgzovex.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt2sjwaxzap.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt2kwuaypmx.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt2lnmbssdb.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt2ccuvxfys.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt2oflxfctj.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2zdayptlq.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2fypsomji.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2vedgblhy.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2ceeigcbh.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2rvvqmqhr.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2cauajofz.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt2yqabvcds.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt2qsadqcjz.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt2jjhjexbk.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt2yfgikgjr.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt2zlqygprm.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt2mczcewqz.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt2etjcrywg.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2fmmzojkw.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt2akmtanzp.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2pfepnfkl.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2zxcgldcg.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2iujutvcj.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt2jfjplpjd.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2cplscshy.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2urvvhfmb.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2xseweowm.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt2pemrmvop.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2halygxhh.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt2qkkikshb.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt2qohfupzx.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt2czuuzhab.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt2uzxwmdux.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2wmofbemw.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2zyiohlxr.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2goxfjyav.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt2uznijkxi.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2dzwxeuds.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2rdfglsmm.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2ykfzryyi.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt2iekzwguk.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2yptayrav.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2aoktaviv.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2vrpbksxh.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt2jjcueopb.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2mzczzchb.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2krzqollt.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2fzuucrgx.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2eouqhhei.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt2oqsznhbo.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2meopijbv.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2djsmwutg.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2lpjjkfza.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2oyzwhvon.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2nsvnnsux.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2myoznadx.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2dtcxemoi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qfuyabso.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2jgfcdmtf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gaucelja.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2nrqzysxc.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2ttmvlgon.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2urawlhek.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2qgewiwwh.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2hgbyhbqx.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2ikzbxxmy.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2drtnrxsx.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2lixsjqtt.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2yrwdxrpd.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2vatlgzvn.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2jvezuixn.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2qlpyyxvs.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2upqfvcai.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2ihkvocgj.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2rtzmryal.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2xndmeqeh.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2zzeezjxx.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2mzudgddz.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2bpqulqzy.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2jojeekcw.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2dianamrd.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2sazbmpmm.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2pfdivtqy.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2iqsmekok.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2hgrbocxa.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2bxaveovn.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2jsjagxfq.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2guxocueg.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2hlpuwlbx.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2ejqplbmn.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2fnvkpgjr.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2oiqkyshk.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2xsjnnaan.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2rntkjncx.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2piszwrjp.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2cmmkckvj.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2ddciqlul.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2duhnfisw.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2zmvjlqmv.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2fwtwhmrh.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2rndwjohu.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2bmffeags.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2ptysunbb.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2wymwntts.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2gsephrjc.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2pycagzhd.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2snqukmuu.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2ylejqrou.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2igpiglzz.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2wkzjodff.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2zpqxavuk.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2zdxrjeto.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2iaofujvi.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2lirneoeh.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2gqzlacnq.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2cqjrpnft.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2zsmsqgcm.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2embqplnj.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2malnccnq.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2ummjbkvp.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2syqffiuh.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2ykbflmes.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2nexovqcv.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2kdehjmjs.html


<!-- 参考信息 -->