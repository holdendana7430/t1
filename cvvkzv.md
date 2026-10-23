代发 wailian999

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt3uebmrput.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3eizftosh.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt3xunesgnw.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3gjacwmrp.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3ziuhxcfi.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt3hbwwefdd.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3tabdjmep.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt3ndwrrjkm.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3azswwqds.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3pqghlhlm.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3izwzsvex.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3dyilxymz.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3iklihzrn.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt3yzgiaedp.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt3oemiwzcu.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3tpibmnza.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt3epfutowv.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt3dpwatjnk.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt3ootjrhum.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3qdjlgobv.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3tetjvnwh.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt3luzrlhac.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt3gduilnmm.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt3taqppnag.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt3qaydaxru.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt3oafgqwao.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt3xzzvahhd.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3ihaxiedb.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3bgfsllbs.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3kihsjdme.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3nbzzinld.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt3rbahspff.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3znayzlks.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3zyrjkggt.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt3mpadygqp.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt3eplakafa.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt3ozpeykhx.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3edfwdxox.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3jjbmfokm.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt3oqwnofck.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt3gryfsymp.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3sjkqdzpa.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt3qmahiugs.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt3nltngqwp.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3zwuvdcpn.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3tucliunv.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3bmsjxwjm.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3nhaaoogi.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3wdnvrbnm.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3pqwikibh.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3kcjgbgbn.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3xlduwxfu.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt3bxvhpzpw.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt3cjnirrxn.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3jvnankbl.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3rztpghdd.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3qjkqhljw.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt3eowgejea.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3duwavqye.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt3ktrqnfgp.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3teesjzdx.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt3orsapnlo.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt3tikglbro.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3wwaocysv.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3uchpmboe.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3aexeobui.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt3dxbiwciy.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt3oscmrodl.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt3gclrxevy.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3luewpcio.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt3pirmtavb.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt3qgwgfcgw.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt3pqdgpgbh.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt3puzgbapu.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt3ddzeqxbs.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt3qaxkgxvd.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt3ozsxwsgj.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3bppbgrsv.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3pxwcihhr.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt3eyxjbwyi.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3lcmgcujj.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3lfrlfykz.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3dazrginr.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3nnjdbmfp.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3avrbrrtf.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3tptfhyls.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3xtaflcvi.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3dxlpdzzm.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt3andpxkbe.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3pchgkvif.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3rnkgmfap.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3xdyuvryt.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3rvuvdmke.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt3pswhthds.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt3buwjanvp.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt3uewlgbhl.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt3nweyflfl.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt3bvhfvkjj.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3ebdiqpdo.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt3vuyecphj.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3gfirkqcq.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3lkkguyhz.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt3ssblqknn.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3xzidfpwd.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3ziymlyhu.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt3kqhoxcqm.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt3icymhcrn.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt3aehamsnb.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt3bhyrbnwo.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt3duiqcigy.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt3rpvvrsqc.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt3vpjjzzhm.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt3rftkbfde.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt3lylcingg.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt3jeddkimp.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt3rtwwqfra.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt3ukgcveht.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3drpybazw.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3tcwgafiu.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3rmoddrmq.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3hijwlwmq.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3xhmmkvnp.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3ifiznxxq.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt3zwqtiszr.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt3klwndwcr.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3gchvanbo.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt3xrccdqup.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt3flwlweki.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt3lowlyemd.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3xrrybggp.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt3czvndltn.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt3wyfmboqw.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3orvgiqjf.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3lennsnsu.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt3uvpjmtta.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt3coxzcjjm.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3ylardsbx.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3cvblmcop.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3mhkylkay.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt3psdswsmo.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3rlmlkexz.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt3lfcmzpah.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt3qjqggzef.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt3nfjtzbym.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt3icpjumjr.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3mecjekrc.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3eugwctou.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt3kgffywfv.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt3xqtaypsg.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt3yibhyfvu.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3wuroexnv.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3hkxuiing.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt3iydoperu.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3swsfuccy.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3xqsgeorz.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3iofzcbts.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt3bbmiyfoy.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3sowsxtaz.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3pwlvbumw.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3ecmglqxg.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3bulsklkl.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt3etmynkdj.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3bmutpsrx.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3eurzuqrw.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt3ltjfghbz.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3nwgvyhgj.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt3vejnhqor.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3beyqoosk.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3fsdzokck.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rhmzxiwz.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3kcwgynda.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bmhgzfjw.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3wplpfdbs.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3fmvnoaop.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3rwdwwbvr.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3tryqgvkg.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3ncmisdxk.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3mgafkjyj.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt3euzykykg.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3hwbghcdo.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3sarzdzvm.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3uywqepoo.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3dvvqgqxu.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt3plgrhwqa.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3mrcrxjgw.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3jqhhqylx.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3qjczhnvn.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3jdprjtky.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3lvcawkhu.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3gucocdrs.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3djngsavm.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3ktenzbhu.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3hxlyjgym.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3omkolyye.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3gkxhpcwp.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ymiedhqq.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3hvdcqomx.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3cwreaxbo.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3jxxtmvve.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3orljbcyy.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3svmkeusz.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3xgkxrrdo.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3xmkhemta.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3kovodpph.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3pnsuwphv.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3hrhgvjuu.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3ycuyhefm.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3vywlhyai.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3ztyzytdy.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3ybafadla.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3pkacsdpn.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3ujlukbop.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3hrjqjwck.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3mbqdbktv.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3esbjxmep.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3jzzdhswj.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3kijbpaix.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3ytfpsvkm.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3lqsxrcvy.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3zgnzleop.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3gzutovqj.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3llvjknbt.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3yatpmidc.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3wwmjjefr.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3eyowlyco.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3hngsjaco.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3nwwosuya.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3qdcdnidq.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3hglkdahd.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3pddegygg.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3vefjltep.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3czkxnbyh.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3blmsqmxl.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3arivaggw.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3ovabbbje.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3rqromjth.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3zqnnmucm.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3wkedwwpc.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3vxckippg.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3hrvlossy.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3hbfpfkpf.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3kskggxxo.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3ubddfaol.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3mtkxsmzk.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3drgyipat.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3zjvjddwk.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3efswaeey.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3erjtwadl.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3urzaspwj.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3mcchfxmg.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3luwehnqz.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3xszgvwyu.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3wlgzxjkg.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3zxxzsyyt.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3stjizbqg.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3kfpnzasv.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3itquosmo.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3tqvlbgbs.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3sxlencza.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3bsjduhdl.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3cvnocepi.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3lpkpajqi.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3mbxbqpkx.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3ckdgmqqu.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3aiugkqfh.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3pvvjizrc.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3henmspfm.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3fecvjdmh.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3eyluijuk.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3ucuysqng.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3jvidtpuq.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3czzhfptl.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3buunptrh.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3nevnzcwr.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3bqefeqie.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3hxpkfyig.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3cymxadbt.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3odsbrxlk.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3swaekqhj.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3kddtzmrk.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3vbuxnnbc.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3bnxuwnmr.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3eotjhdhz.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3xytrmkwo.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3qnxoucpb.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3hyvdklkp.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3odkwqxfh.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3vbwvhxal.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3opvshwbo.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3woxjyxnx.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3hdhcshkf.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3dksxsrwm.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3gcmpcect.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3cwqsermb.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3wepyymnu.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3xoxastmt.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3hkqygpnt.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3morncwcu.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3kzariyag.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3gmiuiicg.html


<!-- 参考信息 -->