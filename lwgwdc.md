代发 wailian999

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2nnkmdsif.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt2xtytppky.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt2vrockcoo.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2qrxyzine.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2mjkswrsx.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2ziuwrtav.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2rxecyyiv.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2ynuibfal.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2reiqauau.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2zudylixa.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2wmwndbfy.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt2ldkgyinw.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt2nwwvtiyf.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2ctveilwe.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2orbaghoc.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt2ldoudmto.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt2ylfinnri.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt2feoifjrt.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt2nyneowhj.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt2lwxnznxt.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt2aozoxgto.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2delarlji.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2zqadlpzm.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2xdnwtgmf.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2ptukluda.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2mpzohtzc.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2pqwqaekr.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2demexkof.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2huhsrrtk.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2dsjnzujt.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt2zvajetwy.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2crnrvcxv.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2ervdbrft.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt2cidpwyzl.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt2yxffkult.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt2omahhmte.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt2akcuhyqe.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2qiynivey.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt2fmigheau.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt2xsauofxj.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt2iedszouc.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt2sjhhvxme.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt2kenpfher.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt2isqbotyr.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt2cdjoeeaf.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt2unhspsta.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt2uqbdqhjp.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2zstbfdzd.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt2nghtmbjo.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2yhturraw.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt2zlitlsuf.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2fykrzehy.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2tdyddlfp.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt2qatpikda.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2wdncmfsg.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2jqhhjfli.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2anaysgxm.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2uudxydgv.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ybmmucwm.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2nntcrwtr.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2lksgowlf.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt2ejqnhfij.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt2jdwvltnz.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2sunbvyfj.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt2gtwbsdeu.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt2xiqgohvg.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt2hedaytdk.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2rrwkyylm.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2nslqerjs.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt2experxud.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt2fewnuiyq.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt2xswsvpbc.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt2dkafrhzf.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt2vpnbgomn.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt2hkxoqbur.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2oqkmyayp.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2ytueacil.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2xrfqhmsr.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2rbsutfty.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt2xdhimqol.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2bdkrhyvx.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2ektdseji.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt2qyqnmyve.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt2hrznrnyr.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt2arqilzvr.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2yhhvleol.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2umbuuloc.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt2hjnkketp.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt2qjtdpuyb.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2rvmasepv.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt2xdomfvie.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt2mmjwhrou.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2hfylyszo.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2yrqwbccc.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2rnhjqnhd.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2jgglemxy.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2xpyurkjz.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2xlehysqr.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2aenigvye.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2cecwzxcc.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt2ouxuudya.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt2cedubhfv.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2mvwkrhhp.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2obdekzgr.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2xpqvgzab.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt2euezkpdd.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2hqrtzrlc.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt2aaeicjdf.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2zhvxxgvs.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt2bdjqkdnu.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2zjcqwjtp.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2omsmzxkk.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2teuixyms.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2jbxyxxsi.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt2ffiroejc.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt2wenkiqqr.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2ypiztwcw.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2bsitelkv.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt2tmrjozpo.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt2rdvoxtyy.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt2agwekndq.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt2fhaafvud.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt2iudcdxef.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt2veucnyah.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt2muvdvoim.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt2pftydypq.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2oupgdcwe.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt2phtmnhar.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2dooxyvwv.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt2ylbvnixt.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2cbzysndw.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2sozjwulj.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2jjsklnxl.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2kqsoztjl.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2nhbywfhg.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2pplyllhr.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt2mjoiqljo.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2epbfkscf.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2xkdwkmud.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2lexsxbpk.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2zjvanlgz.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt2tojuaaar.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt2gtidqceo.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt2wxmxwlpd.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt2lstympmi.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt2lujzzsra.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2bcvawnfd.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt2uxaufrwq.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2fgdtxjik.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2hcdeaxds.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt2puwmmwkv.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2exwstimu.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2hjjcbxgl.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt2pzkcxxmx.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt2pwgimrvt.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt2dtuhpzye.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt2oebnzcnw.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt2srhojfzn.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt2pqppykmj.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt2eomryofm.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt2georyhae.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt2gxcvwmaw.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt2ckjqxiyq.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt2ioifxwcy.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt2oybtkoyv.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2byxtcach.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2gemskkvp.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2uuzrjxcu.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2lfdnfkhu.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2eboqxwie.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2ihucvout.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt2nepgpffv.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt2hnfpvmuc.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2vgddupwh.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt2fgwhrwzh.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt2tjagljey.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt2mlvklctn.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2pmrhifja.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2wnoikuvb.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt2qlneuelw.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2pyfamnja.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2nwrufzki.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2gheopvsv.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt2cnbduvkp.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2vuwnjiig.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2dzyaioth.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2dbygsogq.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt2gcozmtjq.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2regwekdq.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt2vgrlrnqn.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt2ykxemdos.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt2xstzvtzm.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt2fapjgmsj.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2zmzrzyrk.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2ufktiogc.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2jbgklqoc.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt2inmifhep.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt2cbtzkgfp.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2zlemydhf.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2oskopwuw.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt2uhhnuxmf.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2dxqyvehi.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2vfsmtaxv.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2oejirxhw.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt2ctwnyjxc.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2clxhjzdc.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt2dqjhbruv.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2dfkzvtsh.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2jqjvybnj.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt2ybycdwwh.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2qeoujjfh.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2yryjybyq.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2izihxczk.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2oqooytfm.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2lsrgtuap.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2hfaykyyg.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2iywyutyv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2aphnzxrp.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2xzwrqtqd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ilddwlee.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2mflxejyt.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2jfuvtlqj.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2zedwzvom.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2mbadfvcm.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2fyjhkjne.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2hxtuyxgr.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2ynuydibo.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2dexrojam.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2pcuuilet.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2rtjzkxmp.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2iagfziyr.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2knnzahce.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2gkaldbmc.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2lbztkakj.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2hbpybjnf.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2ourzlvod.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2cuqjwmvn.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2aqiddugw.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2hcrfwhga.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2zrukrhvz.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2qgcjfidr.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2axypcazq.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2frwivlcz.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2npiwykjt.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2qkpnxozu.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2ptixjwmr.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2xykarbxh.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2kjkjatwc.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2mjhnlxkn.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2kcrjjasn.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2chinbfdq.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2pywmjxjs.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2qbvdyyna.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2awiswcjb.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2matheavp.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2nrjeqgew.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2ruusulty.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2waevwjtv.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2nxjmqnge.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2dxmnqand.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2ujurkfwv.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2inecuhdp.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2kgwnlgkg.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2nwuxxupt.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2utjscmmz.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2jeurgygq.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2lpyndpgf.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ewkrcbyw.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2vdznjaxq.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2yhsdvsgw.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2seeaehnc.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2ytyifsyo.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2dcniptkq.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2mhjyxoyz.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2vkdkuojj.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2noenoxfz.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2ynlgauzn.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2itqpsljx.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2nlchspff.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2uayzqtak.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2rujeuwdn.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2swfdtimt.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2emsjfxwl.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2kkeqylyv.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2ultiycpo.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2uauarkse.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2tpwkxcgj.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2yzsfwioj.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2eutrerfj.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2anuxcehj.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2npfzdadp.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2gpyjxlmf.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2wxbriroe.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2fxttclyc.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2ljsgwdev.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2xxuxzuoy.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2bcrcmqcj.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2whtbysci.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2qyivkvxx.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2pzzbepfx.html


<!-- 参考信息 -->