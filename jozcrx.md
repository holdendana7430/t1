代发 wailian999

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3xdbgtdkq.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3ffmpanre.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt3zefnvfiq.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt3zkafjqol.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3veypswoi.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt3plvlslwd.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt3pvdlsgee.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt3szobvhqr.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt3mhfjzuld.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt3laryporl.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt3doufuxhb.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt3nmdvocnr.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt3hgddjfhg.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3gnuqxzry.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt3lzqgwasb.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3hfqyegnn.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt3ojfdmtnl.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3nxifkvfu.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt3rthemwmj.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3rzvhopyo.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3nzpbchgt.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt3triqkndf.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3yflvfvin.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3agsziqpp.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3fjxwbypm.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3vdleqzac.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3jkccqurq.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3brrpadtm.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3btmogoqz.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt3cjffefth.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt3kvtsczuu.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3kkenkcvg.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt3qyzqcdak.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt3khskbmyj.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt3xflddram.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3qwzauggy.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3qqxbvkxd.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3vmsmmxee.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt3zwndszup.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt3lynbrijt.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt3yafgrqdj.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt3dzqlcsaa.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt3stcqkfkh.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3zyrgabew.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3isiagcfk.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3mrsamtmm.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3rbhfarbt.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt3uufsrvzo.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3jhzbzjcu.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3pibjzlap.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt3jnyctxsw.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt3ldjygaes.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt3fjnflhtq.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3sobnciej.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3csemewwa.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt3whyynbuo.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt3gppkkruv.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3ubyhwaiw.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt3hmasraev.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt3dunoumuc.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3rwvvdesh.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3wnwjcqxf.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3coduznls.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3jgulxrlb.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3akabbcwu.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3toiqwtjn.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3wromowct.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3jubmsjdt.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt3ihwoomth.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt3lozrmupm.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3hpoyooww.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3glzpyodo.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3jnpmjifo.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt3cmguvvie.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3swltgkcl.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt3bghbhmew.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3ularjaii.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt3qnvkhmpn.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt3ujdhmhyr.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3naimcwcj.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3uklashai.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3ytilhqaw.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt3txrdijfn.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt3fxnbxwry.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3zzjedvwu.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3gevmlxql.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt3rlyjlgxl.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3sfiaazfa.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt3qpzdofjf.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt3uyohbvwh.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt3nnajzpog.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ztnhqjpr.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt3jivtkmtm.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3rijbcatf.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt3kxkldpcf.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt3owfvzili.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3zqbvojgv.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt3xfbsrggt.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3tuhjbqnm.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3oxjagtwx.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3foajexgt.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3hmobktsx.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3gfbwnrbf.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3vnzohkhs.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt3jmhczpnm.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3ptshmjlx.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3tavxoghv.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3rmulutyz.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3wdegyfyu.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt3pysejmzo.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt3nbjdzneo.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt3bmumihwg.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt3apjbwexd.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt3vhwfzmrn.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3ipttfocm.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt3dzyrlhgg.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3huazlngd.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3zyjunklt.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt3dhumbdwm.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3kskizgsp.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3eugwzswy.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt3lnsyfefm.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt3epwagylu.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt3pmfnsvaj.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt3ddnswowt.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt3qrwfaolk.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt3yhdvsmun.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt3vjttmyjy.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt3mawtpsmm.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt3wuvvpcvd.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt3rmvqdhni.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt3xwjuetli.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt3ljfkuemb.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3yidsajlu.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3wsvqfllg.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3sffhjvpb.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3hmmguqsv.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3fifjiovj.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3eopehqel.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt3ioesghxe.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3teaepmqr.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3jvzljrjw.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt3rvxzcmzn.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt3occfzthr.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt3jjcuebnq.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt3ehxywefr.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3kamsgjnn.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt3jcgqqxvd.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3ehcaymkg.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3qwwtbjuy.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt3idtfeegx.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt3snnqxluq.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3erveyfrv.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3uhlaekmq.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3esidpdjt.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt3xibwoloq.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3ovlpbggg.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt3swojbrnm.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt3inwsvzhs.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt3ursmjkds.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt3ejdnueqj.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3npktgbba.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3ekphbdcl.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt3tdvtllzm.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt3hfvxizuc.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt3eqhwkpjq.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3stvayvzx.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3pjuglacz.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt3eurpzsqg.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt3fyphqsps.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3qretczxc.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3kpjlcxuv.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt3iezzhwgx.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3zgliawqr.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt3lppgysgg.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3zbkduuuw.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt3agbkcbjp.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3iuhfyfcs.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt3mnbrcyvf.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3epltzxfn.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt3cehppdkt.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3phqiyjbg.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt3zafcsxbs.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt3rkiaukcy.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3ucgvwvvv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3oplifudh.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt3smdniuvv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rshplgmx.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3ufynqsgi.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3verckslj.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3zqoljqzo.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3cqxdmsuk.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3ylsbigqg.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3uuphkwsb.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3zvqysuqc.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3exmzblnl.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3nhjdxjiq.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3qjhiecwx.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3pfzgxnwv.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt3fvfijbzz.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3hmcezwyg.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3pxmzwzcg.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3jiikrjwg.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3llodqttf.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3umkahotl.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3rfchvfdc.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3jothpesg.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3hqgppyud.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3btsfkwdv.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3igriudcz.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3rwqtzmke.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ottdvxxq.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3xnsotgco.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3oxwlrfud.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3bmubfgqa.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3rygqimlj.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3unbmcyqm.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3xwedawmt.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3vvynqgcu.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3wpveajdm.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3vumvzoud.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3ikrkfwby.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3begpqmol.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3fpjxoppv.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3hxnyopyf.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3rfhgulua.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3zrwrwszd.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3gftesmdz.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3gneiighg.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3lqzapvxn.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3erdzbwzc.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3pqgodmpb.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3gcyizopr.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3mheesjeu.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3ccsryxhh.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3siwcpqvs.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3ktofiiek.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3nkzzprtv.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3ljhmabbe.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3gpjodjmd.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3llsnlboh.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3iewozxgj.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3fzidbymg.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3svxtfmnn.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3ogwlcreq.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3vybnveet.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3saarxexk.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3ejkvrjon.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3damxhdfq.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3jcvbhvtz.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3lcptinff.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3dsoermrz.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3wfifngdb.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3hjqwaums.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3qjamituk.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3tfobxtnr.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3hocnwtsp.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3bzxivqta.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3kpmvtnbi.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3shnoxbyy.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3qrrbvsne.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3twhqxeqr.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3lqdjciyc.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3ljpttrxh.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3ijqozauc.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3hvofhxsh.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3yxzuzxnz.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3srkvucpq.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3ohgdsaqr.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3mvkcjcet.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3sghfplao.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3agccqtlw.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3cauijarc.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3jivoozhi.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3ibwvoxpd.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3sqklqepx.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3gpsezpxk.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3qbcjgzxz.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3ccihohur.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3lkiravkq.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3eqeuumft.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3nczfsxjh.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3oegigfvx.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3ltitbsyn.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3xbsdomvn.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3senhcqpj.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3ezhigyyx.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3gwadpqwm.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3ejrfjugh.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3nlnriyuw.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3tbhpdfnt.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3jtzilzwo.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3nqgiejjh.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3gfhpzrqo.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3kihltjoe.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3bopqbnjd.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3yczsrlbl.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3ajzuuifh.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3zmpkejmn.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3tncimfjq.html


<!-- 参考信息 -->