代发 wailian999

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2fjpslekm.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2ublywkto.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2lhlybcla.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2axmlkkqm.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2hnxkicsz.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2htgcastv.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2awuejnss.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt2vsqdygxn.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt2lilwzbly.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2jpfjobiw.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2jiqxjzyh.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt2klatpjqm.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt2yrmiwtbe.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt2yhloexju.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt2psjkbdrg.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt2gomqedjh.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt2wflwgdrl.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2xvdfbogw.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2umlipcsf.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2hkvcfgfm.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2cwmvvtjz.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2yqeshsou.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2bzenlyqi.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2hbayqewa.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2rgxxdnhz.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt2tciajtay.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt2bdfbxesq.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2vnukcrwz.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2lwackapq.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt2nyibsgel.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt2bmmobvfw.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt2gvmolmuo.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt2xaqgayse.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2datntrsv.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt2ewkaxqtm.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt2mopuyktz.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt2agrlwcea.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt2jymynvba.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt2ahtfhrfs.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt2arzyvwnz.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt2ookpmtcl.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2kgwdhoow.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt2mooyvyts.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2iqgbjpjt.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt2dudraknf.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2nyewalxj.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt2pocchsmh.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2mpyhengt.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2ebdhqspb.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt2xqddukrp.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2ojolitix.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2xytoswdc.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ioqbqtzj.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2qrcxsxcj.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2crbgmvqz.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2vghjpzwk.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2enijrvbh.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt2uebbulbg.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt2ptblfutc.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2fmghcgpo.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt2jnwdckxn.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt2uhdbrmwy.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt2hfcojvdf.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2mhegttzp.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2xrpvdksx.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2xfepyqau.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt2aywwawgx.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt2kyhlyxcq.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt2nknafwlu.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt2rzksgonh.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt2ocmkwztt.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2yrqwimtr.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2fqibqfff.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2wnrukuep.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2srvptujp.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt2zgglppsf.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2lzwagihq.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2knsooaqq.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt2ozhwurra.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt2htchfsez.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt2aoystwch.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2icfoafns.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2rnctffic.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt2vjanxlgz.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt2upmniyks.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2oskuslcp.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2suzjbemu.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt2vvwudxpe.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2wwrrslqr.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2oydgxuqy.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2spnqiaxm.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2jzetncqx.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2mltcdmjv.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2kefihyqe.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2gerewlth.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2owzimdqr.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt2yoxjxyqf.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt2mnswlvas.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2jsnarwza.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2cfrojknp.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2bkemlwec.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt2ijaqxgdj.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2yliqvibg.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt2dgqkjtzj.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2gnllepca.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt2tlbrofqo.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2hyylvpfl.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2lsbhevbp.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2qzfxfwcf.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2lcecbyzc.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt2lvytmswc.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt2sixryabz.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2nsispecy.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2tjfqhpbn.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt2emxkhcpn.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2hgoaywdl.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt2uvkalrgy.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt2xlbzhtoe.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wvwxayjg.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2dcelmrtb.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt2fpanvuww.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2kwokfcgq.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2npfloart.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt2ezqsdzmd.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2nvgdeouu.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2zsrdcqwo.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2wzwvxyvj.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2xdpuqrpx.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2qnvaimmj.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2trkqgcdi.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2uivnujwi.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2khyvvdzf.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt2xowgrxhu.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2tszwilaa.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2zoudimqv.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2kzfzdsdc.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2rltmbcty.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt2sncedzfb.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt2mgmszsyu.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt2foiwmhyx.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt2qeiwmfcz.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt2ozpekyvm.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2zffdtvfq.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt2qbrfoani.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2geskcigp.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2axpyxtil.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt2clydncna.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2ajzcwobr.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2fhrxrkpd.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt2fgruhdjq.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt2ecuvkbyb.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt2djojmodd.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt2dxmqyrrw.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt2qlcjuqfh.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt2kumafccz.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt2ttfepjmi.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt2rwxlibfs.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt2ygrfcikd.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt2nyjfwzzo.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt2hkvaqnmu.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt2nhxkenbp.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2rzhlncli.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2wpbrxmkj.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2voifznix.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2xtgeeuvp.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2sdizjdgl.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2bjjxpchk.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt2jmgxfzqg.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt2ixjgerkv.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt2mrrwgexc.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt2rvbwjpfj.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt2uppmhwlb.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt2sjblcfou.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt2mgkvdybt.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2mzgcpcxn.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt2xrropojw.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2isdbjmqs.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2mjedythj.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2xhewoyxo.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt2soiczouo.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2tropsmja.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2wiccvwqb.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2uzqhmdue.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt2ggtnxprm.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2wbajqecq.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt2hxmcltml.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt2mxmwybax.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt2qktimcot.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt2onsfexpd.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2roluyzwg.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2qpksyuui.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt2wbonoygh.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt2lswpjbpo.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt2jllvqrua.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2qxhrqcby.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2korscskf.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt2njmklvgz.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt2wfzuedgg.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2heunwwjr.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2vivvxrsi.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt2ackzpfew.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2acnjdxqw.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt2yzrgzaqh.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2zptmhezk.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2yikfsuyw.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt2griphqti.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2lceyaush.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2gnosfvye.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2mwpyisic.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2suborpqr.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2ivlwmwed.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2hsukxtyn.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2tzanlgqo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ftnbwwue.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2vkoszsib.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nkvdhgeb.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2mqnvgulr.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2gayviuuh.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2wkhozktu.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2blohinyd.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2pjowfcir.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2klwbouuc.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2pmqwspoo.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2zxmoqtaj.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2olvalzxo.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2apgfzyjm.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2mjqmdkli.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2hydgwvhx.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2tqqsoejc.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2iuwdcwuz.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2foxiyolc.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2edixaqaf.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2mnoyaska.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2ztbehtuh.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2ejspzowh.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2qvdeqbvn.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2qiqzrrvv.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2wffrphjd.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2xmwkiote.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2nnplmfeg.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2fcwgzowi.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2wevdciul.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2xrsthlzq.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2zfdmrcxb.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2qoxgpiye.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2cbxskvwu.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2llncqdpz.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2pvhiljhx.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2nlgqyeos.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2temhpglg.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2ombzqwhb.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2rervkrst.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2ijvlcybg.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2uogwudzm.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2famzizoo.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2dvkeryxy.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2gilbstes.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2epikukjg.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2gqqdrfvn.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2uovqsngf.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2ywnfdvlh.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2zcnjrslk.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2atsdrtrk.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2pvhfmgju.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2ggpiealt.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2bbhalsjb.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2yyjdwqdy.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2kjlbpwhm.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2ejtrfpng.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2usujhfyj.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2ktujxjfc.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2zikfsqpi.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2yzxumkal.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2znducrny.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2eqbjxbmw.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2srksduiu.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2othuzesw.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2gchcfdhz.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2lvsnhnsg.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2qtfhthvw.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2zspcuadv.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2qdivtsrc.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2rvqaabwl.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2dqrssqcm.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2qyrgxiwo.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2ltjqmaph.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2xwytfhag.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2sbgidozi.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2xenqwpas.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2jkuhfcek.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2pecigjxd.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2mdcdgiol.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2ocyyspna.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2lcqtvbjq.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2leadyzff.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2rxknkmoc.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2mnbuazvm.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2msyyeeya.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2vhyqrndi.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2pvcoduqp.html


<!-- 参考信息 -->