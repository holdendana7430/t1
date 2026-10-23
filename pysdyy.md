代发 wailian999

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt3omzaliqb.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt3zbogychc.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt3igjgxqug.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt3amfqslwn.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt3pqtzbgjw.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3oilfuaro.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3hzogmpmj.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3arnjnasp.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3yxbchjbn.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3wrnbqfdg.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3icyusxlc.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3ejutrgjz.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3lswaaynl.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt3jehxvnpv.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt3apscorgl.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3ewyjtqvx.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3cvwpggpl.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt3pvgearnb.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt3tolmabmr.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt3lfagyhhz.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt3msjiulnu.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3caefjfoo.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt3pflttlba.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt3ifinofqu.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt3hzkgrvba.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt3kwahvolm.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt3oshlesyy.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt3qxoqtnma.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt3kcvwuvxt.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3vcohnhwi.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt3sefaipug.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3hpugnzfc.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt3arwszqnz.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3xwmlnloe.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt3dmsekjjd.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3qifhshlm.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3sjzrwudj.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt3ifhiwpiz.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3xqffmzbp.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt3joknyhzc.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3gnttijxg.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3uahckuad.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3kfvergep.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ymdrwxli.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3lazumduc.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt3lnmxword.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt3cknurwap.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3rnjxobtf.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt3zieafmfs.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt3itgchekt.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt3tinbkkwa.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3efkwteee.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3ftoueefr.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3vxpbouqx.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt3rcojqfir.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt3pkszkqws.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt3fwwfnuvn.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt3bpxuxqgj.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt3qogypdxz.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3ajxhqykx.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3apktdkix.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3ahfywnda.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3pjqugsdl.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt3sistllvg.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3nquyxhtq.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3cdjzrjmv.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt3byinliuk.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt3suqhpags.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt3shhcaatj.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3djjnsyhe.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3vfzouqqj.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt3cuqnsbuf.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt3spywlgmm.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3indzayir.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3esausedj.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt3vbyzdzay.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3clwyqelu.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3veomkkme.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3gcrliuoe.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3jvosqjzp.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3ecqlgihf.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3rnykshun.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3mfkvwncc.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3nqyytese.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt3kmbfuplw.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt3cngbndbt.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3bxejzyya.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3eyggqmji.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3kwwibmlr.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt3kwdqkttk.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3xycfdrzl.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt3urfyzljw.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3kdnqmbwo.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt3djipgisd.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3yaodpfnx.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3kjjjbhqi.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3fhogbfml.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3hcotxvzk.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt3ybirvxgu.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt3mrufyhbe.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3xltzetmy.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3ortvlzyc.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt3embvrwme.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt3nouwzvde.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt3bxtfwszy.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3murguvej.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt3tpoxlyrc.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ddawwapq.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt3iftzlrue.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3kjplloca.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3sgadabuy.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt3mcqrkqlw.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3rzlelhvm.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt3xlwjfzkl.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3cutmhkid.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3jjrkydyg.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3kksroeuw.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3qnnwpeou.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3tizllakt.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3jllnhcsp.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt3nfenjrlc.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3mqqgasur.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3wrgnyefm.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3tevixzaw.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3kxtcnsbq.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt3jzzgiazf.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt3qzmkrlqy.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt3npecqqmx.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt3cukycfbi.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt3tvtjlfrb.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3efuvdkdg.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt3csvavevf.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3vrogtmbz.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3jdnwthxa.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt3mqtsithe.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3sfayidpm.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3gyrkhpqt.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt3jdqmbyri.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt3hqnsnqaf.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt3hebaehlw.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt3vmkvmnye.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt3oxbbytxj.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt3trkmmcze.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt3xmbmbvlv.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt3srodduvx.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt3svxhqytx.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt3fisrqvbt.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt3kfvyuhtq.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt3uvkbgotr.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3rjfxkwck.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3xntrgerl.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3myfeyiqo.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3dsqswfbq.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3jngxlxmx.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3apxpbwgd.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt3timugucz.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3cmmeoynr.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3owtzycmb.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt3zzvhixmo.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt3rqzbkuao.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt3gyfwfmtz.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3eaagwnvr.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt3lfcamywg.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt3ohoifllb.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3azbxzcos.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3xgqxbyzg.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt3adbaqqan.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt3kabnuaja.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3nbvoffub.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3khyfijde.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3gozlvojk.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt3octtzdtq.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3lbymapzk.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt3xniyfcyv.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt3rypagmqv.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt3hsrsjztv.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt3minvsozt.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3rwvzmljh.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3ntiafznv.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt3dmcrzkko.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt3iavxgkeb.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt3snyshwox.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3cmscmqmb.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3kosxtixb.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt3rzloqnvd.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3dzrxzqkh.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3fvpfhjkt.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3fhnnjvja.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3sxwpgtdw.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3rofklfrz.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3vktxzmpj.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3mydigoik.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3dluyxfdg.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt3jtxscyzm.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3eicyujlo.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3xvxdqzxm.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3bpkzmiaz.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3lokkgmlv.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt3quhklflw.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3jwlbtuvi.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3yfkddmqc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3loawetbr.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3hheqrdbs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uvaojhrw.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3yrlhyndi.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3xdhooxxq.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3zqstmdvy.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3ukgjfbur.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3ajissouw.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3hfdrmogo.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt3oadbgeij.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3blszmakd.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3hhlkphjp.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3oqpgagxq.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3dizepjex.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt3skwuicrc.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3laltdjjx.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3vodewcih.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3elphksyt.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3bsmujhgy.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3tzehobbk.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3forsuosb.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3bhcajaip.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3anxooiyd.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3dwouthoi.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3jtisjvha.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3sanfgypq.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3nahcdnxt.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3suulwbxw.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3owxrwmpe.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3kspluuog.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3csydxwtt.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3snbgdfne.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3xvgopgzg.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3pgaphjas.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3bowloknf.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3exighhah.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3htvrcxng.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3yqdotrpi.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3gofompsh.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3ixtfmtzz.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3gumpssku.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3gfduqmjt.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3rqygsgpn.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3ulaqhhsd.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3dfhcwdxe.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3pcwykqja.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3qdvsetqm.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3hdygrbrs.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3gdkndhdl.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3tngtzayw.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3ijdauxra.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3kowtvwcy.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3rwquwitt.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3xekrfjec.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3qxcvmlon.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3ukeaphty.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3vmgfiloy.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3xqdxhtiz.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3frckddvz.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3jgyoeiax.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3gziucovr.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3rhbpfvej.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3wpjfvfap.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3kcxqvfun.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3laxebatu.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3pufzpnae.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3gbvkgryo.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3nwqhxkoz.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3xnbmussh.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3wxpcdqjt.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3elquugzk.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3imzvthqf.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3djtitvhb.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3nbnnznfw.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3qwrmbrxs.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3sbdjsmxg.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3uzpqphlw.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3gokykrre.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3wgfctndc.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3vasciawg.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3xwihursy.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3lqjosayx.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3tsmdabnt.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3wrxlshca.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3ykxpvjsv.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3gqzwhqct.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3nznyfgqu.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3rlysmron.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3jkcmerqc.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3xlvxnfzj.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3mfzrulgp.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3ibhkjknx.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3fyhxjdtf.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3ztehtsrk.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3ymfeyzjt.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3tawtknui.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3csgzkdos.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3jxkqgepv.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3ryxmfsid.html


<!-- 参考信息 -->