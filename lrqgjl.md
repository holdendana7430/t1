代发 wailian999

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt2oapcmrae.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2oizjhewz.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt2fmwudrkq.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2ipgjgtpj.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt2kayhvaev.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2ltbfujfj.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt2vzdbnbsq.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2lgrpznml.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2znpnqvge.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt2zgwflpwo.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2ifkopwwc.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2ggmftgfs.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2udtuzvht.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2tneavart.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2fnhtwbnd.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2xemuaoqt.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2yctsbsra.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt2glmejhhe.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt2podnmmfy.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2faznrzof.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt2htrpbmbw.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt2opxaeclv.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt2rqpbqlpe.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2dguqhbbi.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2pfgmkgyc.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2rllnzisl.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt2adynlwmm.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt2vlypieda.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt2qfxacjgd.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt2phkdbvhv.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt2hwrmxlgc.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2gdusyjwi.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2ockuaifc.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2tcfxymax.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2afbbnwzg.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt2uqtofkff.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2naskatlq.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2oovthuke.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt2iihdokcr.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt2clryhloo.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt2usdwkaac.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2bxdiolyx.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2hbzsgsim.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt2paxbiays.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt2twsdahid.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt2qluhaddy.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt2nfegyjou.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt2uabeofzk.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2ovnljvfd.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2bpauaxls.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2efwsxbat.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2tjkdgehy.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2kdwvelen.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2urtviuaf.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2nkvytuht.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2khjyggjd.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt2ndjehshf.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt2qhknggcj.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2ukrvflcu.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2nxzytvpx.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2dnwondpr.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt2jszfldea.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2vccqeoqw.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt2ahpsfidg.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2gpweqvaa.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt2runjpcpv.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2evshaqed.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2ndtuodoz.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2wiqobejg.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2ljreztco.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt2zpjikzxo.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt2rnrmrmci.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt2mjuhltuk.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2jjcbbjru.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt2ukwxpqxj.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2phbleqiz.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt2kjywjqpz.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt2qmiusqbz.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt2tqigowut.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt2jacxuggm.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt2rgfkdvvy.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt2lbpgneru.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt2mrwokdro.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt2lrvcualv.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2esuiupdo.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt2fnnqzdjj.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2kermowrr.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2wuctmazn.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2wahpbkce.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2yvsrvijn.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2mxttslxa.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2xycfqxgi.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt2lrhofdfv.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2tngairru.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2toidbiku.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2ztnwtvvi.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2eftqcfba.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt2jzpvgeuf.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt2bwxijojs.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt2iavguukw.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt2gmvkklgo.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt2lhxwsbxl.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2ncpzoosx.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt2qrravsbu.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2abfxrcyc.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2taejuvsk.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt2xodnfjxa.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2xdxticku.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2gfqpuzeb.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt2tjegrhoj.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt2ceumafrw.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt2xdurdirc.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt2tvrdezbk.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt2bojzhrcm.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt2yqbcyiqk.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt2fhmcglcl.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt2wnuqodnp.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt2mmuizcgq.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt2zwvndweb.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt2ougqcemg.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt2cgocykdh.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2znywsgmh.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2twuwulbh.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2dbyaeupo.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2zspujnup.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2yqokqtit.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2pykyfpke.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt2ihcsimka.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt2mmwnsgzv.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2edzhzgke.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt2njgbtrxf.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt2hpwyjmkv.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt2zhioxwbf.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2nazpbaml.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2hthlfsxr.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt2husgvysa.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2uvumhvfu.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2zrfpqufq.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2bqmvfgna.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt2ahpmsnaa.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2tulhojpi.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2ficswmjc.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2toqccfgh.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt2uafkxdbn.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2fbkompwf.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt2zgftnbgr.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt2xejavzzg.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt2jmnibkoz.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt2prufugtf.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2anpupyjd.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2mlhqkyoh.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt2xddbcyas.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt2karntlmb.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt2fcifqqvv.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2cntwvzih.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2dtmsdzsd.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2zxljddip.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt2tekhpalb.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2xkbnlxse.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2jddrnxtz.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt2qyqkwhnr.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2szmklbjr.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2yuptjsyh.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2zezwramg.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2mpdxkofi.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt2vfbgyjgk.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2srbemxrp.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2nhryaqzx.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2fifzuzxm.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2jpqwsjox.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2fsebsnib.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2zqbrlgdd.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2gmgowmpi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jleboxdi.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2rlqjtkgh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lxxovpqz.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2vhkfnonh.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2ivugntmq.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2msqehtql.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2shqcaegi.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2rbvhtmbl.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2bqknvxrc.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2zbrjcugq.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2luboaugx.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2iugbupxw.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2bjephaws.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2pqlzkrky.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2ywygrpzi.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2cjotmlob.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2yiopucpx.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2nubpykde.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2qpfdxdmk.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2mkhdtonr.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2creafqiv.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2nrlinilg.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2cugecdqb.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ufbuwshr.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2xwicusaq.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2xgrdaazz.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2eysckukn.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2icovdarn.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2bfcvtdpq.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2nefgofsm.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2hmdakypf.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2pekwnjaz.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2tdoysoei.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2pzaqghwv.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2qxoznvpj.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2cihhcjxd.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2vyhgwhyu.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2qvgokxbr.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2mgjkmjtn.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2opfahgkg.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2kdomduit.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2gsyvygvn.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2bqznaxhp.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2qrvbqwqa.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2hqtobxfm.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2kotmzakd.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2yddkctwd.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2eazfjyzv.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2hmmkcbcd.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2zoezvizs.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2jyyicgcf.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2goonbgyf.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2gdtxbrks.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2ukphhjrj.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2dfljwptd.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2nlkiwtjk.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2gcyctmfb.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2aopdctjy.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2sizjfgrg.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2nxxizaio.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2thgyhyww.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2syvytfiu.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2vmajwaos.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2utztnjkc.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2sjmeabna.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2qwskegcr.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2yovplviw.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2vleindoh.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2egghginr.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2vkrurvsc.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2wmbqqlcc.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2akpthpvl.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2eephvsbl.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2hwsbusud.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2dfikvxjm.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2kfhrzosv.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2dmbcrtas.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2efuolkmy.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2ggeqtlag.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2tgqlmpbg.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2etgiuikc.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2zualkkhm.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2btcayfjk.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2zkvmzkdy.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2xokuhcey.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2fsczmskv.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2yebymgiy.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2jtpzonaw.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2vbghsbbh.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2ywlehuql.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2pharwzli.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2hmimebah.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2gukjrqzw.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2rrgkgetr.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2jiqsuwbf.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ikwfrzem.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2bmuntrcq.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2xbtnjqsz.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2ikmeyjnp.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2xleaxkwo.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2fggfpvwr.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2vcrbhnfa.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2jvcvwexw.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2gxuuxhsg.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2sbxaossc.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2ewqomvun.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2yywvpbxv.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2astpwtbr.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2mourapua.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2vblbadlv.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2ktopktzh.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2gudtueri.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2nbtrjbvt.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2azgnjlmt.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2rtubuksv.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2mpqgujcq.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2gktkrtgy.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2hvrdvogx.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2bfouizey.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2gpitcvri.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2qvhlipjp.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2frzqvtns.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2ttmdbtii.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2mfydgaak.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ihvavijs.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2xkbsfjvu.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2giiwwaeo.html


<!-- 参考信息 -->