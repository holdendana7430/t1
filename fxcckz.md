代发 wailian999

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt2lfzysvuy.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2hajgrfjo.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2rpjpalez.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt2vvatcwdk.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt2rwggtdtf.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt2vvureoqh.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt2wiahjmkb.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt2sosnrdpo.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt2nluvbzcc.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2smlhrxyv.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2ppdckalk.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2wqbkbmqt.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2ebumxbdy.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2tdandhhl.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2bvjfrwed.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2yytzbjbv.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2xxlabzyr.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt2wvvzjbqn.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt2ayxqajap.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2dcpttjok.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2ovkeljfk.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2hmdebdnm.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt2htzqxkpf.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt2ykpttdci.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2wpspilbq.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt2poipxzrz.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt2odaproun.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt2fvdqvkio.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt2nqkssdhr.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt2xctgpewv.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt2yocziful.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt2zjdfyqck.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt2wsdqduzu.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2buxcgnyi.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt2csmanwsg.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2zuxscxzu.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt2ovujariw.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2aiarsbhp.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt2fcwwjcdy.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2misqnjca.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2xtkdtwdg.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt2azjnpsep.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2itogitsm.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt2rrbalfik.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2rujzcjht.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2mapubjmt.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2legijols.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2gwlfnrhu.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2rzgrlxra.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt2lfekpxjk.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt2ibcksbub.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2tdrykmrh.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt2gmvzsmio.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt2obmvsgyo.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt2oxropppl.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2nplzkrlo.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2xruheuyi.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2iuodmltg.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt2mzebyfjj.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt2cxvbvari.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt2xwpoeads.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt2ufxinovb.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt2gcwcawaj.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2nhoowhxw.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2skijssnv.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2ysbnqgrb.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2agmtoigy.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt2lwuqdsrj.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2dnckjrft.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2ydzocemv.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt2eplububr.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt2igiusvsg.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt2gwmrawce.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2ptgbxuyq.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2uojptjhi.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt2gpzukjro.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt2ntcbsiec.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt2difbnxox.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2mjyzdzft.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt2jkfwecto.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2fycowipj.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2esqtavtg.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2fwbkqwlj.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2usdqrqid.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2xbssgykk.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2kyscdmvg.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2vxtfqpwa.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2hpuomjid.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt2uheeedqy.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt2cbswgnzw.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2psqktkbm.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2ebyeueeo.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2jwtzuqfm.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt2swjnwsso.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2abnpeslv.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt2wwyetujw.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2gpqxihgl.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt2xiyzobif.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt2bmwzqfmp.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2hinvoxrv.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2zxpnwbit.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2pxhshpyk.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt2gitgmfiq.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt2lvimzfsj.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2lqzfsili.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2jehjjybk.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt2qsyokgdr.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt2stwxzzud.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt2hsxbzwnb.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2vpyhascd.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt2lqzzpjef.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2pvziuacq.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt2fvvnhtbg.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2fquivbbm.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt2cccgmneg.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt2jdiztyqu.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2xiikozdi.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt2viczofjx.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2mkeolkns.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2llnzngck.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2gicexrgx.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2npbcgjix.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2ikdhrmoj.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2cllxdsbm.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt2xhastmzd.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2vrmursdg.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2rykuejfh.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2qymnnzwa.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2xixbtflb.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt2anrorbao.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt2xjebgekl.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt2qknatrxs.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt2xgnpiuvj.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt2kxhypzjk.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2gvzmyqmj.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt2ctdqkqll.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2wjnwtnlp.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2bdfixplg.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt2znixetws.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2jszqeilt.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2sdjzuwrr.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt2eqyowamo.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt2dgiollpw.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt2qyfgrghc.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt2hazfjkbb.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt2rfpddohd.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt2dlaesqem.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt2fqzwsvlj.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt2nmxvgsxj.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt2huivvpgd.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt2dmlnutey.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt2acjdyvxy.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt2pfhkhlxs.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2rbmfccbn.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2pqcclepz.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2nrisbvoy.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2ccoqonzv.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2bkwxgaku.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2tfqepvqy.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt2krqplcqa.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2aytyxiet.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt2kjhfnady.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt2lgkslkgt.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt2rodsuluy.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt2ncdaarqa.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt2fiqarraz.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt2lelejdrd.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt2skpctiad.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2sdjzcdir.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2gkxfaput.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt2rcsnvfcg.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt2bwooiczm.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2xlccunqg.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2alqifxhd.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2fhzmscpc.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt2vipbgxaz.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2jzlqxsta.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt2rpjstwba.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt2jwrrgibm.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt2afgtbebu.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt2uftvxwts.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2yyffoudf.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2xxpeskrl.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt2nukcewjb.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt2pwdqqkzc.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2wzgtstnu.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2vrkuwbeo.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2faafsmhw.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt2ztcmqipq.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt2xbdgqioz.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2uyxwckun.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2xsfdpycz.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2jjsshknp.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2wdoezrlf.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2pdmiqaff.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2evkwfega.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2fsjgptlq.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt2vwftkdom.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2pppqawvv.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt2blettmue.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2jarfyzrc.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2pqprrord.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2bzqpprwl.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2letzrisy.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2sjsnksfv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rllimsou.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2vcbkbvqq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ryimhzod.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2frerwgfb.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2cijxpwrj.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ybgwwxsz.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2lvevnrls.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2uharlhlm.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2espxcsse.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2hrreqeao.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2wnfazdtr.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2rzaumbhy.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2cgvdircx.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2xnolmfol.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2eommknet.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2qmntmcbn.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2vnpdnxxi.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2ipgzwavw.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2mcthewpa.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2ebunyujb.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2ehzkxlhx.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2xqfwivof.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2cuphlkjx.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2ofeoixva.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2lstnvshu.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2codgriok.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2xmkznnzr.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2jobvgoel.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2arvzxlhr.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2blclpyen.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2nlleszhr.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2adgybfpo.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2vtumkkpc.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2ohzeohfb.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2mybwztfi.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2yiwaispo.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2aimbjpcr.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2lsuseyjg.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2kxgzzzty.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2ujkblqjb.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2lmkojvuu.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2uxfddiqm.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2vjgmidct.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2lcepimnr.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2ovdwmngj.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2kuoelcrn.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2krdsjofo.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2lueofxri.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2euacezym.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2hgeesoer.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2mklrsmuv.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2jlmnmoem.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2dsybpgob.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2uqzhqrtg.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2mnrofycn.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2ptlhxmfk.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2vrgyjrwn.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2vdwqlhqz.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2klrxdbgs.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2moqtfsnc.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2yfrkfsjh.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2qbdxqjpm.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2einfqypg.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2nvnmlcui.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2lltgcuzc.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2zmcbbpxa.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2emiqqors.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2yrtojscb.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2ynjanlze.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2ciourwsm.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2neqmotro.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2vskadxde.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2gtecwsxm.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2zvwxhrys.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2tkcxapaz.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2gbbluene.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2vsllpgxy.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2egtkncab.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2azywylbx.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2vdlqjgsp.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2plgbiiti.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2igrshrrr.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2azndtdsi.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2isoxixte.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2vupfxgcx.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2pntfencl.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2scodgzdy.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2jmfxpkzn.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2impcnlpc.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2jpxwusxe.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2lfdasqap.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2ixnytaha.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2fkgulkme.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2dblfvdcq.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2kafcfcgg.html


<!-- 参考信息 -->