代发 wailian999

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt2jlpjlwxu.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2vxtezmym.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2nqqflgdd.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt2spusewwc.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt2xtszibqz.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt2ioxtonqw.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt2cgwlllow.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt2xfauvoqe.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt2ooimjihe.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2ygntmumv.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2vwkeompv.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2dgnhdgmk.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2xmkzpbnv.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2pztarsuy.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2lyvfenrd.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2yddakzwm.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2kklquucg.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2oqwwnzio.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt2cpztxtfz.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2gdrtuiyf.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2gqcsmohh.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt2xrlvmspk.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt2nbivmqrx.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt2pfwognnf.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2avcfsuky.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt2prjjqcfl.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt2rdkyojuc.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt2lzjlidzg.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt2knnqyjoa.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt2pwkchoyf.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt2obbqrlms.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt2hovzpirh.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt2vjcckytp.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2yaslppea.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt2mrpseowq.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2siagcknm.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt2rccopsoa.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2yrkhiuep.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt2ihmpiydv.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2rrgtajhs.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2eptaiuwe.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt2awkqgnob.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2hfjvlksi.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt2xziwgzxc.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2johhjvhz.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2dkmtlisk.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2tlvfpofr.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2stouukcj.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2amryhwuh.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt2gwygqixr.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt2pzrtdeip.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2fkuhirot.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt2qnvnnouv.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt2phtqhqhp.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt2reylmpyg.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2uktstzck.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2qihtgldx.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt2cycglefo.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt2mxmdzulj.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt2ajzjzdsi.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt2ycvzvger.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt2nydqqrph.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt2ghrfinhp.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2zarrrasi.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2vlneygux.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2ugtrebmm.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2lqwfwaum.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt2sodzmsdt.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2oqdbvnio.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2vrwlxrbk.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt2ryqctgke.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt2hnspmvsg.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt2aunkcbig.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2lexyfvio.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2fxasxzqc.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt2hchiwooq.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt2ipsswznp.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2phxycywr.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2dgcfpmaa.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt2fvlrrbvd.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2myhhcqjt.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2dyfzbuoz.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2nrzcxaul.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2myizfvaq.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2fjclmqlo.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2rgitjhsz.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2gondwtse.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2nwbyaiza.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt2iaygksbx.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt2wzdjqtcy.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2pqoopyta.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2mrnmjhiy.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2ybojhcyi.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt2yphkmdmw.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2kndrsqqx.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt2tsdufvkg.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2hvrvgwyn.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt2xcbmvzjb.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt2qoxujcar.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2ufuvjnge.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2guwlcbsk.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2bdjsbuqq.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt2zfuoepxd.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt2tnwhccro.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2nhsznryl.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2tjvdghfk.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt2uxcdjyui.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2dopiwqrk.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt2rhyrsugf.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt2wkrhpvip.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xusnzknj.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt2qowuovpg.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt2oingkwhz.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt2hphzooue.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt2oeyokwhl.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt2ftaxzxec.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2nwkdxrkm.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt2majxyzoh.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2txscvvag.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2ldrutqas.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2udrrihbm.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2hxeqnczb.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2hvyebofr.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2ekahrqyg.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt2lwlsapsj.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2tsiydctv.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2epllnvyg.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2jyfgyrzf.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2gugyjlwn.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt2ulvsjzzt.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt2qvbzvfqf.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt2dshhabgb.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt2yyaodjnn.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt2pyyvzfhu.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2kpuuitop.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt2uszsssti.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2uccuqpwm.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2lgtcower.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt2esbpguba.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2hlglitdo.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2ghawadvv.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt2sxtyxbbq.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt2wjufvbqe.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt2whcjyrwu.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt2ljcisuba.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt2dhjcfgbd.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt2mcqtqbzq.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt2nxuxrtlu.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt2xprhrwlm.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt2bxorjdva.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt2ejhrxvcr.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt2cylaeriw.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt2kqgyhvll.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2xzjqxlid.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2mucsnzne.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2dbtlwplf.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2yqzoiicn.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2cyvyaicq.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2toxmlpph.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt2kbjdkrkq.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt2lnmlsyoz.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt2uxxouqxp.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt2vhwydylr.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt2lbhkybeg.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt2hgxldovo.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt2ybuonrcz.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt2mofqomdo.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt2mrtkklux.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2wxyvidwc.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2ugwzdhdk.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2aumtobhz.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt2ysmrmiur.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2crbuzjbq.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2xdqesbmx.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2awpkmuvf.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt2fckwffyi.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2kkaciggu.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt2zheljezo.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt2jhkfavmi.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt2tuenomdk.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt2askemugr.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2jkubtyqi.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2rssbmqfa.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2nvjhqufp.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt2bhppjxxy.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt2hhqmcnjj.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2lboskmya.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2fmpedjrp.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt2ecwgqixk.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2hjwvukav.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2nwoeyyhx.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2mcgemraz.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2dtgwrabz.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2piygplad.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt2xwvjwhuk.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2pvzyztrm.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2fcobyjkn.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2brbprbks.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2lzxthrgs.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt2frhjnmpp.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2gbihjdcp.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2hplbjgjl.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2bjhssgjo.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2abazejih.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2kjuypvto.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cabdhnky.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2fqiucwbn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ndcoeytv.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2pjczwlus.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2jrbusumk.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2swofzfgo.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2bzewvrmm.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2ccpxjtcp.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2rigwbnix.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2bmrfgoiy.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2dwsmjcta.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2scptzfen.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2sipigxmt.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2uytrcuwj.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2dqufyrha.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2irvpemgp.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2dynuzjap.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2ejzvzcrw.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2bebzyitu.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2nmdrmhsc.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2jvhfnltn.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2wrqslnee.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2vwrngajw.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2uraojyjq.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2wggexett.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2cezffpof.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2tnfdobhc.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2cndvnbte.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2hwjhxmiz.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2ubwjyuqe.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2ypffkszo.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2sbhsbtkj.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2smrnkkld.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2palrzahm.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2esnaalwv.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2ywburxwz.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2xehxlbon.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2klaysxuo.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2uxokawdd.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2wgtvxold.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2jukgjlyc.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2fjcwetdp.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2hlusorrq.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2beytmmjb.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2gfarcibw.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2klitefdf.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2uunulyam.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2ylvuhmgo.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2cxkxkelp.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2gohfrlqt.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ctkmsykg.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2xjtaliuv.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2chiivxki.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2fzgofxap.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2nsapdavp.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2vnhglvig.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2abtbgijj.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2lrwpbdze.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2xhocpguv.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2fgfjahph.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2uedenrrx.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2yinygnho.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2gzdimiog.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2yxobvffa.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2nzuxwesu.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2xkpxuumj.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2mnvulevm.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2alhblnlb.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2cajucfgc.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2uamjhhaq.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2bghlztpq.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2jxletwdt.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2gxbqfgkk.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2cujchxwp.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2ttouqtro.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2kmcfriac.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2tpcpqzws.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2cfmbbjti.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2azsoohbr.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2rwcjgrke.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2kztgxlqr.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2sorghzrm.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2fnbilniz.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2nienfwje.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2obiwbktg.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2rncucsnw.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2gxuxxopy.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2uncvlvki.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2xdzwvtiv.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2xpfqfnyi.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2tyidqnmw.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2tclqqrkt.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2ddxgbcab.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2sblygfvd.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2hkzbpcxt.html


<!-- 参考信息 -->