代发 wailian999

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt2rgfucfwu.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2sklggeda.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2mjakizad.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt2tzshobiz.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt2glsppate.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt2yhfeanue.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt2ggbvojjg.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt2waumfepp.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt2vqyqsdvn.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2pbiruwcp.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2njbdmubg.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2fhbeeiix.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2yecphpvs.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2nzztajjd.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2kdjyuhxp.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2zzbjhjxu.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2azbmwybe.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2ydszxysa.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt2vyskgztp.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2xullttxo.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2cwwurabw.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt2tgzrsjaa.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt2efsudlvn.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt2soxurkex.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2bgxzhkfy.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2zkeikbaq.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt2aiakxhpm.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt2mswruwjr.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt2efleyhtz.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt2trelkiqi.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt2erotjtvs.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt2nnjurfbj.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt2yqejpnhp.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2mbvuovnf.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt2wpvwqonl.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2xespxxnr.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt2wcygbnyx.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2spcjsqgg.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt2lkgqptyh.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2hvyenxly.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2uowjzvik.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt2bfacolku.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2yqcebbat.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2ksxlrboq.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2wjszhdra.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2tkuslded.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2hztfeddl.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2uhndxgfr.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2szlahlvh.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt2sqadrtyp.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt2yrjubtro.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2vjhmxqey.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt2jtmhwhmy.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt2jzeyftee.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt2vfghkvnd.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2ywppurgx.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2auorixml.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2bdazxnvv.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt2cgdncisu.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt2xboxpwna.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt2sgtikcrj.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt2sokphhvu.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt2olwnglxr.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2xhordzwj.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2arslgylh.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2kavetmzu.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2vjqegylp.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt2eumrdeih.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2chezxbow.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2fklzrodx.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt2jgozjxyn.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt2kitnxtwt.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt2axdxzexf.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2lmolppri.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2eqlxfiar.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt2ldscrgcb.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt2orhltouz.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2dwztwrlo.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2nmtmxxvd.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt2zjmvpdro.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2qqqukbul.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2eubmuzco.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2nhjtaeat.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2gwrxrvmb.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2sjxmntlj.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2nvgbebtw.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2jdperxra.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2lfnxcajp.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt2rfjaxwuf.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt2bpkbijuz.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2fdbetflc.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2wlfqjqhs.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2inkmtfbk.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt2fnkcvxuq.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2wrcebclk.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt2oejflxmw.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2oruzlbdx.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt2dctecfyp.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt2oryyezpk.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2ojcsxteh.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2rkpxtxzo.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2mzwxvnwr.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt2stgefgph.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt2puuewzot.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt2eofwecms.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2cvidpjvl.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt2srcmymsz.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt2hsiobbfs.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt2jqzklwgc.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt2wpoxjesf.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt2ifchslvf.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zwmhlbwm.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt2rirpscrf.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt2jsqsubof.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt2yrtjrvjc.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt2vyjmmkcz.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2sfmideoe.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt2djorwuai.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2znbetdwi.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2uzcoycey.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2gcayduao.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2vftnhlzb.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2azsylpuu.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2etzobfau.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt2uxenvruv.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2fjhcdioa.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2akyeowpl.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2tmndnqol.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2vgqdilio.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt2kmigvymu.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt2gxfcrbrp.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt2znxanknc.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt2zkgtzspe.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt2poaemkla.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2jqpxlgbw.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt2twxrtjdj.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2lzwyqysc.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2gmbcofmu.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt2hqpslxcw.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2opqskwwb.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2msadhrhz.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt2dcuqkgog.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt2ixkicwbm.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt2tesceego.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt2wqkxzlvs.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt2wmqmsqfw.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt2elluagia.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt2rlmeyyis.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt2zngjqrxw.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt2hdlibqfz.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt2njrpphll.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt2fmcudpyd.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt2ueomdpsu.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2bqotfzhl.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2zavhdzmu.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2nucmxezt.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2dqcqjqkn.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2fjfqspkn.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2lcootkzw.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt2ccaiogmu.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt2fkdoiikj.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt2xkrorfrl.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt2ahhaosgp.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt2cgeopdnt.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt2szygusdo.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2rzxolkwr.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt2zkwaznvu.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt2vvjimbqx.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2snbkuqog.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2ppdukfmt.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt2qnlhqead.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt2afqqmwva.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2ravuwkzm.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2kbmfsayk.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2gffutfvc.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt2vmvjjfwz.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2wlrcdwmz.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt2aqftskpv.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt2qeeubngj.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt2wxjgetfg.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt2zlxpbeko.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2dyppujcp.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2rcaezjnv.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2fdajrfno.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt2ykiyhaeq.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt2kzqaffeu.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2tzfwkivs.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2peqedqzl.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt2wudsxttp.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2ergawskd.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2funblihh.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2bdfonwzd.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt2mfeyrjln.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2sriojdwz.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt2yodmffvl.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2pzxtwzry.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2fugjegwx.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt2osbubcjy.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2kmwebzcb.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt2iuseuvyn.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2nitewvva.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2khrfpyed.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2otkfvzyi.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2fqjqhpuk.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2knjatqlg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ajmmygev.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2abbexqrr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pjnbfwkt.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2tuowxppg.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2welsqclx.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2iksdjlze.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2jptgfyvr.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2asswtmcy.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2ztxxgspf.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2arqfglak.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2ziyzwxna.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2exolqvff.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2ssnxusmf.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2twwqxagq.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2wolojfju.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2dqxrdxhp.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2zddktsvs.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2tnlidirs.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2xluvhnkr.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2yqpftcuk.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2kshavmdx.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2jbbgopwk.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2uyzscojn.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2pukhfbib.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ynpnwddg.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2kekrtkke.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2qjvteydj.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2gfeglxnx.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2sxvxckpr.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2wlpwxgrh.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2lqvremke.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2leeppxbm.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2qyfepiho.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2fbzvxbpd.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2puvtwezr.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2yuicuelv.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2rpyyiqtg.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2xypwoiwi.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2mzrccqmp.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2sbgcatiy.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2lwiaqpsn.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2bztpulad.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2dchtxpox.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2ufztsqxp.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2nzszjwmp.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2ajcydmhi.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2zzsslmab.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2yoqunjkb.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2dpgutvmi.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2exabissm.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2lrfacspt.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2jmahatch.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2tmijmtth.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2zuqzukfy.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2bsyecwoj.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2kqdjbapy.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2qozcunya.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2ldmrvqcp.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2wabnnvlw.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2affkutwb.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2fqewdjlh.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2cqgcrjax.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2kxjyxbpj.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2duykaout.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2tzeczovr.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2xnwqxnar.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2gxxkueka.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2zmoklqsa.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2qibsizqu.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2mbhdnwql.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2vsvhopyn.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2vhsvhlyp.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2vijhjpsy.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2ifzxdonk.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2pyvtapyn.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2ryiqplum.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2zlgxjoco.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2iefxuwgh.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2pvokofsc.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2rvmtkdcj.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2ngmzwzvj.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2ougpaokg.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2uclruzwb.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2uzwekskt.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2razlkttx.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2vpygkrma.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2nvhfwsac.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2rolnycbq.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2smsdtmbp.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2xezevzos.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2lpuaxqgl.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2rxqwavpz.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2mwkvaujc.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2unrefsru.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2tfcxowcy.html


<!-- 参考信息 -->