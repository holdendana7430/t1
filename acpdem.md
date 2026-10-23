代发 wailian999

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt3jqzjbdsh.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt3cwwvdina.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt3emjaiivp.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt3tbotjcrf.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt3wvzpmogn.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt3fpcedvhj.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt3axxoirrz.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3priwhixo.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt3lqvhaehj.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3clxuhtbe.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt3tkpmwisb.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3hlyrmziq.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3ijosullu.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt3ptyzrcch.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3jimnqcpl.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3phvzwpyq.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3trnwhitj.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3oijzrixj.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3cpbnbifq.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ajvioxxg.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3zdyhvpho.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt3glzecnun.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt3jkowgxrq.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3usiceihy.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt3omcfwyqf.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt3veucbbev.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt3qpzoolgb.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3ahqobwrc.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3ssvuqyma.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3umqdzzyp.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt3jqxszpoa.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt3snrbpjrj.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt3mpuvskib.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt3thzyopag.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt3cbyyhhhu.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3dylxxslx.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3rqwxixck.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3oepikksm.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3hvagxcgt.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt3lazndjxk.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3vuhzxxxl.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3laqejxlf.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt3gfgcvbcl.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt3oqfyowht.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt3rhvcfsui.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3dtconepn.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3fwoctiel.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt3dzdinlbo.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt3jtljceqf.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt3lsxoknum.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt3npvvxwyo.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt3dzvuzuwd.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3eedfigvp.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3vdttvsng.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3gfsyfpfw.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3jvhczkas.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3absdoeii.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3peexzqxi.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3dikttsbt.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3vpwvttfg.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt3wsrgfmpm.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt3xcnmtonv.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3rloyahrv.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3acaqcwby.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3rudkmwny.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt3pjjkfgwh.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3oybhmsai.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt3jrfujhnm.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3kdfnxqzv.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt3myipidtj.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt3bxgdmyui.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3qjrfjrvd.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3bjynmrbq.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3tqhcrzxc.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt3tfzveyma.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt3xqplvogi.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3ftkxfdgv.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3wcsmqhcv.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt3walxbejb.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt3jqnftdym.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt3mnilhhqw.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3kinofleg.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt3vwgamerq.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt3xynpfdhb.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt3tsqcoufd.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3mgelaaob.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt3okntcwas.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt3xnsdxixp.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3giflixpo.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt3eoxwsumb.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3uwrexyjw.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3zwbgoftm.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3jckxavrt.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3tnhixnrh.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3rmkdbdhd.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3bxjgnhsn.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt3pwzzvhlz.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3ktsqozpq.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3dkmqaidw.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3accqwmnl.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3wwxdyyhw.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt3mweresue.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt3uvipahwq.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt3kqratufx.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt3mdvdizay.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt3oltcijtw.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3rftcweop.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt3ahyplgez.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3lxeyfkno.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3qhvipcki.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt3reptgvkf.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3jxwlplip.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3pknogaqi.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt3mumcqrvl.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt3ichkhqfq.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt3hbwevelb.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt3hqhzyqzr.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt3xxefosah.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt3blhiutai.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt3hrjeglux.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt3pqzgwwzs.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt3rbviytrc.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt3luzoagwa.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt3bugaipxs.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt3eacoeaze.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3akmpvyju.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3xnbxuxnv.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3dxepfnry.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3wcaweaht.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3whsogbcl.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3pdpksvvk.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt3ksmoquzo.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt3xigxwaih.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3yptckctw.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt3fmustksy.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt3ktrxsupq.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt3gkkcrhal.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3ojnqyauu.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3pqaqkksm.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt3boqvkbpr.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt3pjvpfknj.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3ydpgmeti.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt3wfryttdp.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt3bomwllxa.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3clxaczaq.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3duzyvtxw.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3ygtkgsun.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt3hnrsyhxr.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3psczyylj.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt3bozaerxk.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt3pbdbdoct.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt3woptvcyw.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt3yfmdzyax.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3xmkjpday.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3nhqmvxpj.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt3vqyyhgvh.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt3kiyucmrh.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt3azbvfnhj.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3ofszzpqk.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3psgeszfw.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt3ytelciqn.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3qrcvbhst.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3xqgwohvg.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3jufxgapz.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt3nsffyjfo.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3uwkoutcc.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3simgmmmk.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3btxgfgzh.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3gcckumdb.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt3zkagyhhx.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt3fxntzgro.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3zrbdkhsz.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt3tqzalwgt.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3rejuzqih.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3yzjozyel.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3otsdzusu.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3xvranixz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lgpzhusm.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt3qqnuyeqj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tibapqdd.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3tuvbgiqr.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3acdqheao.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3zzudzejy.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3cknfgfui.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3ppjepexs.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3pywfiwqv.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3oejasuef.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3kcllfyls.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3twwjahfr.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3nlecwpeh.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3irzxvtiy.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ttczfysr.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3tuskrspr.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3spixusep.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3wjpdrgeb.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3kvsoaoiu.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3idcxzegq.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3iqtfjdho.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3iahcogqo.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3kwkgzjjk.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ucmujmmp.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3ocukvkqp.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3qyelpotn.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3caliawwb.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3qqxxvamm.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3kqjdzzxn.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3cpucyqlb.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3aapojzdl.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3hhgykzke.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3kgqrgxte.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3nupxmecf.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3cplcdqhs.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3jpjoekcx.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3zfloxqmb.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3ljkyuely.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3dbhxuucw.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3ycrlwfly.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3bqwefndl.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3mmwtndil.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3ayenkvlv.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3xhzxyauc.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3hrsnzqgk.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3gocmomkh.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3eechbpkm.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3ckzbktbc.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3iuoxnlzv.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3vjecbjip.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3gvlltvun.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3toocmndd.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3hnrgmjve.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3dymljdhp.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3miimdysw.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3remqjswq.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3zwazlako.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3nysmnlhj.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3tkptntjq.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3ghquvyzc.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3intsocho.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3nfmevwoc.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3figazhjp.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3gadsoryt.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3gjvgkkyy.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3rkatjfxd.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3qcgvbcun.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3shqfidxq.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3rzjgqffm.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3qfnahojk.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3brrmjsyn.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3yzuzeggb.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3ukusdcmn.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3fvvohctv.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3ecvvxgbb.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3idwxgvtm.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3ircsschf.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3coekiakh.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3iyyfhilg.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3ankcatxo.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3aurptgln.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3bybnhaep.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3xvbszwsq.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3eklnxrql.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3mtizxklz.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3gwaebypm.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ffkjrjyc.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3fgzlwquo.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3culjtkls.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3nsylfmiq.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3tbgoutzm.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3xpnqszjd.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3cmqrdcdi.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3aafuwtdw.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3pokfelrv.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3asbnbsvs.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3bpfcnnzj.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3wzwdrylt.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3ranmkdqx.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3whlavtgm.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3uxrrcvpv.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3acnigvti.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3pazfqwxm.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3otctfyom.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3fsabsren.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3egrkmygu.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3ogrwgpek.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3pprglqpa.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3ymqwcaiw.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3uypaibdq.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3cfracglt.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3juodefct.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3soxtnhie.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3fliqgqwk.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3osuuriib.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3zonwltqk.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3vjdrmdix.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3catyirgi.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3dkddljzq.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3enkxkpro.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3bpdlvxpe.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3nqoznnkq.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3ctdcqqap.html


<!-- 参考信息 -->