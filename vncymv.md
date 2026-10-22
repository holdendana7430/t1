代发 wailian999

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt2ukdxprri.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt2kxygxmgp.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt2iasvmtym.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2gikpergu.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt2suhrwmty.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2svmhexlw.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt2nsmsdygl.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2avlvkljb.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2nidzsekl.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt2svnrcivo.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2vjwhvbcn.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2gupsdgte.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2uvpksrzb.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2pcbpqsyp.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2mlmhbguc.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2gkttrcry.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2hjnukhez.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt2vxstiill.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt2mzmqiixv.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2bwmgielo.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt2qoehlmyw.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt2jknyiofm.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt2qpausqmg.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2bgbbhpwc.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2hpmzfpiw.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt2ssdalfll.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt2czkgvnog.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt2phljqfta.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt2kvilkgis.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt2pajrwsyl.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt2jlkvjpbs.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2jalmftlr.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2rjwxceqp.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2orprtjhb.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2uxsnfkyt.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt2ptscwzuh.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2ifeyphcy.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2nqtyqlpm.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt2mvkeklbs.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt2trmtvich.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt2pigvujan.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2nxoufqwt.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2idnodhpf.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt2nhrsewru.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt2ohlybrsz.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt2zmqomtcd.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2irnjhvce.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt2eijupwzq.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2rgbhywvc.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2nihllzoy.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2gdmgcczh.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2cmrujwmg.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2watqazrl.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2qtdsfeyh.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2kkpuecsd.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2ylcfwsnk.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt2rbulhugb.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt2gdqghbkw.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2wdnqnprv.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2qigrssxb.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2hohvcdue.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt2bwgogdyu.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2xsrasdnm.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt2qafqeejs.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2zydktdsl.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt2kbduubtc.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt2wnhvansv.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2gfdfcdlk.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2idnfjbps.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2fsxyqmbm.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt2fkxdozix.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt2udvcngck.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2ngnrvrcg.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2nlkkfuym.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt2qfazufmg.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2umrhijmu.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt2dcteyqne.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2sanjjbrb.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wedceoqk.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2dcbtdgqm.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt2wqijmxth.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt2uqwyoaap.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt2pejpggkw.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt2iqgejmba.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2gpqabfcy.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt2emtghppm.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2wzxhvjpf.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2slyzkpll.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2nplkfozc.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2txzmeryz.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2rvumyrej.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2znnytbcw.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt2rtolqncd.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2ufpkxoeu.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2bzogfnxp.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2mvhgzoiu.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2obkiovdq.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt2umadfjqt.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt2zkrakgul.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt2mglphgai.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt2qvmkzeis.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt2pjlwbnyu.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2xkojqlcy.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt2tbvonslx.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2jqvijtna.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2gwzlugmq.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt2cxuxeisz.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2fnwewxym.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2ffqveoqj.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt2aocakaur.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt2wddjjxcn.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt2lowjuafa.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt2juzbwkrs.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt2croxfkvw.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt2prvmjtra.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt2xsqjffch.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt2kazdqzmp.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt2gmepwsyi.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt2yclozsuv.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt2doomhixe.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt2smntgvkv.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2nfhfdxfm.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2atcoilxm.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2nbqvpvjo.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2lizmfuyk.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2favzmwqb.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2lxxvfiuu.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt2balvpbuo.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2wjmpaaje.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt2zdyxclqu.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt2piowrwyr.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt2numrgktn.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt2vskutgdt.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt2hkkvnavi.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2eldcaaub.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt2lbifinmc.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2drfdmmsy.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2rsljdnab.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt2hpaacyoz.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt2saurogqx.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2bhamohmw.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2bacongtl.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2wwwkbvyg.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt2hngmwzbn.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2afezauph.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt2yxicrpad.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt2rqateaua.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt2sircdewm.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt2dehltcgq.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2asywvnuj.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2ffbsxyxl.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2xzxxsshu.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt2paluriut.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2urwbvhmb.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2iykvjrvr.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2oglnzflg.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt2kzzcvovo.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2zpnnvvtp.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2kcyouveq.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2gavtbrba.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt2xxtxjsfl.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2eokouwak.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2janewwdp.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2kmwrcikg.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2whkadgbo.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt2rqeezezb.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2nexonazj.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt2jmagupbh.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2tlzgwgns.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2gdabecga.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2rayupnhc.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2rfgddyeb.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2vquskmkz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vgvcycmn.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2ecfoyvzs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2norrwwob.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2rmpnawjp.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2hmmohodj.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2alesgqhr.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2jlkraqyj.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2smpcjbwy.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2jstnudww.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2yvsxuwot.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2nwbyjcdu.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2dvjhgmix.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2prcoyxfm.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2hoaegwvu.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2wppynqef.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2fxxjussk.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2zlbzjbrv.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2bguifyja.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2vgrgebxv.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2vocnsvpd.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2kyqrsjvv.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2pqdkdtqf.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2yfnupazr.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2tjeopifm.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2voqpvnki.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2nouyjraa.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2arswjyan.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2rbctotqi.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2yhyyeeya.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2lldldxdb.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2mynxuxnh.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2xujzrizk.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2jhcjxllp.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2guxqojhl.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2kedjolhn.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2tqwftksn.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2mcyugfgb.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2wbazlkmw.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2fqcykvkm.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2vliycagv.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2ynueqvfl.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2utrpzcuj.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2wsvkxfpu.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2gdyjhkmg.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2hsgiwfrk.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2oeoukbwd.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2uumoggmj.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2xfxktnpk.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2ubumztmz.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2jqtqlgfp.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2mzuscnqo.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2flkzlrlg.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2bwhpuqzc.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2lontvdpz.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2sfqouxyt.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2uujjokdn.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2jgrntwja.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2fyqipczs.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2bwkcympj.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2pveolpbo.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2uufxbnsl.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2jfmkimuf.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2fhagiqwr.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2tfwtirtl.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2nfambwlo.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2tqfitpaz.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2ntjjlqeo.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2zoybxdnf.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2iwrwmfzu.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2jtepuwrz.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2wsbfoexi.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2svyhayxm.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2xxxbowqk.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2wswebodi.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2uducwlqb.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2izvdnwxw.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2rqrtmceu.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2tuhcumcs.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2yferdeok.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2mdwxpclx.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2wmooiiiz.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2mzozhhrf.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2qgkteqoz.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2qrldeqii.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2roupmfps.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2xcbphmtm.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2aoxzkxaq.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2bnkldryp.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2ebwtqgtz.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2aaccgehi.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2hcwhmqjo.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2sqfswyzu.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2hgffwwql.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2bequjzdh.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2qljlsmgx.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2lfafhjvp.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ptkhlcnl.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2ldusmbov.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2zymcvuxk.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2atjgrtqb.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2vvquapvi.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2ctenxzjt.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2ugpaklsd.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2aookxqtp.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2wilrgqot.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2iosrnrgd.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2smundsep.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2mvvsnzxn.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2wumgymmb.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2tpxaovek.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2pizsnbnv.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2mzpvpmbt.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2qookrcol.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2fhcpvmpz.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ipkvxxwz.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2cosfrvoe.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2zmvaxtse.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2saqxtxce.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2ffpsmkeo.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2fzvhsqlo.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2isypvsxf.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2gkcepkeg.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2cyqorrpj.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2zwpetcvu.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2rqvarrxk.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2ooaxbuce.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2ksbfowxz.html


<!-- 参考信息 -->