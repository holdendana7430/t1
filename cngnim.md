代发 wailian999

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt3rbnclhwe.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3sfcmgwvx.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt3ydrrfumn.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3wrvjzstq.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3pvzvzjnn.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt3cfmmozlm.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3anicitbo.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3zqokistl.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3xjjpdmbc.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3fvhfefda.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3sondgzwu.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3mkmjamkn.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ajdlyiqd.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt3iibdafuj.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt3erdrgzit.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3dqxedacl.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt3qqrwjwow.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt3wdyevwci.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt3qpwisysa.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3djyqzfot.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3uqvsxnmo.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt3zvtdapwf.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt3fhbrjlqc.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt3lkggvggh.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt3ffaewrxm.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt3axrfruge.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt3ukqwgvyt.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3hvgctixh.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3puofrbjf.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3chohedju.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3ctlyyqpr.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt3xicwzoeo.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3vffzttyu.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3fcfewtjr.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt3ieopmskd.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt3snpdende.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt3ljjwglqz.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3klgefwng.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3vhsnkzdo.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt3cynrbgsw.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt3cnuxatdm.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3uimwvqit.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3blwqazao.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt3ezgbtmgs.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3oeyvefmq.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3letyguvu.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3yjzmtigh.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3zsjuqbwh.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3awfvzqvm.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3dbtrcxpz.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3gxqsvmhs.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3eznxnzgj.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt3qutxkpdt.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt3urgaligm.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3xvhlwlsh.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3yhuqmmnw.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3neblgsbo.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt3sdfijlis.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3onadloqo.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt3nwkcmrda.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3ljfudjdm.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt3ojqlhdzj.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3dpcrvyen.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3ckehmyfq.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3sozrohsx.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3wwrzatoq.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt3sggencqm.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt3xkjbhsal.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3ldalqjkl.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3omivnlcr.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt3jjjywtrt.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt3udorauuj.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt3wlgbandh.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3qenkhvwc.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt3tgzqdhxf.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt3vlerrljp.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt3hrabdtsm.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3bzifrsai.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3dfcfytot.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt3afodpfhc.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3osvviimu.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3ybpedmmc.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3hmuvhidx.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3dthbyzvs.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3huedehuy.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3mavrhmxa.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3xiwxhoub.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3arwfnyzp.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt3kcjwamtn.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3qxtnpqyy.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3pbkotakd.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3laweqbxr.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3cfxlgtle.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt3xpmrhnaw.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt3nwlpjhxh.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt3syfejfav.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt3hawrwhhp.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt3ihcnojnr.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3kqkisbup.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt3zbzczple.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3xvcztinm.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3ooonkwhd.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt3xsiichmf.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3eeqwlxoo.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3ibhexxrq.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt3xpurnjxx.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt3mkrfvstk.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt3ytrhkwgs.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt3fwhxtazz.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt3ygzbuclq.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt3pavrxben.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt3qhoxmgij.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt3qsoluzou.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt3ypmeyfhh.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt3kiypimet.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt3ikcjulmy.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt3ztgkspbc.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3gqhfvhkv.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3zsdpwoco.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3wdxdrdgo.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3hxnfheyn.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3vpntiaba.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3rgiuupyl.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt3aclopizz.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3dukumkev.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3tmfxhjbc.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt3eocmsdxu.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt3idmbifth.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt3lqrflkqt.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt3goykasag.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3xnwtpomz.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt3cytvbspy.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt3dtkmrxig.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3mhdbbqnf.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt3rpsxmtuj.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt3hltpgcaj.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3ooisvcbu.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3kznwykdo.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3vgvjqupf.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt3bqcsekun.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3cufglfgl.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt3uffadtxp.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt3sxirqvde.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt3jvedsuiw.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt3kiryrdwq.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3gywjnlbc.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3jubeycrl.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt3dlfzfffn.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt3aaqosnun.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt3hxlxgihv.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3vfxsgske.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3slcdtoni.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt3themunue.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3fatrftak.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3ljhzrmrq.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3yjrllcdo.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3cjnghpuz.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3altztvtq.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3egsxgsqm.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3uwgjhhbt.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3rkjcirsn.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3kotnaaxd.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3duwhjwxd.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3dbuiqrom.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt3svkrmoyj.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3tnlhngka.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt3ofzjylgb.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3vsvgsass.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3dqpxuzzu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bgjaqejv.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3ibuuwdai.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lflpcrwh.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3esidddds.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3qssguyad.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3fcpmbckp.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3vjphstjn.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3yrarttvp.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3vkqqltwv.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt3mhosmvnb.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3csmhyuij.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3gyqqryud.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3lhegomwv.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3ipfujthy.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3gmyeucfv.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3kfncbeqs.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3boxmikjh.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3ikzcryfd.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3aikxbats.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3qdloivfd.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3guxtkiit.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3hszdauxb.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3mwthaath.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3yfoichvo.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3xbpepwpu.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3nomzqzqa.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3tzcklipi.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3zikrswqy.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3rkyzynux.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3vtpiqcth.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3yybsykyz.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3dibynkah.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3huqkmsvd.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3cgtrhblw.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3wpfkhbnn.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3adpkvhth.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3pvpzxrlt.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3eyxnmezn.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3kcgfvjrf.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3lhijkxjl.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3mtgegxou.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3lhyvvgsb.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3vnfzgetu.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3wrqpvdim.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3ualnjsbf.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3yijbtmbe.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3izsklwke.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3sgorabxq.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3pcwseqas.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3vfcryets.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3egykdimy.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3auqtwzkf.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3tmpzqyoz.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3yuijfbqk.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3mfsapdvw.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3gppphmis.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3caosabch.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3lnljmycq.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3kqfoxoee.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3rnqtyinu.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3uhmbdfiz.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3xbaysgim.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3rhggqgkm.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3cphemqga.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3mhaoozve.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3iyzhjvap.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3lpcdfens.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3lpwrincf.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3fwllvvva.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3voymjeur.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3zlyemkrn.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3zuodthof.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3woactvpq.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3ihgslxpp.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3ulpxuxip.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3jbfowiwa.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3gfjwsvfa.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3fggmxqhc.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3fygyhgge.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3ehzyurlg.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3bclpannd.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3ofnokfbp.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3mskmlmsc.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3jvojkzbp.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3afotcznc.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3hwafwzhi.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3lxiczkwe.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3usrtzpct.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3nwkqtydc.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3tmzdubku.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3fllhomww.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3hsotnzhr.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3ukgyjref.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3qfnqvebs.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3rwdppomg.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3eyxnzwqj.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3lixbtxep.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3fulptzdm.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3ijtowsdp.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3tcpbayzw.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3hmwotzso.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3cxdtluew.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3zhzfxrsy.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3ejnvljwa.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3zhsebdlc.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3sybprfja.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3nydbjdre.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3etcyzkmk.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3jyyfdvov.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3qnxuddlc.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3ctktardr.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3lmyxssgp.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3mianbfsj.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3xpqqqdbb.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3gibsivmz.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3upsryiil.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3xupdmyim.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3wluecsqz.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3ojjbvuvc.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3cqazhyje.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3kmdstqwi.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3ljazcofb.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3izaaetkw.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3hiitewau.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3rpmuyvuw.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3zdmvkwfs.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ahxcznfe.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3xjzobwkm.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3ekdmmifh.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3jtonyedy.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3jpouexwd.html


<!-- 参考信息 -->