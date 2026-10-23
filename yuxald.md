代发 wailian999

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3daeusqaw.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3sfpxokfb.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt3sqylnmsx.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3jiiqzfib.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt3xrjapwyh.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt3xnfrxgty.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3wwhyzdsf.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt3mvaqebmj.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3wgkfbwol.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3xswpqawm.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt3zzxbpjvs.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt3jksaeyjp.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3mntvahkv.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt3fsgpiiwp.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt3qewaogby.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3zarguahi.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3rwvovuiy.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3fftfdrya.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3ohgeozyt.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3zlnxvogo.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3khmjrklt.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3frijvhnj.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt3sdwjaokq.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt3wsziuadb.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt3qxubwrpe.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3ytwvpdxj.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3gmixcyzj.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt3ajaguync.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt3nioakqzk.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt3tweokdtf.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt3skdeatfb.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt3jdwkvkrs.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt3dieiwdds.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3xosdjebr.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3yjnnpgzl.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3bxmcyqxu.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3axhclaxm.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3vetefnrl.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3stdfaasl.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3hqkwzuhw.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3gcaxervs.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt3ffrjfpsx.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt3zavgduau.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3dzlbrxbe.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3sfwhiwhi.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3xhhszwjz.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt3tbnzggyn.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt3bhefwhqz.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt3qxryafsd.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3mwinjszz.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt3vhcrjhkt.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt3sjabrpym.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt3doinzscc.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt3urcpkhxq.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt3lszelesi.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt3wccdnsba.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt3yqijhslw.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt3kvrtgbgd.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt3seyyrbxg.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3zbhjvzlt.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt3wdsybtcv.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3dkhyrgxv.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt3gyxhucox.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3ctdmkdqj.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3ihkoyheu.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt3zwjaqovh.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3ykccqsbq.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3ugtixgli.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3wdckyzvi.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3qvqvudio.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3fprcerjg.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3dnndvsfa.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3xpqjmkvg.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt3kkguegwg.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt3nctwbtux.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3unugtvyy.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt3vywqibgl.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt3nllowlii.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt3uyleghxy.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3oldffclo.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3xkkgqwzf.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3tglnnqhr.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt3ynqrgrqw.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt3nrevhnnp.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt3wvhsuhjz.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt3outegimw.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt3cydgybqa.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3lcwvkzpu.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3oinkrzfc.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3qqyvxufc.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3uwrlnfti.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt3msadyngp.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3iruusqbw.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3vvyjlzpm.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt3papxdcop.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt3kvvhdreg.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt3hdpfycgf.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3ckwqpjpp.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3jmnozszq.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt3fziavszt.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt3iqpdvjrn.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3vnmawkcc.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3wjfmrriy.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt3drfdguzu.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3mxsfqigx.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3sttoehhm.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3sgfbavny.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3cyerhxek.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3wnomkmgu.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3ayfhofzw.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3smelwwjj.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3dbphcqqt.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt3awuwlqil.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt3jphmhpmf.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3gpscrrzd.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3bphmbhbb.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3uosbjfbi.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt3dejuildw.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3bennsrrl.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt3oqcgcywr.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3yfpszwsr.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt3bmaogieg.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3ikkfsskr.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3piqhjisv.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3lxfcwcfi.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3kqxtcitk.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt3grcfench.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt3vhsyjufd.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3xkrzdomg.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3decqybph.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt3yehkatba.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3ounywylx.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt3nubnfrrq.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3kgaebrjm.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt3loeocwrx.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt3izgszfwn.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt3jegerpwi.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3iskrhvvr.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ingeahef.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt3bikwdrcd.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3rcpifqwi.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3quprdhkn.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3dbkrkomw.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3egvjvivf.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3csiuxksu.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3kfwdmkpj.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3zgscjlre.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3itzexrlm.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt3bbskiorl.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3wlhtfaoi.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3sfqthvpa.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3qrcpqtom.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3bntepupi.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt3kasoirof.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt3ivzirkeb.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt3gfrimirc.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt3ebfuetrk.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt3awwguasq.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3hxgvdllb.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt3csgxtzaw.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3eysqubcc.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3xeapqpss.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt3umyhcjlu.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3kcgxvkuw.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3avhurhik.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt3bgfuidxy.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt3xitoqjpx.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt3ugdhjxts.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt3wkxmthfg.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt3ablzfhco.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt3wohttoed.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt3kzfdnmkm.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt3zoxzmwag.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt3ddjqlyyd.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt3owubivfw.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt3fxhjimkg.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt3hehpaeua.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3fhkdafcc.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3aetjbinj.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3xwzysxzg.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3ozdgdbpr.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3pmycgybk.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3upepwvvl.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt3fikmbkpm.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt3wgsibeci.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt3uccouout.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt3akhlsmhd.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt3lfjveqre.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt3atlzyyfm.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt3fzndvife.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3isfmvryb.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt3qkvcmela.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3mnpwxqmv.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3vdnqxtty.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt3cwlmyfgm.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt3vtjrgjaz.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3goexgdme.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3ppvghwzo.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3hfcolzze.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt3zfcrpimn.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3ekrpbsxh.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt3awjupzyu.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt3gwpbjanw.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt3qodjtldg.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt3rtwrobps.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3swflzjrd.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3omdzfcdx.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt3zzmuacvu.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt3uivenwak.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt3yrnyocya.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3xndmpfjw.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3sivbkelt.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt3lhnahhbg.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt3jyksowuz.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3zazowwaz.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3xhblaruo.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt3fatiihkz.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3hwwyvied.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3tldgpkes.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3uvfhmuog.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3ayvclgsx.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3nuaqlutz.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3gqlwyalf.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt3jeorlxfj.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3lerrylmm.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3hkyiulnf.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt3ivwqccaz.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3tyyivjtz.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3yxjmogla.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vzpjtuwz.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3tfvaphks.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3goxsyvtf.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3xbzbuyrq.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3gezciwxb.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3yuggugja.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3phnuzoxs.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3zqefchkk.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3dgbfvstq.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3mswahbkz.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3swalvolh.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3fmwasbjw.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3dkyqmmyz.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3qaidwgxm.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt3novxnuvi.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3gsgwuayu.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3ecbtxbaw.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3lakpigcr.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3dtvtmkxf.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3rtlphect.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3opperxtz.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3fruigxqu.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3wsbisjcw.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3mpapfogs.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3ceznsphf.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3hxrnkkvt.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3ueybuuuj.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3ejzeajth.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3hldpmfvd.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3dmnwyvbg.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3hpmajdjo.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3tqgbaond.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3yhjsblak.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3zrtiuegj.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3ibfmbjsy.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3mxqhnugo.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3uzggnzkm.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3kneuebnr.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3ieenerfl.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3wifyfgoh.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3qqtcvhzb.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3laiiflwd.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3rpepwrfy.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3bkizvopr.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3pgejpejp.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3snidfpyh.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3kbmazaxc.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3otizyxlu.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3bqreahak.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3irbmnqwn.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3roppkedu.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3ucbmobfo.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3jfntzogn.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3loysbayo.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3rxmbqzfw.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3dpxnliri.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3pdpgoxkd.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3ietvbywg.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3ntcmmoha.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3goxffnpz.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3soqzfbcv.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3bkfrbfhj.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3fwjjzirh.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3xtrseram.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3exhztrey.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3rqbguals.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3gciimxob.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3iwahfajz.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3nvnhzjrm.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3fbfncgas.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3lvlpzyce.html


<!-- 参考信息 -->