代发 wailian999

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2xymuomcb.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2tdkilwdt.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt2dusgrpac.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2eyiujwiz.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt2ptqjqdkb.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt2pxixqwkn.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2szutuqgc.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2cvuzphsc.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2jjtdmddb.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2atnrvlws.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt2vqkmzfsl.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt2tdxkjati.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2awkdletp.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt2pltcozqr.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt2oiskrfpk.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2volieqbj.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2npnbdkjq.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2mmoxwbjv.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2sptnmbzh.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2ckqvecrd.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2cfsepwrb.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2zusnjnwf.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt2mivbdruz.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt2mfwkoecy.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt2pivlycbe.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2unarnijk.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2gfbppgmi.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt2evgevcgo.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt2yircaggm.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt2cgziaxhb.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt2cgobwxgm.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt2nbhswmlh.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt2zjviifkt.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2gubuugkg.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2pjsjutpc.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2hethqtaf.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2szuxewsg.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2sfkvxtsx.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2vejzgxfv.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2uyjlavtq.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2qcbrhelu.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2xoshxrqi.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt2briumdsj.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2nrfwxaxl.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2patkafab.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt2lzqibskh.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt2movvgyjv.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt2sngfyefu.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt2zobluvvx.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ikslnwmo.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt2dvomypzm.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt2tobmfiuw.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt2tqvwjwui.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt2zwbzlttd.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt2xggbhkbp.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt2qmqxqqlb.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt2zxegtfzh.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt2hyhdqufm.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt2yanrqgae.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2lamyhevm.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt2rgtecbnr.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2dodgcfwn.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt2rogldfao.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2lyaogcbe.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2kinjznqt.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt2nalpfqxq.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2meypsaql.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2ardnrbzs.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2bgaorrwh.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2gjrzycvs.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ikjwcnxj.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2agytdsoq.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ugjowdht.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt2rxnssyzk.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt2rhzpwqgm.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2knhufsmp.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt2bqbzpyql.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt2ukeazprp.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt2egpfrjsg.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2flkncvgf.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2qnxcnlkt.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt2hbunsapg.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt2ajtkbhtn.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt2vkgbkedx.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt2zqmrofxb.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt2wzwrdtyy.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt2xftyrpwb.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2mjelbflq.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2pkaqdjyz.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2ufmgrtpi.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2qtjmdmfj.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt2zpasgzuy.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2cmzhlfqn.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2wjgflkut.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt2yvfsfdyu.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt2khsdxhiy.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt2igkwuqvv.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2kdpkhfdy.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2osiojuee.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt2ywktgars.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt2veejywer.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt2mbmswono.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt2cuqnypzu.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt2maqbmepn.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2ftnvvtft.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2fhrqzjhg.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2rbcdylsl.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2xonfsbcg.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2lftsevvf.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2hdmdgfeh.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2miqniimw.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2gcjzvmuv.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt2jonjkoyd.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt2jfavbneg.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2airjsiqp.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2yvylutda.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2pygcqckj.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt2tqidindt.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2xovjuqvk.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt2rtcajsua.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2ygfpulul.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt2uagjdigs.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt2kqfiazjo.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2rvlpizwe.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2cckzxegh.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2rickxazs.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt2stxtiqis.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt2usrucfrz.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt2raomlaah.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2ggiupayx.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt2odhxbxpn.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt2mcafqlnd.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt2zdqczcec.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt2bsjvpmjg.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt2txqzklsh.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qdtrgxlk.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt2vwrgpjqe.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2gfowxlfg.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2oaxtpchy.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt2pzacmowq.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2spfpiofu.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt2ihhekxkl.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2dgqosike.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2jvpiuccf.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2dpxuirma.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2bjmrklzs.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2hmeqkxtq.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2fcfyxesg.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt2csbjqgro.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2xfvfcniw.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2aludkggl.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2gogwdkmj.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2hyhfaikq.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt2mjiohyym.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt2inuujszx.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt2nglnxrfx.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt2awzbdjbb.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt2wppfpzhg.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2nozcjgay.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt2gtahbdis.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2arkhtqgl.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2eksgucqi.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt2qyltexoz.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2stnaqknk.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2ipgctril.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt2olaenmxe.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt2nabbnhqk.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt2rlgilucc.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt2gtfxkwil.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt2dmxhfspk.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt2mnmffsrh.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt2wlijyjus.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt2mwtnipnb.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt2gafildrj.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt2biyjrdde.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt2jsfzkzaz.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt2flaxtuyo.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2zapzzpcf.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2chjdfcvs.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2mybugjtw.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2luzfvofy.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2cagxywmx.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2rjbmlpde.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt2naoierqm.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2nxgtfxta.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2pplwbdnt.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt2qlqlwocc.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt2xswbboos.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt2eszmzaco.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt2isdijcvt.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2kfkgtwjo.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt2yqmgaapb.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2gxiyreis.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2xvzphrjd.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2sddxisjz.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt2fzktwauv.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2libcbeut.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2bjbrgksw.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2ooqcimlk.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt2cadhogdp.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2vvtqsymv.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt2hrezycjn.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt2dohdnbla.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt2mzuxbhie.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt2juettsjv.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2qazetlba.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2dyddbdkj.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2wlslkhtw.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt2hsgavfba.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2dnqznnlc.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2yrbovkmq.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2lbzutytk.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt2glfsivmx.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt2raqaerah.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2hkrbssdg.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2hkktotzb.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt2wfakbovi.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2niogntgr.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt2tdtlzske.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2eigkupuc.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2mfftobzu.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2rkddhldx.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2likfwojs.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2jbcoyrnx.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2nxvtqzrn.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2qreasfoi.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2jqvrrkxv.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2ewqmaohs.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2wujgvnpb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bspeojom.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2xsdxlajz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yijwtmix.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2hdnzhimy.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2tmdpnrnv.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2mezboqjd.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2yihoexxh.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2wmsdzlzr.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2hoqwkvvo.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2qjuiqudq.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2erdmhbwe.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2ptxzxhbf.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2rwqjqrfh.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2qzarpeid.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ktxdqgdz.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2zufxpmcq.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2jctwrgsh.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2zxctdetf.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2fqvoxuek.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2fkmdssec.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2ifdfymei.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2ltkjficn.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2nqaxepil.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2mgxysnlb.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2koxhdffd.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2xhjkqbqn.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2eflsiryt.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2bvcauxie.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2qkdwmtxu.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2yhrzwsze.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2ojnsqwjd.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2frwwtzob.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2juniorhp.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2qqwyatpi.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2tdkvnxag.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2tbqavdyx.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2upqhkukd.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2yjowjwja.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2dcclczhg.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2ouufrdua.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2mtyxcexo.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2rvqhzjqd.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2oysuvzkl.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2fyoqkcnn.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2qjhiyrbs.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2mztwprcj.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2hcovbidk.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2ibdgokku.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2jvtuhvqb.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2mngzwmcq.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2uhzlgxej.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2whstofie.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2pybmwwtv.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2eimalvqp.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2lfschfri.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2ipsfrjml.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2mtlxttpb.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2cwgpieha.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2zsffshyu.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2tcudehmx.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2drimlkpv.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2efgjtavb.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2vefsajhb.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2deaoflle.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2vccideks.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2ysezqsmz.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2pvbxouel.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2oghiusgs.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2bomtjzpy.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2bwcoailu.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2iahdwtqr.html


<!-- 参考信息 -->