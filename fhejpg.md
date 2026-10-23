代发 wailian999

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3wqjgbiur.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt3ubzuphsi.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3lnadjusl.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt3egsnjaht.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3mejxzkrw.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3pdajxrzw.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3jniinueb.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3jmfniivr.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3aozbtndu.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt3heduviko.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt3evsrmbzk.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3ngoyhgnh.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt3tejicxtx.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt3gpbyoxzk.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt3sbeifjec.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3beikyqvf.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3irddkeue.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt3uzwueqwk.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt3emiybsqt.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt3dfurxmye.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt3yqcxfhvq.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt3syzwwobf.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt3vpevsuvf.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3sghfsssl.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3vcmjjmif.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3genwigas.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3fjczryct.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt3qnydjevy.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3nqafzaim.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3tdsrlovl.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt3qhzvjndk.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt3korxtxtg.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt3zidpngcx.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3kglimfie.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3cmjfrlrj.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt3byvasbuf.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt3imsettmz.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3gcpeasrx.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt3ktugllkq.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt3vtipkxmf.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3idyeeukq.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3frzcvtzz.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3tnkflqii.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3khxqiuue.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3whuqymxq.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3odwdxogj.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3hhvwfvqr.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3cjkhrlsa.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt3semymnsa.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt3nmzcrlwm.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3zomydyvu.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3uabcpzml.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3upoiopps.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt3tcetovuq.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3jncvfyfa.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt3ggtkmqco.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3nsgbvgux.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt3mwqatgtf.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3fvpogxqa.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3gcsnimzn.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3pajznnpx.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3oketvwev.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt3rwulolaz.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt3nostdjqt.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3uxxthsqb.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3zupopecf.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt3mknrjyva.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt3zldcnufi.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt3ovgpkkew.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt3epdvznde.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt3isbpmrbg.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3opjmyllx.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt3apkgpieg.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3tpzqdlfd.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ackoflan.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt3ngowhkfz.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3nfupfuxu.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3etaqcsky.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3tmpzraza.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3qjfboozv.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3ktghdbjv.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3ssozyvdw.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3ozmexfdw.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3cfhlkhti.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt3hiifdrkl.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3nwpietbd.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3vdzberji.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3jueabkmu.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3wyixcntu.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt3bcmeulxz.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt3smcmpjpm.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt3prybepsn.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt3ldripapg.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt3fdbhlxav.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3lmdhlmbg.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt3ozzuxjuy.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3gbdxgsxp.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3fygsxeby.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt3ivawjchy.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3gkqznykn.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3tonpoxrm.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt3gyjkweom.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt3plsubhja.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt3amwfaibb.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt3nksydgwu.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt3ppdwxwup.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt3fokpyoys.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt3tpehnzyo.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt3wvmsjeuj.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt3zatxrdho.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt3dlegtbqu.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt3grdvwpov.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt3yfxjmtio.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3oioecucr.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3nrcxlamq.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3odladqde.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3semtcnlz.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3ngstxguv.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3zpfowuav.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt3xknbdvje.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3zwllanhz.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt3kdqjsnaf.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt3dnoatlsa.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt3ldeihuma.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt3nsxotlkv.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt3vvntpwbo.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt3jmdldjpe.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt3tsynrcep.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3ctizsvhd.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3ooamatmc.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3axxfwlmd.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt3wuaktggg.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3otpttllf.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3uhacshkc.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3aalydbxc.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt3rdjdlygj.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3desgzdrj.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt3jrcatajj.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt3dzucuyhe.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt3plcpkxoh.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt3ccmarqib.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3eistrgag.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3quafywii.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt3nqdivwus.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt3azjpyney.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt3amnaekqp.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3ftrwfwtv.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3xnxtdnot.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt3akgehdjw.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3oklpwolm.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3egdxwstr.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3sivolidj.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt3ifkqpkqa.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3eavdyqxc.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3fipzruff.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3fjxbcbbd.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt3rbdwjbjd.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3lmjjojig.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3afwpheic.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3jsxxhhpx.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt3zlfqttko.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3qjysdnkc.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3bjnwzidh.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3ryfjymin.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3xkopnjlt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ustxiycy.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt3hhfucxjn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3llnnkznx.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3kklkfoix.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3iuvduhim.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3qibvkejv.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3gnxwhaqk.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3dkdfhstw.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3zrsqnvvj.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt3nhyefyid.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3zglxvvqr.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3houekdsm.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3kplczceg.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3fvpdejto.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ekgpuwsm.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3rymutvle.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3ipkpvbrr.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3hhggfbxh.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3yyifchke.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3ghalkyvt.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3jcztrxwq.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3jjomgwnr.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3qselxpfm.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3aftdvujv.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3rfytlyvk.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3drimhspa.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3bknffmro.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3fztbyhel.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3vrcfsvrz.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3aqyyardu.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3sdmgehlo.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3mrqifppv.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3xzdobvee.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3lhmrwwfq.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3maqcvbhp.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3fyxomgnk.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3atikcqrz.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3jthcymwv.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3ljjmlusi.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3llpzaqqp.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3wnqkaode.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3hrrxgvjr.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3rncbkuxe.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3dcjoqhnu.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3cskjjlqz.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3ectcndyp.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3fsbbesvs.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3pqeknoym.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3ibtgrvmv.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3dsxqzelb.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3rkapjswo.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3bzzjwcgg.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3afalzkho.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3mbdgkwcq.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3halqcrxk.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3zmbygstj.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3rhtdssvh.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3didrgnmr.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3yzfuxlbv.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3lirnzgje.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3otnxlefx.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3omvunxjo.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3rqkkgxuu.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3bpuryotj.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3frpcguwf.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3gdnhzauf.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3cfvxxwqa.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3rolblxks.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3rxpobfqc.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3jupckiwy.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3cpxouang.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3yonqprma.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3yksvsopx.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3ucrgftsx.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3tpcpdmad.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3qdlhtwla.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3aephspqv.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3ddcuuoty.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3ajvvmszm.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3qcraizes.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3dovirkel.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3cunicggd.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3uoxajtxb.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3bwdjnmdw.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3meueewdw.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3yptynwmj.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3bqrhybfi.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3eajisotg.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3dowywcxv.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3sbtqdtbu.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3rkhteycf.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3oysgkxeo.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3gcgskvuv.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3asefofad.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3dxvjsokq.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3vxyvxtvg.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3jnvfjtbc.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3mzahnmiq.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3xxrsrect.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3pkqkemhz.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3izimhmwh.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3avcynzwp.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3qnnrriua.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3aafdookm.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3gekfhizo.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3vbctiool.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3sijuiywn.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3xyyfzuzi.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3shvnygxh.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3zvfjyefs.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3werxoauf.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3glkhvyzb.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3oirnyxds.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3kqxconyp.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3qlmhoxtq.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3hnoiwjkb.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3odefbpbb.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3rxiydooa.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3kufbghqq.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3siaqsqdx.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3swtwnmxt.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3vyxvwcgh.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3xqlbyxrw.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3nzpkosmy.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3buyddtfu.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3mzbgywpl.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3jeqrextk.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3pumrtxdc.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3zxekvkum.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3zzifmvww.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3epwmvbvi.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3giswqkkt.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3umhfcoop.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3mjduixhj.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3rlwnsjmk.html


<!-- 参考信息 -->