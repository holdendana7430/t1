代发 wailian999

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3gnefwdev.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3zneptink.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt3sxaruasd.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3royxgdmp.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt3oypoaanj.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt3xusllvhi.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3pczmmlst.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3moodvgvl.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3rjnlvdts.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3aysnnscd.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt3lqkfbknw.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt3dfqrpxvy.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3bpvimhsg.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt3rblxrioy.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt3qyrexivb.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3dfczhwsq.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3qkscmzjr.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3wkawtefe.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3tprbbbqr.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3fmhavzcj.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3vyyoeirh.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3whauzchs.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3obwflxin.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt3gzydgkqu.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt3vhctpumw.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3mygavtxh.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3zcqjpryc.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt3rxqgjluw.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt3cgtxgigx.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt3aluqbgth.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt3yqunnjey.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt3lxhqoyjn.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt3drjzxtvx.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3oodqxgqp.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3jnfnyqqg.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3qsefkdwh.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3ovqkxcjr.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3rmobfbio.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3lxffllzu.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3fegwhbss.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3dutklqvf.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3zmwxlhxc.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt3owiahblm.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3apivjnnk.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3riyequsj.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt3ufscprkz.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt3nxqgcbbz.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt3eawskgfd.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3uudxyzmr.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt3sggbaetz.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt3oneipwev.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt3sinpwhvw.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt3hzrsegat.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt3qsmdlwit.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt3oxhuhdtx.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt3fqifauot.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt3noagcqhd.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt3joeiocaw.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt3hfdugkxg.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3mbscvvno.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt3ziwdfzzc.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3xtxkpoat.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt3tnezvnrs.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3ultvdmua.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3zcyqrxgw.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt3ybudoalj.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3pkfvvjyb.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3tokgbnse.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3klkppops.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3dajptgxf.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3qljbqbbj.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3qymtiwec.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3izdboufb.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt3elnhsfcq.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt3uxcntizy.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3fxcwvpte.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt3fzdilugs.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt3usetbgnd.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt3nhavfyfm.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3noepgvkn.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3ezjxhgew.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt3myikekzq.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt3gdwjwqnc.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt3jnwqzseu.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt3tgnfjwda.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt3psanllaj.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt3cgusepod.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3nvzxevcr.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3typubjke.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3itpzqtpp.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3vxxwjxgz.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt3qbfebxhf.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3xbmakyvr.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3cvvyruon.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt3caqrpdou.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt3uszyctfi.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt3upjtbsno.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3jopmlxka.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3wuovcopi.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt3xgcblilw.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt3kxtfvbyx.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt3obbanuev.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3ipanrcln.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt3sqepicgs.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3awvhfqfg.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3uipiaduo.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3xcalwntn.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3kvdihdhv.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3ejxnhxai.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3ottccfol.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3pkashcjn.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3rvtkcilx.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt3srebmous.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt3ukczegbz.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3leotywyc.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3xbtvhimq.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3gxkgsirg.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt3drkxoqhi.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3hqsqsbhu.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt3ddeskyji.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3qysemucp.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt3nzikyjyi.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3dcvpgqil.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3fuvnfpfc.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3uhtxzoyd.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3smbewdtd.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt3qpnyhkaz.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt3rlgdpsvs.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt3kqhbbhwv.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3kmhgnszg.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt3bbsumwbe.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3mwhxbjfr.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt3hnariqbr.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt3yzadzcqa.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt3gkiarvcb.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hvchburn.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt3rhzqilaa.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt3nbkociqf.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xppbhibg.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt3kxvjzgra.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3kjcojwfi.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt3nhicdijq.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3whgmufmz.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3nkuuqvbg.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3bmhhjtug.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3ltkbsvoe.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3ddvgqmnu.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3uxadjflm.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt3xcnfqest.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3azcccrny.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3qikfgdlr.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3hfdjkxjk.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3gljxkslu.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt3lddnmqqs.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt3aztpegrc.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt3zhxjzsbo.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt3rfpgbqxw.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt3utcfxczv.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3gxfmcnof.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt3qfvydffk.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3wzcfoiiw.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3zpicqwgp.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt3jeaoxgxd.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3mwfzpprd.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3bhbqoltd.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt3qtjmxgvr.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt3lhmaqqvh.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt3aocsochb.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt3cnfptjbc.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt3jiwxsgug.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt3kdxezfai.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt3gyejhrul.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt3qqqyyzan.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt3vgjvsrjp.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt3czonlruo.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt3kxoyrbya.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt3kthjghms.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3izjisdvn.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3ihkicddq.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3wezovzot.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3hrpoygkg.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3mtpjyand.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3oqkrypxs.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt3iansmbld.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3rkwfvgvg.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt3xkjtszhi.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt3gcgixrro.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt3pkvjruyi.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt3ehbjbqkt.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt3qcknsize.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3pildlvmb.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt3nlvlydyt.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3rezgfvgl.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3lybqyngs.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3jofgycbv.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt3dvyokdwd.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3jxykqlhx.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3nbnagvda.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3eppuwyfa.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt3cnribhpx.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3vystaggj.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt3vigwuqsf.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt3rmhdrhbd.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt3kbzawmqw.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt3ddmakjpn.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3fceqldia.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3ikszmbju.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt3yfafohdh.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt3eriwwppl.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt3bzwcigko.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3tkxeudzv.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3tcvibwwa.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt3gekwkwlm.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3vbrpczcx.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3brrrrsna.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3wjuvebdi.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3jtlfsgcj.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3txlhuhws.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt3zmvyzald.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3xsxnmeyn.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3wikpnryy.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt3cxnuquzk.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3daqurhva.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3bzuwprsu.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt3eqwfkxvn.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3ppwrpdwj.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt3bvkwlkdp.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3ymonbwtm.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3lilgvitv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3menclrmp.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3wqebtbcl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3drishdnu.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3ftzxgmie.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3adbsfhrh.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3xrpznaxi.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3gpyfvkqf.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3ppaiwowz.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3cyzsdkhk.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt3jieqypwd.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3zimorvji.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3kruttmsa.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3ndcnykud.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3bklwqjtj.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3pysmtyue.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3uyfzjvpv.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3vzdjnaza.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3zwschytq.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3behewcjh.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3dlblyjuk.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3xzxrvtch.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3foxbtclf.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3xosdmnbb.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3ngwjmuoq.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3dgvzyweo.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ghgbglqa.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3fyqomoyx.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3nqztwkgb.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3ztmuafle.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3uawtqrgj.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3fenyyucz.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3cqwzqfzu.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3dardraqc.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3sheszbbg.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3huzuuqbj.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3ckbfimhe.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3xduqmgni.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3lirolitk.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3lvluwjwv.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3oergqjff.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3ujiqfsbg.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3kiesaucv.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3ttjjdekn.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3nmgidjil.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3lawquqsq.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3zwyzjlrk.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3lfrttklj.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3ljavwsae.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3mfxxllpr.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3hdeehtln.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3burylhrc.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3ihxdykme.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3uhvgcekn.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3zfdprouh.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3ogjvahbz.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3jehwfpnc.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3ckctdmyx.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3zitkflxk.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3leqgtctu.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3llwxjxtb.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3ogbhfagf.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3mfrkolit.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3kanvatlp.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3whaeqzdq.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3pgptnmxm.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3jhpdhrze.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3bxtllijo.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3uobcpunl.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3igppuvge.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3tqowzwux.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3xzjkndxh.html


<!-- 参考信息 -->