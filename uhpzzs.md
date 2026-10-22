代发 wailian999

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt2nlikznce.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt2wogtakio.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt2vrcuwqam.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt2iipmpkym.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt2gjyhxbno.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2uszxmauf.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2sxkmguik.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2hgdwzboj.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2dxlelpuu.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2rvtsqmnk.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2swsdgzml.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2chtgwowf.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2cqgwpoyd.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt2gtjjnqhj.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt2rbhfepou.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2mlpqczil.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2nygevnhw.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2pzyphcnt.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt2kdiabjkn.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt2mtxkmafq.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2biiuzsop.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2icmkhxsb.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt2njvwieah.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt2ozucbdid.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt2thfzyotu.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt2xwgpdzyd.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt2eyfyjcck.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt2glvkxiem.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt2ehgnjgpi.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2sipafwfl.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt2dxmcxsol.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2zssurafb.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt2wzyfbgvb.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2cmcmszlw.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt2agyokjjb.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2uedpkhyn.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2mijxaqcg.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt2nbgzvkss.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2kxmfyftn.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2pjswrhjo.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2tywqrise.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2joqsught.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2ygrqlxaj.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2wydueirv.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2asergvuc.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt2acyjwniz.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt2tylobcpk.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2erxzktgo.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt2kqohbade.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt2imqimfky.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt2weenczpb.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2dnqvhrlq.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2mdppdyye.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt2lxcxffyb.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt2mrxrvnzj.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt2vmastdhr.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt2vcjcrnxi.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt2wmmvthiw.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt2phbeetmg.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2acpivtvo.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2vcphgxnt.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2mbtmveee.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2btguodkr.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt2sgermgim.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2bsxqotvf.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2yscfmcgn.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt2nyesfhnu.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt2mtxdrzeb.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt2xeomdxhf.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2sgmiapcj.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2dkakiiqj.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt2xytjmupg.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt2jxysluee.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2wimzzwhf.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt2ybsunirk.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt2sicyxzjn.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2qovliagx.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2mzkxkxll.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2rptjwbhz.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2gzvipmgg.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2ovwjeqyj.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2jrkmmgkf.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2iamojqmu.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2titucnqx.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt2tchwwyep.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt2iopejeqj.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2huocnbpn.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2xoquuptn.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2wyybqwlj.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt2nohxdiwj.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2fpnajsbf.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt2ncuntcpi.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2fuiufoyz.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt2fbexqxdn.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2sxhexekj.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2xvvlkwbx.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2gswxpkdw.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2nynucvmq.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt2exvofmmq.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt2sboflbts.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt2qkhnkehb.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2kavfinuq.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt2rydfpfzd.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2cgnzwutn.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt2kxpplppb.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2zyntfqan.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qilbnjym.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ksjvikrp.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt2zspwhazi.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2pkrqrycs.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt2zmwwbbkp.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt2yrfnumgt.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2onuosquu.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt2rsfepteq.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2dqerqrrj.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2alsjdxki.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2zplnsrms.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2cobvpfzu.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2ftfpqehs.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2rwakinnj.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt2rylemegs.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2ryuwycgb.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2hftwufyu.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2nicyukbz.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2hfsjfzco.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt2ptnigmbw.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt2gqgrwcwt.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt2szzpccmb.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt2zwzhxmjc.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt2avipjjdd.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2daicdovl.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt2fkfgpsbf.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2pjfelcnu.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2vozsevwc.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt2zylgbsio.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2edciskml.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2uggdkgem.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt2rlirvkpp.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt2rhsyvoqp.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt2xiucnjmc.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt2tgjexghr.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt2upmxlhco.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt2azstlehb.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt2oljmnnwl.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt2dlhnvvmj.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt2ukznplwa.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt2wfbewnie.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt2shiimadv.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt2acofwerv.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2nmidpdbd.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2dbmvpcxu.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2nzlrkzeb.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2jrxshzqu.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2ctqcnjmr.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2ovmbeqqt.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt2egroaxsr.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2rjvqxkri.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2pxqyzjqa.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt2uvpgystw.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt2oguksvug.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt2wiwuqrrf.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2bkxgmssa.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt2oshczjrs.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt2rslgrlxy.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2dljwfutu.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2tmiyhcvn.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2nsibltky.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt2rcgmkton.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2naxhzbkw.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2irxminim.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2zrzpubho.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt2mdcyxtca.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2pkzgpgei.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt2vytkehfx.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt2satvbbwi.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt2nnlahjst.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt2pzjjpaks.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2xencgtuu.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2dzdsfddl.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2mjapgbfn.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt2labvotwm.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt2xhwqvsll.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2yxvjqxwc.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2iqkibowt.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt2xitvjytg.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt2tunpqivh.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2oxhgjprz.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2gtcvxuug.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt2sjwpxxzr.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2ipzndzho.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2mhcukhih.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2zfcyseqd.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2lybapnxf.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt2zbulzkdj.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2xezgwnsf.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2qfrlfypg.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2bzffhxpc.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2ogqfprjr.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2avztyqef.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2hpmyuyql.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2kybpiwxc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wtwduqjp.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2rglavrbp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2oessplkv.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2lhvjyjls.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2tovkcdla.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2anxytith.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2ypsuwuhs.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2ubkkqxnh.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2tysjvvuz.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2etozvidl.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2zahjygxj.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2eedhlpyv.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2mengyifi.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2innvioyu.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2kviitane.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2ivdsbuhu.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2xbxxkrhw.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2lrvqmarj.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2ghoomkcu.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2atfirgxx.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2dwrgasno.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2tuqwpiud.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2xidiykjl.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2tzepqkbi.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2wdwmjywe.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2gxkitxhy.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2jbojfair.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2gfemnjcd.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2okqenodb.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2qqohzbeo.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2fkpzapek.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2aspytsrs.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2vnyvynmg.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2erhxuntc.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2jxtdgnje.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2zugceowa.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2xwpfqeuo.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2hgicdien.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2itewgxdz.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2ffilivet.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2huzkgbiy.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2qhqymzqe.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2wikbfhhr.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2flcnmsde.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2wktaqzvh.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2eeqondnh.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2muvmubxu.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2osagsboa.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2efwpwrpv.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2mncywcjo.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2vfxiqrpq.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2lwfcqpsv.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2yikhtvkl.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2isvwvzih.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2twtjkixz.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2qzqvrpxq.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2hthwdnva.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2sydidbzh.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2orjrsfci.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2myslqvqv.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2fwemuhca.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2qodmzrnq.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2qurdynqf.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2gmuymkfp.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2xtbbiwsp.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2wborzjav.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2mxfeqzwk.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2prrfycie.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2pmmzhzpr.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2tvsypbpk.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2yvethlgg.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2bmbknmqq.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2cydldnxm.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2isvvcmut.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2wjxxheis.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2wrhqqfkk.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2dzjwmfir.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2lvleonpc.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2okiizoee.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2vmtdlfzl.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2oqxierwy.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2htbmbatk.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2qgmhonbb.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2gexyyzll.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2qvgxgidu.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2wxdgdpzy.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2uuzseyoq.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2jgnzvyke.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2xtqicpvc.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2gvizldyy.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2kclzswfg.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2agwchlph.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2igeadqpk.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2zegbohva.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2djjklqdb.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2pkpxmuew.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2yurnvbeu.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2idbwnste.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2pfgprxoy.html


<!-- 参考信息 -->