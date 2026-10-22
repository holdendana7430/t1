代发 wailian999

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt2kxvyarvr.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2kwhlsiet.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2awqgxfoi.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt2xzjdtozn.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt2rutcnort.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt2cyssaosj.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt2uoaspkqg.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt2bmijlmgq.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt2hjxixbnc.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2ftuormzx.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2wlpdpjoe.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2wjckogml.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2nlejgbhj.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2yyymuopc.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2gruzpdkj.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2dekhhwfu.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2txhqpgbt.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt2ddpjnjup.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt2xapdkexm.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2npzlfwrn.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2uznwmbza.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt2ofnaptcq.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt2hpcxcpey.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt2gcsvosvt.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt2ctvkkcrq.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt2pkrtlyes.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt2autofvjs.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt2xemqoyrn.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt2bbjdxlvf.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt2ingkcnyp.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt2tdsgeqod.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt2ztsxuthh.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt2ymttrnxm.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2qjcoeced.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt2lwdnmziz.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2qgeqelcc.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt2tewqtxli.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2hymgdcud.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt2vlcfftis.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2lheokxnj.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2egearbwn.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt2hkjvtffq.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2iwntndts.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2hzbnmiqs.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2hnfqtqlp.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2bzzzzzai.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2igxqtkmb.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2hjdunpby.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ccygtnar.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt2kwkqppdl.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt2uhsnsynv.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2xelxpqlw.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt2wqrustis.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt2twrycgol.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt2cuarrguq.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2fmjmsbxy.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2lxuqryxc.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2dtesslyn.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt2yxelqtoy.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt2arsqzgdm.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt2xqbasurk.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt2hjqdcwyw.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt2fdhlunox.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2owvhaugp.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2uymijhgt.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2aahrkijb.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2alnihfkw.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt2eqebukjw.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2dfmmnrsy.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2llfzngzr.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt2gyaststw.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt2rohfhfxh.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt2nlvypwlc.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2avxjqjgl.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2imyceoit.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt2zhdyluas.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt2obrwmpwp.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt2pyrjichs.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2aaczqbfl.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt2jtlkuiik.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2pzwtxeix.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2gdhutplo.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2lutbbxqi.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2cfnnpjij.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2plerzixc.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2vfowtfqs.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2ytrsnyvz.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2jtqcgiim.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt2rubroaxf.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt2kheosxei.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2caehmgvx.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2gbssxdaa.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2ilkdirnf.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt2gxtcfmdt.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2bnkdvzrz.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt2fkzfeyqt.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2gxdjqgrq.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt2srukqfsk.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2aeliysqk.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2bajiqdqh.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2gwzuboan.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2foimqpbe.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt2apsrfeph.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt2qgneinwa.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt2suddowns.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2nnvwbzsu.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt2jfjpvuvo.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt2jbzxzjzk.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt2okpukutq.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2tnaixmbc.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt2hnvbrsgs.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ilgyplht.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt2lnzmgkdr.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt2ftttjbwg.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wvxkelgz.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt2wwcaflln.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2zflvqrjc.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2uhmbhixc.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2aysnblik.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2uivlewue.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2fyiqnqre.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2wzppqzxs.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2takvjkly.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2cvahdxrq.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt2txijymfr.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2vrrhqtet.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2axyxgtdz.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2tgkqfcqg.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2ozneepxw.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt2xwgkpbrb.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt2pjscqnsd.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt2ahgfpigw.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt2onqrbwjd.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt2wiuokvde.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2mmmkgfpk.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt2jsbomcou.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2lknslfav.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2sobooidc.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt2xmcbfwrm.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2vwrldvjv.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2rqtagoic.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt2vjclvenu.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt2tgarghyp.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt2jinmyidh.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt2ezvbdwdc.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt2msoyobzk.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt2ipufrwnd.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt2cnfgyaij.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt2zfrxjgmr.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt2elkdvguz.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt2rdgsrqjh.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt2dzvxovdl.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt2oxzxeiuf.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2cxsbmedp.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2odmklsuv.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2gtjemgid.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2jxbtkdws.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2jqvzpxpx.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2ucitmsah.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt2stdmevcm.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2sgyhmcqc.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt2ucuqivxj.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt2rlhttxgq.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt2tzrsdphp.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt2rlgdyyfe.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2tgtwrgfs.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2rkddluwv.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt2vsoghiom.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2ryhmwwhv.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2njkiitqm.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2uzefdopv.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt2ginasviv.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2wydrsoql.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2riqwpivn.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2cimwqhde.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt2wservsys.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2ykbfvvuo.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt2vqsguere.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt2apemityy.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt2mwevsuns.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt2qfxlsfxu.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2iaiualuk.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2ynukzmdg.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt2qorwkcsk.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt2rnidixkg.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt2zxdhzjxw.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2kclhtuft.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2ghpemury.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2jcunqfhf.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2sptewriz.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2rvlpsnri.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2pdkrraid.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt2wdwnovip.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2fywdkyrc.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2qtprjwmw.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2gsfnnkxg.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2lsiuzrax.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt2ciuhdlkd.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2waecvffr.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2fjckopbz.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2rbajnylz.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2bsevissd.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2qzliibyu.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2ngtxijxr.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2ycunowug.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zqglatyk.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2pjpoximg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cdhzxvey.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2ukydreqa.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2hbkripqs.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2wwigoloo.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2vaycxzfw.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2wxeokdlf.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2vgtkulze.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2ffjuzuxq.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2rcfugldf.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2zjvydoto.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2xadxkgch.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2senswved.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2advrruzr.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2aerrbqax.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2iyoqicpv.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2hafovqii.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2mdvqkfby.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2ljsmmpfy.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2nssqueue.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2lnkaulpr.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2anqaqauc.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2fysjqifx.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2ezeeajue.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2oaxacqmt.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2azlbhjcq.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2qluqnmvl.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2sczilfom.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2qxpdmomq.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2nmafzhpj.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2rxnkkgft.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2nsjjmala.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2zobihdhr.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2sxbubkyr.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2pthwwbfz.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2dndurtpq.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2dfhygyye.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2fcukdfzo.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2dulewnqj.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2mdoqqmnk.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2ajrgnwkm.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2oalqodmm.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2txtnkvjw.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2ijozgkis.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2ozqjshry.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2slumnwqj.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2mifbjqfh.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2dlsbwfmt.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2zkhysvfo.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2rtdkittb.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2olvjroxi.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2fjublcbr.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2oaxlibje.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2lvyvclxa.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2nytqytxp.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2yrymqphk.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2olhogqav.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2dbitwzpp.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2furiklxj.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2iaugiyvu.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2ladjvqkn.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2mzhfnvpf.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2axhqutgc.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2ndzeowbh.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2igpwavui.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2xxiqpvbh.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2tpgtdirl.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2alhwrsim.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2lombyzou.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2nohplsee.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2iwlsbhzk.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2mikbdfyj.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2ikekqbmb.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2gvgysrrs.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2rbtfjmga.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2mnspspgy.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2pkiyxceo.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2qwtgeflj.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2rzsxwvpy.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2kiqbzytx.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2azypxwcc.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2wcwfnlpy.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2kfhvyoyn.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2yqlhqyhc.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2lnrldwfl.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2vjtmwrof.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2ajynajaw.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2jjazalcm.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2llxkhgob.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2knzjgoav.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2yckllkgj.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2psuvezzs.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2ugfowecu.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2ohoqvnmx.html


<!-- 参考信息 -->