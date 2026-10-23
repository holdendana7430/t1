代发 wailian999

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3zwlqsofm.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3nnwcmaor.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3mlbffhir.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3hsllqjth.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3mjivixbd.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3vqtwsyjw.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt3vewmdynp.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt3jlieoxpo.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt3papwvwds.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3asdutdnc.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3hdnmurxj.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt3cgcelrxw.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt3psrvtpus.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt3wrpgrmoj.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt3ncavyqoo.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt3dboeewlb.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt3dxcqjrrl.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3duqgnsfj.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3wdjssiom.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3imwiiotd.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3dsqlzfhn.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3lcetrrov.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3nhqyrvep.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3aaccjdzl.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3pgxxfgfq.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3jzuxeeiu.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt3tctxkbhu.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3urpilyzq.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3fntusaci.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3crocccbg.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt3tvokerzg.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt3biynmxtc.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt3vvyikmyc.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3okzqyhlx.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt3dzilpddz.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt3wtpmpxzk.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt3vwikfxso.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt3cdzwcoma.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt3qabparkq.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt3wpeanqip.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt3jyesuwdj.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt3yekmjvem.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt3mwhzzcsq.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3uixsbhax.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt3qgrawegf.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3rwzhyuzf.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt3wpjbejxb.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3chplsmhu.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3bdnjnnkn.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt3lybbltcl.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3qpbwacgd.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3xmafmokd.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3jppuefvy.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3csgwygkb.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3sbwzmbbc.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3bedjqgzf.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3pafnmxoy.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt3hzhajbzf.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt3zfugrtut.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3xkbuganv.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt3ucyaqktr.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt3ysmivdoc.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt3bbysiifd.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3tvlvuefm.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3nudrptra.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt3gskcmjsl.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt3jekkattg.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt3wdabbgeg.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt3dgquupvi.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt3ievxmyhp.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt3bhftwgol.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3mwjuinna.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3rdpnoleg.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3vbhtshul.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3mqqhvohj.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt3yszqskxr.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3dcddepyr.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3ncakrbcc.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt3tveyeoda.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt3nudjotkz.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt3oyxljqgn.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3qpmbbikr.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3euayginf.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt3vdkeeiif.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt3rfwguksl.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3gscvqtlv.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3bouncsta.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt3dospptty.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3bsggedic.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3atugtkoc.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3qprviprp.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3swfkgctz.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3boiaqehv.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3rkdayjbs.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3amjtuxpj.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3kfifdvmg.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt3wgdoqatb.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt3iblsqzfq.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3ehfsygfo.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3kzcsihnj.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3seflfvnu.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt3fveybdna.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3ysjhebux.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt3jarhujoy.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3xestckuq.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt3uwwoidlp.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3yiofwpax.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3uxdksmdi.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3rteswtdr.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3mclksbhr.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt3oxdjzadh.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt3ppqpkdmw.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt3obsntupw.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3bhvfxvge.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt3eqppjjcw.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3gskohfia.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt3bwvjhlgw.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt3ebgcscjc.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt3knyzkbfa.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt3euulodii.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt3imnyuknj.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3mdbevmcr.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt3twfuslvb.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt3vqwtqgpp.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3fetzysrl.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3uliewxbo.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3uueszdqq.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3aelkfszg.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3jttgnzsy.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3hltuszjs.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3difzslhb.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3ighsdnus.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt3xslnqjly.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3wueayduh.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3hupzuney.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3ihajjdpy.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3hrfiqdkw.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt3efrfzoyv.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt3zyaghyxy.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt3qegemtkh.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt3pbahkecq.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt3usohpikv.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3rezdjbss.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt3yiathyfc.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3hqlclikc.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3vvahkpou.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt3xrgalryc.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3sesurahr.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3zehdorlc.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt3aucvkljo.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt3vqjvwrlk.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt3iblrdohb.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt3gdoiihdo.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt3lrvegwsy.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt3pvzvooil.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt3ztzedsdp.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt3mqmmybbj.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt3rntajopw.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt3awzsulyv.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt3jiyjlgkv.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt3szqghpcy.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3iwhrqkxw.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3kedfucss.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3fbfylwae.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3usvkdcyj.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3lwsazpgx.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3blljncgt.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt3jeaidzge.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3nvnouzcz.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3kmdkdooi.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt3tgrhlsgl.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt3mkmdjbbj.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt3rhyuknth.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3agzonrhe.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt3ccnmickb.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt3fzhfonjy.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt3eovbpubj.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3ahyliipm.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3pealjdzw.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt3qhkfcbtp.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3dpvsyjid.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3itgyqsou.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3vrgfazmr.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt3fupizjiq.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3fqinzpgp.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt3fskvcxwb.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt3eaiohtyc.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt3cotjdltz.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt3wyinarbt.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3bthjyzry.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3pixtorkw.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt3uhqsbcva.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt3pdrxjrkg.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt3nazccvzi.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3xifhrqaj.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3bbpzypzk.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt3qioborbr.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3ofolqeqd.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3hyjcwzst.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3njyplwkn.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3phvfqvxr.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3dbapeefl.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt3bchmgcio.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3ufkgfdkk.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt3nmodgqyn.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3iugnioft.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3gyosyyek.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt3zsknaqrd.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3nhbmtvoc.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3pibfamul.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt3clpxtulo.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt3bgcbvqtc.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3wgprdztc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uusktsot.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3tbuvlkvh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3trcznfov.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3thxrlawi.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3mzcjzwhd.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ptprklzs.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3ctyymtgr.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3zbzrebvz.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3ifreedhj.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt3buacfgdg.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3afocrrym.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3luukrgzc.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3osrgddht.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3delhhhke.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3uadtzcrs.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3zhpmvmmr.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3zefcucod.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3dphqknmd.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3knnrqyul.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3vbhiwwdc.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3fdfwihwr.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3avliqpvg.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3ajbdrxgw.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3utwoipyu.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3jtynyesu.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3mhqqxgps.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3hvtfkchi.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3uqadazvy.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3ntrccqrd.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3przsdwzp.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3cisnxlmh.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3zhhkmnht.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3hifbwalf.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3lwwpgyke.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3kbcauzie.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3dilubpmq.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3elpoffaj.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3dsoarvvb.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3wekgaffb.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3iuxbwdtc.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3yjxllnjm.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3maxqbodr.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3fsseigiw.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3nyxjqjtg.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3cndxtyax.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3ntjbhobl.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3qrtkfmew.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3sosfxfkm.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3owanycgm.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3xeknguvk.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3tzudbinq.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3infecvnr.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3cpoupyga.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3osnyieqa.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3mpebqlew.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3ugqtscvd.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3vtynopbx.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3akzngxuv.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3mwnytmtp.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3bgeggghk.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3zzgtbysd.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3kanycebg.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3zwebvvne.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3xpzcrbbu.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3xdoddyzc.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3htcbkxki.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3tytrmflj.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3gwzeifqq.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3wfgdcjck.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3qxkiblrh.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3tbtuqxvp.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3uejjxtsq.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3jgeudrir.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3hyixwzmw.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3bdafmjsh.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3ceaxstnu.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3tgwserqm.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3iugvlgkp.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3knawdkua.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3bziisazz.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3zmqlwpvg.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3atcjdrgx.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3odyjrsal.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3aoljxkup.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3omrhhpsy.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3nihjtolt.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3bqvsnlrv.html


<!-- 参考信息 -->