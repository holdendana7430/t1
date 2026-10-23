代发 wailian999

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt3dzubvgoa.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3xgbxrfhm.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3owqfhyvs.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3aqzvjgqp.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3cehxmbeg.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3eboqmrie.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3geqcfkrq.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3fxsmdhgh.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3ababhelt.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt3dooyfcfd.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt3uwnnuhmv.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3lwbuptyh.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3igajxmua.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt3tcylvbyv.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt3mambmzne.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt3hiracrrm.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt3aakxbtod.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3pghaerdb.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt3eudmseiy.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt3ivdmuzjh.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt3qnwepdfx.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt3hhavgwsf.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt3hwvxwfdt.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt3qxdftlcg.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt3vasymlwx.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3vufrszvi.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt3ajkbzcss.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3vkzhmkjt.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt3oefdevil.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3mdsbpjzc.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt3mmigufzx.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3saognwjh.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3sgcilgei.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt3ubnhjpaq.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3zvhwwinr.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3aiukqcgi.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3exaielyt.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ynajimtn.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3ycwaoqdk.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3yleucnce.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3qkzbkypk.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt3onxtcfla.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt3xpxxumed.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3ffnjfgcs.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt3tjjdymme.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt3yzbqoejo.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt3dukosdyj.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3rxvvysat.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3isibpeni.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3zzjtnrkr.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt3fwmqnkqp.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt3qgrgxhca.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt3dmrwaonf.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt3wzkdobkf.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt3pvsjjfpa.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3hxqmcatp.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3geurtarm.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3hyvxkgpw.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3jkvbfksi.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt3kvjkpyvg.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3jdduiddx.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3eqtgdbce.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt3zktverik.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt3saxpojce.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt3rnfvcfot.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3lbnooxli.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3izgtkcvw.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt3tdsbjnyx.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt3xmfjuivb.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt3gjizklal.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3enuptnoo.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt3bzvysamu.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3hvziivqe.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3wevkjgne.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3wsjcqvtt.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3oftxanhl.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3rnfjoofy.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3jedjszrf.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3zqyifxrl.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3fhkjsmro.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt3kwrwvvmp.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt3faqmbvbi.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3hhfskoxb.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3jmezaqus.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3xtiqawrz.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt3cxqovodc.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3ljlvipeu.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt3zbjhuolc.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3sqpzhgpg.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt3etbcrqrv.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt3lhbbpvrx.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3xjghakhj.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3usxnwtjw.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3huykyfax.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt3hlfcvuhc.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt3jblsdaqo.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3jwrbkeim.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3yapkmpcs.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt3dmwwulbf.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt3cpeedhyy.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt3hsmzmoed.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3bsgdibjj.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt3xtnnxmdf.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3bivxdzlt.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt3kfyqgslc.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt3dzrobtdq.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lrdyzzxi.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt3poyztsqc.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3wrjczuoj.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt3vwlkqmtd.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3leewfybr.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3sjkuuapq.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3qnpthnfi.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3xjkzhikl.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3nrsbawdo.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3fbidovwp.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt3vwtudhzh.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3aizcmnfx.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3rncknxbu.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3iwshqahq.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3serhcrof.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt3qwyshedp.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt3pfyblrxi.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt3lpburrjy.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt3mpgxcydf.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt3lxgrktzb.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3jhvyjrtx.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt3hyenkikb.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3ocxgqpjf.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3ztwgiiwj.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt3ikngjhxc.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3gyzmhrdl.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3czmjgpzj.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt3dvpvacey.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt3easdywyi.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt3muxnamgz.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt3vhigrvab.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt3ypagwegi.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt3adpruylm.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt3ivvpsfhn.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt3mbxipyce.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt3bijdokvl.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt3idfxtjri.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt3iqfwtrym.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt3zfqeckpv.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3tuvckvmz.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3hxeujpei.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3ljwlmone.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3gwqokcci.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3lgrnlgrt.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3vmjkcgnv.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt3orsjehig.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3rexdisld.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ltwowgjj.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt3ccjtmvad.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt3ckrvcnuk.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt3uzaaxbxe.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt3xjsfztiw.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3prxewjje.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt3yyarpzop.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt3taarbihr.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3myvtorpm.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt3pyvfwcxz.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt3iakoiqlt.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3hffeurqb.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3jjisgthi.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3dttchnij.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt3pvwracrb.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3tccuudss.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt3apgsiklu.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt3ojulmmkd.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt3mbenjbml.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt3yxiwkfeb.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3ygxitaow.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3eizdjkod.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt3tdnwpnfy.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt3zybniidp.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt3uyhfjefs.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3uldjrstg.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3rukbbtny.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt3fwrfqbjd.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3grdorcho.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3vjxkkfpy.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3dyhdqzcw.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt3klsjdoet.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3rxidltoa.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3adpdnwpz.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3joeddhpa.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3zakrtvyi.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt3suxjtkfw.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt3cwiylssu.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3knigswrm.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3dtdrcdol.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3sdkeyboj.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3gcfzsjjx.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt3ocgcsspt.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3vhpngbsu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3oxvmhakl.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3lzdndkth.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ivwquexk.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3ztqohuqd.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3lrfbbbwe.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3sjrjhzaa.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3ocoljjpe.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3hxzbmuci.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3vrlbtana.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3agzlyufj.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3axkmyyyc.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3cxozrycm.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3kpgcawjv.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3fdgltuqx.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ptzmixrh.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3pslvjpjm.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3nvwvhoie.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3hqdkjxpa.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3gwcecejf.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3deddatsm.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3yvemxtvz.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3bfgsxpul.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3dijmzyjp.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ctetzkmv.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3mwuszyne.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3msueaewh.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3yftkeivp.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3cctolbdz.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3nzjbuwup.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3yxxaytzo.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3gndlshjs.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3mdwaekun.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3eyurussr.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3uolpgdcr.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3ewrxmoeh.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3kbucsmbw.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3skoqadbe.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3zockxuou.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3yqzriyjk.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3omkytyar.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3vqudoann.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3amhwizqr.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3bpmegded.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3sjtdwhlr.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3mtyfogkq.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3xgjpivdg.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3fijmjwog.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3zrcghhgb.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3empcehuv.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3pnghvbwc.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3pghgiaox.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3ybbtbasy.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3sbkqbgvz.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3ohbuycqa.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3kyphwqyc.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3aonpuqnd.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3hihinvoq.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3ftqxrizc.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3nrccyprf.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3wzkdkjhw.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3dzgqkjnx.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3nchfgrpg.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3xqjugxjt.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3acjcmoxc.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3wknasiao.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3wgqgwpij.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3zrdngiad.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3jrgxfbim.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3zocnapav.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3pterowvu.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3yuggzcjo.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3vrajxmac.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3jujdscha.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3wjxpjrdq.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3djeesjcs.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3qzbvwbfg.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3qswjybhp.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3givtywgu.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3udzahyxc.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3onvjvgem.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3bclxbdan.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3gazbrcfa.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3udshlbuw.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3rdqpgvhy.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3cgdakcpa.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3bsauyffa.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3jykpymui.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3fanpwycw.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3gijmmyks.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3irrehyrx.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3mlnsdupx.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3wvsaqhzy.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3nrlbviqm.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3bwfkhjza.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3folgaril.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3vodgaylb.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3xbsiiybr.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3ggsscdno.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3tiwromaf.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3qjezfesp.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3jiafvthr.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3jkgtjfqs.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3xmufqwlz.html


<!-- 参考信息 -->