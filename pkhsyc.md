代发 wailian999

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt3nsfiqcdt.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3qokrcvoh.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3zechwxja.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt3rvhmgijw.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt3wnghwptn.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt3hmypegdq.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt3wtzoovyc.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt3ikiuwqrk.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt3duxsgejf.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3zyxmsnva.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3iqyyyuwu.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3fjhjkzve.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3hosjedfo.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3rkaakrcy.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3olkseyut.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3imewjujq.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3tqurrcvv.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3yladtvnt.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt3qgcapgwq.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3mifwltby.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3kxjyaobp.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3rhcwcgnm.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt3kjbkcvlf.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt3sahbtvph.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3krznrnzy.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt3imlztfdl.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt3usnmtvmy.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt3kqjfjnfp.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt3casdihcf.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt3fdfooowo.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt3nvwdtjxd.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt3vtayqlmo.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt3qekxvuhj.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3dqbnoffd.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt3mcfogaxs.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3xanudcql.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt3ntczkumr.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3xogisnxv.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt3ocfxwuyl.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3ljsucoft.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3ussxhbsu.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt3jsyuqjkh.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3pqrnuszl.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3vmjfggbf.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3pfuydlyk.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3kiuhnkso.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3jryzqswc.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ooayuzvr.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3wzqxovgv.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt3etivczfm.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt3ykfjolpf.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3spjazzbm.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt3gzewxdtm.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt3yanqvdvv.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt3ilnqhluo.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3wshnxiwi.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3auondbbz.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3xqtlizwq.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt3dhjvfnnb.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt3eygayjdv.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt3zenitmet.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt3zverxxcy.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt3bzzkiwwp.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3xxsowbeu.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3pgfqmiui.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3cbtjoxoc.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3tmrpwgkj.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt3zaxsjwzf.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3uqizqbyc.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3hyqlhgcb.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt3vwxbewub.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt3qqpoldrv.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt3joauoemr.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3xgigzdtd.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3twrcbbkx.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt3pdqbmmek.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt3kuxnsito.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt3qzfodttj.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3yvejfmpp.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt3sqrvfvpw.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3mmnetsac.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3uvdcotnf.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3rtvjfxcq.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3ymqglbhg.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3cvztxjib.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3coktquxf.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3pleulxlb.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3hpselfpz.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt3belmecna.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt3dqqtopxc.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3jayeyyzp.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3ipoxvawx.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3ijdiavjn.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt3vybblvvh.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3pdpduueg.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt3lsowythq.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3ffqkwlug.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt3dbukspkl.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3gvoenihe.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3uskksvfq.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3hucngzju.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3lhdykrzn.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt3nydgrsuy.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt3qskdooop.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3riadygvr.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3wbvmiehk.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt3adkjmomv.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt3ztgfmhtd.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt3ptehaeqj.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt3pwhdzkhv.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt3bnmiatkz.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt3harfznhi.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt3nkztvlpp.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3pkljclsk.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt3aqgjnfpo.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt3bhkhbmsx.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3klznjwxt.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt3ncivvizt.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3yydkckdy.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3sdnueitf.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3gzggxnyn.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3rahxkpvt.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3ryxhvrdr.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3rhbvpunl.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt3yxebgutv.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3oahofejs.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3nfmzompy.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3wducoetu.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3diznvlyd.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt3xemzczvu.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt3mpynivym.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt3fxpzkbmz.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt3kjvtqzqd.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt3yakxebtu.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3rjniaccu.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt3fllxijmc.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3riextzyf.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3vcoulqtz.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt3yepapdgn.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3qoknqhqp.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3lqbhkhym.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt3rvcucioe.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt3kiwxonsy.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt3iwqkfjks.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt3jfubspqx.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt3kcyglqxg.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt3govyrpki.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt3gjkccgki.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt3wecpohme.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt3eapmalkl.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt3kjaozjat.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt3kcbkjjvt.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt3ejuuhnji.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3qgzysyew.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3tgwggovj.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3wekpsfvd.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3hhwhjxzr.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3kdpsnawh.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3peupouej.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt3dvraizco.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3chnfxppi.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ccrttnbd.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt3gcvrkoux.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt3jvtixrek.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt3bpojvnnj.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3xvsydayl.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3awwneeko.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt3qqmaoybp.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3awyylyfi.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3tpkcesmc.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt3amxpsytw.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt3wzwgnwev.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3osiijkbl.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3sjegdcsx.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3mfrjohuf.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt3noeukedz.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3wctkmylt.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt3dmkjayqc.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt3zehhguaw.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt3xvbhbdye.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt3jjmkajup.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3osqzclzx.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3ptmobesd.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt3uebqaoce.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt3xwsdciil.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt3knsdoxyo.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3sceqvhhm.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3yhbqmxkp.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt3acymrugj.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3tiofavjh.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3anqhvebf.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3fmfqtmiz.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt3tmejczsd.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3hyczbepw.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt3czwzweom.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3vcnbvegl.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3pyztitak.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3luseaocl.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt3ckxcwmes.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3impuffhl.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3fzhvkauh.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3zniwster.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt3nbfphllm.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3ttttaoyz.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3fmfxkgog.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cjzzrcsl.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3ilkscvxa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qrpdloph.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3qvmersmu.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3rqrgihya.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3ndmdcpui.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3tfhgxkwr.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3tieyqvpx.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3eicbjopw.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3uecripts.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3pwxuhake.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3qoaxcldv.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3kdrlxokh.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3xhabjxck.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt3rhxbdqhl.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3zzqnmcdd.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3ayyyosrf.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3htaeoqpr.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3fvprslfz.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3yxisafnl.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3vjcpglsl.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3nndmqeua.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3vviiwnnv.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3cybfcpim.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3nyzydkvq.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3khxlnswc.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3fsgvifqu.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3noimzifg.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3svsxnwnp.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3bykebqbp.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3eylkkyaa.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3tkopqcsa.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3mpcjdyhe.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3czwlcdon.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3emhgtyjq.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3eqmzeazy.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3kohapfim.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3segfpzkp.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3nvjdhwtp.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3bsxtviqf.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3yjqyaejp.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3gldoyzxp.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3fvyjcsrl.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3dfaudlau.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3vjkidcay.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3rzdcnynz.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3wmzcxiqx.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3mcpvdaxo.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3ymmkosuw.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3slfzxkqi.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3srvegmzf.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3htflljfx.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3cjxwiqzz.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3lqlprcrz.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3mvdclyjl.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3jrhidmfb.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3hepyzqym.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3mxyvaxfq.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3lhwglvhq.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3efnjpgud.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3zjgxsuca.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3nfbreyle.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3ibaiktjv.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3lecjbezs.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3pjcqhiym.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3zwghoafs.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3oipejbed.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3xjlgqoof.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3viewrnyh.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3otxztjln.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3lybhgvza.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3nbafztcg.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3utjknxkc.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3limpbkbj.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3wibfjvtn.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3gxwrqhiv.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3gxqzqsok.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3ydjohvyu.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3jgdzfxxc.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3iifcuoao.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3uoiaimlq.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3oeqrrtio.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3atztliuu.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3vfnuhdzu.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3szzljuor.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3nzuhdziq.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3enjqhvaa.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3pdnmwhtm.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3htenozta.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3wxvegkep.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3jrsvepej.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3seofmfyv.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3veywxlxy.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3qbphensi.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3mynakfpj.html


<!-- 参考信息 -->