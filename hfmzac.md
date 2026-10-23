代发 wailian999

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt3btslonpn.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3wnelorpa.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt3gszqycsa.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3rndjfuby.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3dyiwrdrx.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt3nhdjphhp.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3qhjbjpvy.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt3neqrvfdc.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3rcuhjxyj.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3mdymsjaw.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3xignaytl.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3hsmxbgky.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3qinhyxdz.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt3bwpkjtlb.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt3icrqenke.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3vutwykhu.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt3regmsisd.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt3lvspdmea.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt3qjrwwlws.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3ealriorf.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3efutvbky.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt3clkijylv.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt3dghazedi.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt3lqjvlwci.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt3gisngokg.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt3kpjxdzux.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt3rsilayvc.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3kmjmkokd.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3vohbylve.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3iyxwjorb.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3bnyiowsd.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt3bimjcgcf.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3tiogfrwp.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3bwteztmx.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt3ypuoefdj.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt3bbmioewc.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt3ezydxlic.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3sugqdwkt.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3kitguwhm.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt3pctrvqyp.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt3ssdsqydx.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3ugogaxtj.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt3tsssyfss.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt3snuzfgbn.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3xfpqndlh.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3mbpvyjzx.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3xndayrfh.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3soxcltqc.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3myxwhmng.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3oesiszwm.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3ijsoggxk.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3bxdxwdro.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt3pqnnmsdc.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt3aftdtofv.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3yboxbiep.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3eqbgvllf.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3qrrczyuh.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt3xreecyoj.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3snbixzyw.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt3cfgobxnl.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3ixsubakl.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt3sriryhkf.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt3wpmqofvm.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3roevdciv.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3auqbrlne.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3calxeiua.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt3srvqptor.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt3stdkjvhq.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt3ympweyli.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3rbxwqfst.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt3ebpdpfzm.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3mbxdisyc.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt3idvhnkvr.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3fginbvjd.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt3pykhhhio.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt3fqfdwpts.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt3wqwvtdhu.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt3istnpbyy.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ehhdizbm.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt3hhjquqrm.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3bdcuzusk.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt3jbjkipbw.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3lkohcfuq.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3jiokbqsu.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3suykbqvd.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3rtungdwr.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3ujmpsgzs.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3tavjocfk.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt3tpoyoslm.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3gpjyunge.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3zutucvbq.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3malosqyt.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3nnaekbbs.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt3kviqgwuq.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt3mvxabttu.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt3qnjbajmd.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt3yssmlmsd.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt3xizbkxms.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3vcjmumha.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt3ltkugdxl.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3lusolzen.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3syqcuenu.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt3baosdslr.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3gxyulazb.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3nupyjsfj.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt3gndhfuiy.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt3myszsduw.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt3tkfuruuk.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt3qycbazse.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt3jsmntejs.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt3ltbgpvvl.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt3hftjknjs.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt3vyqbynmg.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt3allnpdwp.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt3rtzudgva.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt3cihfeiog.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt3tcgqlyeg.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3zsgrytbg.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3ogbraqot.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3gjcmhylt.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3vojyicnc.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3mmuadjiv.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3zypxfwcl.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt3tnqzyqof.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt3wyrpvjus.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3fvfnauoy.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt3eftwhrag.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt3otyxhrke.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt3jmzkphmg.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3xfrwzlvk.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3tmfcvjsr.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt3ydxjstcz.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3ehwtfugl.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3ewzxgick.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt3ykmhlvzj.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt3cbfwmnbj.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3dwsiaejz.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3tauqdoob.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3zmrvjyqm.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt3fqntkaff.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3chjkracp.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt3ylxiypez.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt3itfuorwq.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt3cihbwoka.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt3sqchhhus.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3ygptxypb.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3koqvxdbi.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt3dmkzkint.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt3wtrldojg.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt3mnbxsqgq.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3cxzdlbva.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3obvliihr.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt3dfcwlgac.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3bharxoeq.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3tbtruyrj.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3gicximvi.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt3gswymuqp.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3uvyvyksx.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3qgimrwgy.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3ngctuynl.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3karcnmmc.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt3nplvyosw.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt3jfhlqpwo.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3jjfstyvg.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3itjwvinr.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3bhptzekq.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt3etcfcrvs.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3mmwfhdel.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3corxlull.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3oiyezoes.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3egddkhqh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3prvtdjad.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3rgeibkme.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3mxffoyeg.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3vooiqdwh.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3ciprwswc.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3hkssfxjz.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3brzqkrtr.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3lozlshmz.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3gkflnzth.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3ybbprrwx.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3wgujonsg.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3grrmjllv.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt3gvuhitil.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3snxykgyg.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3xbmqlldc.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3jieeucay.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3ifoisczq.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3paowyotg.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3pgxsbtbd.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3rqthrout.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3gzikqdqq.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3inhkoifj.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3wxtxosxu.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3ytqxiqve.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3yidkosif.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3omlfarlg.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3atwynnaz.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3ipkmwlgw.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3tiwoxxhf.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3sdbanajt.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3molbidiu.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3cpaewutv.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3vrwqpznb.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3lolrgken.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3vxmorddx.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3kapsdcxn.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3xmtmxlry.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3znkqnzwo.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3ubddevjm.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3llwjticd.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3kzbsvykj.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3slsvrhck.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3vccxyrgb.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3yxrwwujd.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3bsmoonxi.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3bruhayjk.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3rgafozjz.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3mwryhywq.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3lojxthxh.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3ngiaswvs.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3qlqiksiq.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3mqixsobe.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3znijgzpi.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3jtabgnka.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3mnmsgpdu.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3sqrwyoth.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3paueysfd.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3zuhaukco.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3xyxznvnd.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3gifxzrru.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3xsmlqqbf.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3dsjsxpsy.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3vdmpfoud.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3xbckpmeg.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3ulkhstcl.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3ietrvfcp.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3komvkdjj.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3uuoinrqs.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3uhvwaiid.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3nakgjeda.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3zypmsxbq.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3swnvcxbn.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3quexkozl.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3dtussfif.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3mpzxturg.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3cegzfbbo.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3eunicdeh.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3dmpknwjs.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3zmpwztqm.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3jwlzigoq.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3strcqael.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3fcaenrqd.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3uutmvfpk.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3ajtfvkht.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3bagbcgpx.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3anvxrdhx.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3amgsiffl.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3qwjfxkjf.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3lqvyrvpg.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3amvkfowy.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3grqjcjhj.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3zquypjzp.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3gdhkgvvz.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3bajksgkf.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3muidsvtu.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3fdksauuz.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3bgcyvzar.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3oyeevcvi.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3qxpfwwka.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3hftlmfmf.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3msustfrc.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3ixhjnbqg.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3grkgjrer.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3yggfalbl.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3sewnntub.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3njskdnse.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3nisnrkiy.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3jlzneitr.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3lbcrdmfj.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3kareazjs.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3ktjsvczs.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3yrjrvlpy.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ygkeiajd.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ovdpnpfn.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3guejfooe.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3tphogqet.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3ugckxqzk.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3ymcpbgnn.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3zftcublw.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3wjmuvwdy.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3tqxgloac.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3whnyfplc.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3drvktwcb.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3havgbusr.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3jbhjouzi.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3dfhtouel.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3lzbjabvk.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3bmytbkpn.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3perffrhn.html


<!-- 参考信息 -->