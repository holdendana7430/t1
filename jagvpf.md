代发 wailian999

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt3zjnwdsaa.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3pmhqkmui.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt3gtbirheg.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt3yvwyppvk.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3aabeanvl.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt3matqpqlg.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt3ezmkyzks.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3tphcchur.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3jxmibauh.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3pccddfyy.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3xyvossbf.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3fdwtsqwm.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3redvpshg.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3xykhzauq.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt3issrhgdw.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt3enuonvtx.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt3pdzpxyyz.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3alynwusf.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3egcgqcku.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt3imyebufw.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt3wsotrfdj.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt3gzxztbyy.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt3srtltqku.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt3hqfylejn.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt3xhkuzkrm.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3nqvisinr.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3sgibxafp.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3sxrmgdev.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3dgmbepis.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3pmighxhh.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3ozzduxzs.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3gkdtrros.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3ymirclaq.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3ajvkwfoy.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt3prlrnexm.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3mddadaxm.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3kosfojax.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3bwuistkv.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt3okujkkev.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt3evsadbbs.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt3vrfalruz.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt3epmvgkxg.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt3rrbxjzhm.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt3evkzlhqr.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt3jfapzsex.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt3vyddsksa.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt3cltmddxa.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt3ykultygd.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt3vtxvwdxh.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3pftmtpcb.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt3sftrlgoy.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3sjfmdpwj.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt3qkvhikbb.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3cwoimomg.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt3nmbimwgz.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3ieghosjs.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3puqsigks.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt3wwkmdzvh.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3lhgybyij.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt3shicbcik.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3vpvkusxo.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3gnsycvsv.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ayyojcvt.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3aexqvjfg.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3yxywvwhv.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt3rsskgtbp.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt3zhvitduk.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3fqyrvxlt.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt3ygqzofgh.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt3ellzyufh.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt3tkjbajnk.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3gfhyjicb.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3thwkajor.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3jquxilzq.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt3pzevkedj.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt3fwmupira.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt3gnzssepy.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt3rtgvzqsl.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt3mpdlccet.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3cuxtwzfw.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3elfjokgr.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3egiibzsm.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3nkeshgqv.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt3fntrjlau.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3grjdydyf.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3whrhagst.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt3admpaqsm.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt3niqsmwlm.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt3hlhfngna.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3kvcwebyn.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3tbxmbhxx.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt3crcgxyqc.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt3rtwqsabn.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt3yekntnfu.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3vsmysqaz.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt3qcfusdpn.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3ffabobqh.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3trzfdgoa.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3stzdcfzv.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3pdrycicy.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3imriwcjs.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3cweolsyg.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3rfbmnrmd.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3txxhagwr.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt3gpqdejbf.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt3zszxcrje.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3eqhbostu.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3nrhlohrc.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3biyraavt.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt3uuycqxeb.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3ueaopwso.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt3mpbibymk.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3fokjxurm.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt3qwvtxbkk.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt3uowqjsiz.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3zrxawspq.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3jhuutyec.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3sshormyg.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt3cjdvrbdn.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt3uoofosdn.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt3acjpsoss.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3norwztmy.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt3evtcihhc.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3ourievhs.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt3tzkdemfe.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3ppgljmui.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qktriyrx.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mhxqtvkk.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt3kqppncnu.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3kvsziwlz.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt3mcqdfhns.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt3vtikrjuy.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3zefsdlgr.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt3rhobxwhk.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3hrfmhlcx.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3moasidwf.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3pmgeeeuy.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3bnvsxnys.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3emxqpxin.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3zjszndfn.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt3qtvebgfb.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3ugmrowlb.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3rsaquney.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3frahygxp.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3dzwixtrk.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt3krknqhrx.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt3nligzwcm.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt3abueyjcy.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt3zuztphrw.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt3wioslune.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3tivkfqqs.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt3blukfnen.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3gmbfoybd.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3iaclhliq.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt3pxfyeiok.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3owvjjqdk.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3gnthuipx.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt3cxpqriwi.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt3mbjyhadv.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt3jxphyggm.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt3odjobycz.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt3civransf.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt3pyeahlhn.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt3aaclwoti.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt3wvtgijzs.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt3orfixojc.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt3ejgmyhie.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt3ivrhisri.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt3hbwozkbs.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3whloiiyp.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3fdztqbqw.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3wqgcmoez.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3neeeurza.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3uckephgt.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3iphjctlh.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt3rgokwzoo.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3fxhqylwz.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3nlrshlqb.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt3lwfzkvwe.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt3cmpgnoon.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt3ckozxfxt.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3auxljnkg.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3oatqsazl.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt3wxvqciph.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt3ffnnjjdr.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3sayezaff.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3owowjjcy.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt3shzirrim.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3gmaiabgd.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3rxqucvto.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3jvzrzgzv.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt3zeukfnim.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3pppgwbzh.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt3vynxbdhs.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt3gjviljnp.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt3micjkrss.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt3ckuvrrfm.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3etyrnpxu.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3utuculvx.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt3tjyqcvgs.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt3xwnzpgis.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt3whfjlfva.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3wuzimtpl.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3cbgvhkgb.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt3ijavaswb.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3wveoplwm.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3lkbtytgm.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3wdhoqkok.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3swcdxjdv.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3vtdozfgf.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3epgyxajo.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3vuojtksq.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt3xsbfzudk.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3tkcprihg.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt3nqiutntg.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3cicssgre.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3fxppploi.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3nadwkidn.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt3mfqbnrkg.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt3ojcolweb.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3zwyoldlv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bltripwu.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3gbpwiwrk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3arsozsya.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3humgswdb.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3gdvmbwxo.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3hjlgdeoy.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3yivnboup.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3tcwjcdcl.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3evjpzhzq.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3wgkarjxs.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3odldawxg.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3yqjsffmb.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3qgpbjlkv.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3fcpwqioj.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3olnpewbu.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3cwsfphji.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3llbliurh.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3oiqbktpc.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3glaxxjhg.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3ciwnvsws.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3wvibbwas.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3ouxtzywp.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3zatjlvbm.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3kmtixrdc.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3rqlxdqik.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3hhndfkcs.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3lfbvtlfl.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3cnaavndh.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3ohgqvroy.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3rvqabhvj.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3jnjoijds.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3roddhegt.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3nnjjioil.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3zzojhmch.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3puzqsefu.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3coguwcsr.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3pxcpanwz.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3srosfjmd.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3urzbdjes.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3aydqpzsr.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3iojbrfmi.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3bhnpiroj.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3wopcnxpr.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3umjktukb.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3topsipif.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3melmlrxy.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3ezalwplp.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3ycyiobna.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3diextzqu.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3mygbbkyx.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3nfgndixx.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3rvzmlidx.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3hxjzvyjm.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3zvmcnbmk.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3huozqnqt.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3lenptwfu.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3yxhezblq.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3fccaorvd.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3zhqdvjsa.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3mpssxbzk.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3ylxxuxer.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3uwmhiznp.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3skazebvn.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3mmwhzpbn.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3dmntlfcd.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3fxukxfsx.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3xwgrixya.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3bnmsodjs.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3yxdqlvmf.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3kjcdhrna.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3ugywgfhs.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3fyirpqtm.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3lhcbjvbr.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3clqkvihb.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3iqzhagxl.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3osdvfuyw.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3yhtyaywu.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3ttjauogc.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3kpnfanvv.html


<!-- 参考信息 -->