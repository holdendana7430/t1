代发 wailian999

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3pmxlfjfy.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3kskxagvg.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3qdovwguc.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3arzywmbn.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3azmnsjyr.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3dpfwszle.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt3lkqbejha.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt3ejitlkrl.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt3ffckgxfj.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3qwixqwlu.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3zqfecfih.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt3kwysljin.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt3hwlkqvep.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt3ieyasqmq.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt3jobyhubo.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt3grqwkopw.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt3btrcsnkq.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3mmndezsj.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3mvbdsoac.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3mpodriuw.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3kimzgibu.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3svmjyewm.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3bjtcbxcg.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3nzxphqmf.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3vfkgyacg.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt3sdkhfxfw.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt3pwrhgdjy.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3itogehcr.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3hjxivdel.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt3gdcvtrhj.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt3khitflic.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt3sualvszx.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3qipoekan.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt3dtoftvsg.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt3isdrrtxq.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt3loezikyd.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt3fhivefac.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt3uewklxdx.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt3fukkzptl.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt3bmpvtdoj.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt3olzkkfgk.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3cocmoias.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt3ykedbqpf.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3uufixqmd.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt3zubnhkpw.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3kifpahvw.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt3pwaamoql.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3trlezwjc.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3lftdrgim.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt3uanyvmxg.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3caubhxzv.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3unrqcqqo.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3qihdcfxr.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3kfqhmotl.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3yqgfvxyq.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3lrmjncmu.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3rtcpfhxa.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt3yyouafwj.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt3qsvfkkzw.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3oftimphg.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt3xnhtimog.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt3mnbbxqin.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt3uwlgxfzx.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3wsxufcsm.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3dmhevskz.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3iwseqdcz.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt3jbcqartt.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt3gefbpklt.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt3fmbhwclq.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt3hkzjzevd.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt3zwjckjxd.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3fmvmgvoh.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3iljlsjfw.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3dgsaoykg.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3wqdhuedg.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt3cskqyxjc.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3xjoaprlu.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3dpslasbd.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt3kofwgywh.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt3kjzzjzez.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt3xamxvuvp.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3oorrzvnp.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3iqdxmosl.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt3rgajuplt.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt3tsfwvnwb.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3zqmpbdae.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt3tzifarel.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt3rfabpwpp.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3wtwujhma.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3qtjpbelo.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3tntjmhcr.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3etoehsjw.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3rfhcedzf.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3qspyrina.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3oqxgwecw.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3ufdhdmkd.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt3qxtkcsys.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt3redpfobo.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3venlevre.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3kywrholm.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3lnltukbn.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt3ojhnanwe.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3muasmume.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt3vepkyngt.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3lnvqgxpp.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt3lujalbbr.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3ofbmcind.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3iquraofm.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3bpmnhmkd.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3ptjvragb.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt3jorjsthx.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt3bcyhhubw.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt3qdtjsibh.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3upggeoao.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt3dqxfximm.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt3acftkwbb.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt3bypifslt.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3usbcblql.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt3vnrlhebx.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vgnsvsik.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt3wmqztxqg.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3hxxozavs.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hgeauzce.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt3ahrcupcr.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3zwovrpjk.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3alcqxbya.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3biyajegq.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3zpiwnewe.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3ienkkdax.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3oxulmwgt.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3qxdbmyjz.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3nqspyreb.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt3pepavbke.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3blmufvqe.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3bjhuxgrm.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3gwnqbwck.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3awhwrsbk.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt3xhdrakqe.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt3texiwmsm.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt3gfnulwjz.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt3ofjmsjnd.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt3tkkcbcxb.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3xpotpzrh.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt3kjxpqaia.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3aadudjpd.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3ugtzsopl.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt3uludfvke.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3fxbirzqc.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3gvrtjled.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt3pntzqjlf.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt3xywtaaqv.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt3qgrszios.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt3aorfmmss.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt3shzlxhdn.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt3foagidvt.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt3ntqsqaci.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt3hqhprqqg.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt3uaamnyny.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt3fkctujlu.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt3ufxofsak.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt3vlhoxdjn.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3bfczdtwz.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3olefcpel.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3mraexqtc.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3jctkcipr.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3sldmrmyt.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3vqsiacnp.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt3junucrgl.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3ouekvdww.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt3oinzdqmj.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt3teqjylcw.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt3exjmdytr.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt3mzdzauec.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3qmixpmii.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt3fhpptcsh.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt3izbqjvrr.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3spbzzzqd.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3xesiuekm.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3wwwqnnas.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt3rulnfwme.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3guknnifs.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3omdedjsm.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3zmemfirz.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt3lwpxalbx.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3efzorvrl.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt3fyvexjgr.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt3aoropfvu.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt3sfztxjtr.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt3maaaypqs.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3mlqvjbpo.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3kusdekjs.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt3qfsplsps.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt3wivjczfk.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt3ybktoofd.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3vlvyubej.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3spnqsirp.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt3pfwglymd.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt3ycrvbtof.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3itmjmbwd.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3heaprlpi.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3bngdlasp.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3dlwcjyko.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3afrezcfn.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3wzgdzrer.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt3uvvhvzzr.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt3vfjiroco.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt3sgpppbfe.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3ihttafwh.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3pxsakewa.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3oqtljzyp.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3zdksagez.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3bexougwk.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3icxqakfo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ojuoarfe.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt3xuhkxnhu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yfltbeju.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3monstyyx.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3zwnnwmex.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ymuzaxlu.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3mmstapqy.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3huregxym.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3znbsxiby.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3pnpnewnx.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3ydhhfclu.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3pnfdamau.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3fdrihkcx.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3ncccqlwm.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3fnulzknv.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3zzupfntr.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3cituhlwx.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3juxbccqh.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3fjocwfsq.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3kkrbpmhn.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3ogtzrqmr.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3mxeolltr.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3yanikxyf.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3otqkoqgu.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3kscdvanr.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3wwgnzoqd.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3ulaiceey.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3awwibvue.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3aneptlqv.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3yimjramo.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3nbegaowp.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3mkfkovgx.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3qokdolpf.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3argileam.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3kumwqkom.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3ziuhruzs.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3lrbflfhm.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3bjpctpvx.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3gvcsiuir.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3xppbohlm.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3eawplauc.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3nzvsrqgd.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3ardhwsmq.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3umjdqhbb.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3xvrjzray.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3ntaaveqo.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3otfkypre.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3ujizucym.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3lqhkbplz.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3ebftguvm.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3tbtfmbwl.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3idfkrbat.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3vbcqwqly.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3lgxbdmzd.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3tsqffwnd.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3ufstuivv.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3xvhwrscy.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3pnouahbd.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3ujyvfjoz.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3xlacjqkd.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3mnzsczmg.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3wtejjlem.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3pnyeytob.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3ncozrngy.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3ehkaojug.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3iolcponl.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3ghxvssrh.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3pbhkzejw.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3bsetsrkf.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3hmkrtwrj.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3qakqfjku.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3zalmftrl.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3iowvxeor.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3znuqbflc.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3ntuexrng.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3qyjigykt.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3bhkywuqz.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3cuixgznq.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3cnvztygw.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3yzvngmsc.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3tnmdmvvt.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3lohayfcf.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3vszssrea.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3msnwnuaw.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3wwawnpdz.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3ymhcbaki.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3bncpkyob.html


<!-- 参考信息 -->