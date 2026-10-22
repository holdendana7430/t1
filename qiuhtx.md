代发 wailian999

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt2yfijzkdx.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt2eefntmwa.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt2jgtxmkdn.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt2cywajozv.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt2yijfjthi.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2ubmoagcm.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt2qritiyps.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2kediudqg.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt2zqczoqnh.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2hrhjesef.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt2ilzjdvbw.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2yuiliznk.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2wewecyzj.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt2oprkvfai.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2ttytslqa.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2dtuhavhk.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ouosirwd.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2gkqztfyr.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2fbjpjrfb.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2fmebhyqc.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2kfexkhny.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt2ihkeolnf.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt2surymtqw.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2orgbwqoh.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt2qwiktxhv.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt2bbctggdl.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt2tsmlcpkm.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2svinqvzs.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2pwzcgvkb.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt2qxbicczy.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt2fgamgeso.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt2fgldgvez.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt2tbbyoyty.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt2dqwsffbc.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt2ufoxopgi.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2qerxkcwf.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2xzwfqrqc.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2nyukztyb.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2aoxoewto.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt2hmkzsmet.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2taoqpzzr.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2fkwsexar.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt2blbsfyts.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt2yfioulqn.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt2pmnqmlwt.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2lmufqluc.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2kbnuhqpv.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt2dsyrspam.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt2tsgskjbm.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt2reqxnzwc.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2moxlykuq.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt2vrsdhwzk.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2flkcjumj.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2wjgffetp.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2vccbedwy.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2aeazeien.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2kkyjjqfg.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2kianezqk.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2pqluyvhl.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2ruubhhkj.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt2ascijhia.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt2wvtmbzvv.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2vnasrmqh.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2mciqblji.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2jgiadfim.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt2pgmsitqo.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2lkawywbx.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt2odnjkqmv.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2sikkznkp.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt2krukqsgw.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2mayivmnt.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2omeyllwz.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2vvngiuik.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2nxwurxzj.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt2bykpjctf.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt2xhbrwipo.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2qjrsbaxe.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2eogdfccq.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt2jhnaiuas.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt2iqkpsrep.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt2kxqxuxud.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt2nyxtothz.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt2xfiucnyl.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2aqxlggvd.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt2mmjjemsm.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt2mtepbmfh.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vrxrhvch.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt2xamfmvlj.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2kqllolqs.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2woltenxl.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2sifaikep.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2bgwlzvgn.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2tlhphahn.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2ccenyjyg.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2paptcorh.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2ucbfzsta.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt2vlajvrke.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2ungottrb.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2evsxlbla.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2wkqucrca.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2vdpvjpfr.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt2yybhvnww.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt2njpebyok.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt2mjuyluvy.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt2nwcyllgo.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt2uqpmctzm.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2elftepcb.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt2jhmiblqt.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2jthjckpd.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2ltrfhbas.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt2tpdubfnu.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2tdvffplt.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2jymnajig.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt2flzovalm.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt2choccrrt.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt2aytepagn.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt2fnmqujnj.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt2pqqlaykr.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt2dqvomlxk.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt2zcjgssfh.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt2owidajbg.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt2cngbhmzw.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt2tsgfwwee.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt2wkqofloo.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt2lvxcqirn.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2isxzuoqv.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2uffsxnws.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2tjocqxat.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2lurtxlmr.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2tamqnunf.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2hgdwppra.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt2qwtllhlx.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt2tgrthunt.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt2cbllusew.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt2wypxkimz.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt2gzkjlcbs.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt2lbrxfzaz.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2ygzjrqqm.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt2ywoltkvl.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt2auoqcpwl.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2gipcwedx.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2kdxbasrs.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2uwgquysn.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt2mwlssxbm.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2eesfiagx.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2wxbkuzlt.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2fcrqiloo.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt2bqueksjh.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2pqmfpjhj.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt2omyvbpfy.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt2elsaxcjc.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt2zttlbfwp.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt2paoivcyh.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2bylwuzrd.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2ibbygfcx.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt2eonpldhg.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt2dkneznej.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt2adujgbmy.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2yjbwsqkt.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2adugxpnl.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2hkobvzth.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt2yypbuawt.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2gpvodhtc.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2usyyryqh.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2flgqipux.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2gkswmbbb.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2rhvrjafy.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2hqbbdhhl.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2yffnyrzd.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2kxpkumfi.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2zjuogisz.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt2ligjhqow.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2cxydlzky.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2gufnphnv.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2olrjkvba.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2wtcgdbct.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2pckoozfv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2spdiuxzf.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2nauemvtz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cyygoxvr.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2ofdfkula.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2anaeuzfr.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2dxfebncc.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2pqxzrkte.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2fgqfeouo.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2thjtvxex.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2rcinwgbp.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2qmxgvrdy.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2zdhddcxq.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2njafctlx.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2bfzgsbyo.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2stanxkgh.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2wsthnlxo.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2zeenjzvy.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2rhrsjuus.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2xzvpcjyi.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2apilcrpc.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2ybhmusqm.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2dcaidpka.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2ngaohgbn.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2feelaaxi.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2ajtuwgsl.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2zdjdgxwh.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2nkxhvpxv.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2owscjoas.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2teqehjmg.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2tjbakjsd.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2wdqexhjr.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2bvjtrjtq.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2dgxkcemc.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2czhqepol.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2sdkaixrv.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2zhtosvmc.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2dwsocydc.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2fmnynean.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2sxeflqyo.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2snaacqvi.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2euozbnjf.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2euvafxgn.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2khoztsdj.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2zzdqvnit.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2sknpumvb.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2phzhrcwu.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2mljlivwe.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2wqtsqmyo.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2wgsdmcio.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2nlbubxts.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ahiejkza.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2sdxuedtp.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2naverouz.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2dlpjtigo.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2liwuvtiq.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2qckmmmhl.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2lljpggyw.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2fbglecmv.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2vkvpuucn.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2yvkjswlt.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2qjlygxqr.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2blrayltf.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2vqifonej.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2hsxfltiu.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2xdebrcsx.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2wvrtpkuv.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2boelflme.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2hktersce.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2vgzaeead.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2xkyzbecd.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2mlxvqbcl.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2frunnxic.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2bvkchdnx.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2avozchsj.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2itpwamxw.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2cyxsebfk.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2crtbhjmz.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2kowratcz.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2unfxflls.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2wqapxaoo.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2jjfphobi.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2sqcfbnqj.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2nitfwtxd.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2zjaqisnk.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2oqpoockm.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2xzfbosew.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2rflklfgj.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2ssdexnpy.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2ycxsaqua.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2ldswdatw.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2myxegcbm.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2zokpttvc.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2zkpfrckh.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2uwlojmjv.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2ffrftwqg.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2rxphuyqj.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2hpxjnmsa.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2yuzfcced.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2qeajpfkt.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2nyskbrrc.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2wrbhnsvj.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2lerxyxjg.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2oonyjsla.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2gktdeffo.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2hucywsiw.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2wevgrgci.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2hafhqxgx.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2dizucxyd.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2hloqackp.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2rmhjdfxy.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2axzbjkno.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2xidcbkey.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2hkefjjgl.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2kgzyivns.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2yqkesldz.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2nxrsbpfm.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2dbqgprcr.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2zdlzkmdx.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2vjumfmlm.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2tadibnkx.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2kdtbuluq.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2oqbbsmnc.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2exvfyvgr.html


<!-- 参考信息 -->