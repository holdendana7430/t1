代发 wailian999

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3zgdyzobq.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3lyxantwu.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt3cpjqrtoa.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt3rapvpkui.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3feaqpepc.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt3pustpwpp.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt3iwpzuxhi.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3ybhrqpvo.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3biczmpbj.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3hfuqoiuh.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3myrnetrb.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3xfoloctp.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3gdyldprt.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3nsdpifck.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt3vgtzxmqy.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt3mguuuzff.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt3wwugcmfp.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3ldkpgvii.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3oxiompjd.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt3zauxkify.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt3avyfftkl.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt3lhlhiakx.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt3htlspvzz.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt3roenieph.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt3vvfvenqb.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3ybdjzioa.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3xvsbhcsp.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3ktblpltl.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3vhypepam.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3kcbyjcxb.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3uuxnjwvh.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3zwqeufcq.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3uzlpeijt.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3ojevvopl.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt3gjjdtcew.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3rfqpczga.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3dpvwxoao.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt3bttpahxp.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt3ossstzwn.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt3jgzdwehd.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3fyvnwooo.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt3wxfafzqk.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt3hnerhlvs.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt3bxfwbrqb.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt3fwfcgebo.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt3kfemgltd.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt3zextnyaf.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt3tqevmvco.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt3gfhgabea.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3mldsechc.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt3afhigamy.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3kskymtnl.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt3dludzrgz.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3bsfxzwet.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt3pnxybasv.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3ipyyppss.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3sufyioeo.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt3pwmdtgme.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3wqdjuuaa.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3uufsaimr.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3nvllhpgk.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3qrwvonzo.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3gfxhvsgf.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3jmvghqvk.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3qbvcslqe.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt3klheemmu.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt3mpbxeszi.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3mlhixhzz.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt3itgmfjsf.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt3iwdmfccy.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt3rgdprzso.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3fcuokbbm.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3ebhcbypt.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3xrovtnvi.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt3eijyiguw.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt3mlzcyjke.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt3fjugyzfk.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt3eknlxrcl.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt3nokilsoh.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3amltnipg.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3dfyhgpuj.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3daacujlj.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3bzsooaor.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt3vhuydszx.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3sktnqeob.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3tsniulap.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt3fijnugvq.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt3sffbsooz.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt3rilkjzeg.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3beoiuekv.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3xoboifsm.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt3lfpyzuat.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt3nhzfkxkm.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt3ofzdvhbc.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3scbezpqm.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt3zwjekrtx.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3vtgeafsb.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3msbbivbc.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3rhgbanzz.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3rumzprua.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3pibninoh.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3qsqadqlk.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3ixzlikbn.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3sjeivbaw.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt3ifibzxne.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt3ifnzjagw.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3yfkdgjsb.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3jxzktkkd.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3usltugst.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt3jnsqpohn.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3fephggdt.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt3zduwfuwy.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3tknnogmc.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt3zapwfdwb.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3voyordqj.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3komcyzxx.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3lrnwlqas.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3pildqbws.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt3vzwtugzk.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt3mbmfpvnf.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt3wopywiqp.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3pplqkfvh.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt3bnddttsz.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt3ruadknvu.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt3nfyudvss.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3xfngyykj.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt3dejzobqr.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt3fkozyobz.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt3isclfscv.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3ewyaoefg.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qckrnldp.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt3srcozoyk.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3zkuxeknm.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3ebzywogd.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3mfqrqour.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3qycyodsj.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3gckahnuy.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3pumbnzev.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3ndvaehkn.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3dnjxbvjs.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt3tkzsutgt.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3oyolukkd.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3ydqptatt.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3wbdmdyyx.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3grqsllbf.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt3ekcnxvhf.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt3swqwunof.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt3pdxzodsm.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt3thsmzmad.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt3crzgujxq.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3gzbmxace.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt3ijagkpdl.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3xgscvsdi.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3xutzmbhx.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt3ytdxsbvy.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3kmgcyycs.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3zqxmbfmt.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt3qwnjrzin.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt3myngkojt.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt3oetbctpd.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt3ezwjqjzz.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt3qipahjnr.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt3xnqmywql.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt3jvbpligb.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt3pentvtjf.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt3gjvoiwac.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt3jbqjzsvp.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt3vgqdbchh.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt3pjxeocvz.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3tsuumzzm.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3tjbzoiqb.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3lhgmseml.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3vhqzixby.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3ujbfrebe.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3dphqdzcl.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt3cdlfihdk.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3exqvzwqo.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt3pygatrfw.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt3joxxyvbi.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt3frpgssdi.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt3oimsucil.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt3oreqdgqk.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3dvcrrvzt.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt3kxbqdgex.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt3eqbckiib.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3ojjcqjfk.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt3ggbqtjfe.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt3neixlfai.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3zykgearf.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3unxcfdxe.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3qviifvss.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ctzcjvgz.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3piqtadxi.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt3cjswutsc.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt3debwojeq.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt3cgzmvdoj.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt3jywqeygw.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3yrtbqnig.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3qzrefrla.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt3ypyokxpa.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt3pqrsniuz.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt3iscwxgia.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3nooisxge.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3cldsbhgt.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt3mrwnvuec.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt3spwsobim.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3abhhdccn.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3iwkyftlq.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt3dzaxgsur.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3sgxryjsk.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3joiiebfl.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3aqpmobde.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3nqjrxeij.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3yulxzita.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3iaxpiakw.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt3wahhpdre.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3tiaqilps.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3gikfdrlt.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3dfnbqmav.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3jfcwudyw.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3jtczxvaa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lftzdiyi.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3efmtyjse.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3spnpchdr.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3hhodvyve.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3vjaimiss.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3besarbwc.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3dpwzmtqf.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3cxvnuqly.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3hqqnlxvj.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt3uyepgtfa.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3twxnuxqq.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3lpujrpce.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3bojeynfz.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3ewyggnhw.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt3ptypybfw.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3hedooikl.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3kxxszsvh.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3lpnmnuhu.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3fmmypwbh.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3mcaiyexr.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3agpwvjdi.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3yhrqsqif.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3hwaxzbhh.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3evwvagks.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3qjvaffsh.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3hxrjztix.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3pxolhzqn.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3nyycsoxf.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3hbudkaiu.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3rxlubmwr.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3xxaafscr.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3ltbtmuul.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3tsjcycms.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3rkmibvzh.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3xacwidts.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3bypcflia.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3qqwspvbe.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3kvcegwzz.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3zdpjspdz.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3excablax.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3sfpucosi.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3jwrmtkzm.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3qilfrkfw.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3pqmysmnj.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3zdctcjkg.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3wvwhmmdo.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3dznyrkgn.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3yjnhqfyi.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3hwaezjfw.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3tbixubiv.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3srmuwyni.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3iwrefdez.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3umrrzvja.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3ffrcmtsh.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3rndmfmrr.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3wznakjig.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3effnpynz.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3mpnupejw.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3vcjqlkik.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3ypxkzuru.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3kjtziact.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3zfglxlgl.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3eamvlbrk.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3eimkvgsd.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3ihldxhrt.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3etnknnvv.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3ilhvsebl.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3ptzajjrk.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3qdqhbivu.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3oyflpjqy.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3vwsgrrwj.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3hfionaad.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3tywmokdk.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3gpphfdso.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3pzljrlfj.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3albfcsiq.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3fqdiasth.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3rfxvxdtc.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3twnrxaat.html


<!-- 参考信息 -->