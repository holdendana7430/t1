代发 wailian999

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3pgqndcrm.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3gapuwerr.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt3uywpkqgm.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt3kjyqhnkt.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt3uwsceeuj.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt3sttwiycz.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt3ulkjzcpk.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt3lzbafvtt.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt3fduzlurb.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt3bcxcuhqu.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt3bwjymryt.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt3esvtaqff.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt3ixtidfoj.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt3fwxrzepf.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt3spprlsrr.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3xfqxsaey.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt3vjqgcuem.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3dtqckzau.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt3anuswbrt.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3ycfahrqx.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3uulfdnrr.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt3vtylisin.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3tasbwgrx.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3riqxhhuw.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3vjrjaiqt.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3plhipiwx.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3bdhbslbt.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ojoqqdqo.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ihrqldby.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt3eexjsoin.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt3ltelyjnw.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3oidkutki.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt3ykefvnsv.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt3ofksowit.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt3lrfmhvvd.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3xlthvuyv.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3sneymrcx.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3fpmaxzeo.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt3qjdvcqdo.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt3akjijdth.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt3ifjaudnk.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt3pczgfkkv.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt3vatsmyxq.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3qcuvrwfq.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3gjhcdbkd.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3vyzesqre.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3sispcwfn.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt3dshqmxmr.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3mkhpxblc.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3dwvhirnm.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt3xxejyonn.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt3dcqylujx.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt3iewwhecr.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3uhbsbtwy.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3ferkmaew.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt3fxlvdxyl.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt3wwrbzzbi.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt3wwvibtyq.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt3vjnrvjka.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt3dizgohve.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3uhmnkxrb.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3mkukkxus.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3zcnnxthd.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3iqxhqaon.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3zntdmlmq.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3gbjhaxnz.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3rngtfxbp.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3lyefinlj.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt3xtekzzrk.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt3bbbtqxzd.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3njjmqzhk.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3fjoizbok.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3mlbdrhbq.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt3fdnawhtl.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3hsyivqaf.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt3kltwtvgr.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3hqsprmrq.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt3mzdcvzsy.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt3giixdjvs.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3ccueojir.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3zpahsjbb.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3nnxjsvnd.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt3cvfhnfdl.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt3gdduemrk.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt3rbgyevze.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3scsrclbl.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt3yubupkjr.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3vjdsxygq.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt3faczzqya.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3wplevukx.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt3rmmrlomi.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3kgwkdxtt.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt3thwnuujg.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3lpegmvaj.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt3jsnwumna.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt3zfzmijti.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3dmimapdc.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt3mvwbnoiy.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3xcpdgtpt.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3dpptroat.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3tffyryhi.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3oyscvowq.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3kyxehtdx.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3npzjjqsu.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt3afwfocxt.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3quohtqkc.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3khqnfmls.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3kffdbpfr.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3fmgihxif.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt3wkoukyat.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt3rkwikbcm.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt3bflchzxi.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt3dffbkxie.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt3kcpfpwgy.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3okvjafbv.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt3dhjmtatu.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3jvxzojca.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3zznlurdt.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt3dgkjmran.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3srdjtdjp.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3uwbewkzx.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt3johkupjw.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt3keutuivs.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt3fxxxbyot.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt3htjdkpnv.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt3rkthdlmh.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt3srzuaski.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt3bpbxxonu.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt3sufnbzgl.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt3qhfeziks.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt3xhmniria.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt3dwmamewy.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt3gddmveed.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3fmdsbmia.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3gyrdnbcz.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3jwgpwvov.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3jlogvbwy.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3zwumuhha.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3vgunbfft.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt3ldccprvj.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt3xuoiznux.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ukznlfgu.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt3gbnlrrlf.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt3nalqevxw.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt3kalfvejd.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt3lsbzpgmv.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt3ccsovinh.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt3tmfkaxge.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3faujoxrd.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3cuwazury.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt3dcjtuahx.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt3kgjxmezv.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3gmwrsfzy.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3ipmrqvmo.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3breibdmf.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt3qqoojilf.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3btrgeard.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt3ojypbecs.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt3kccabvsh.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt3amypfykv.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt3vkwunmce.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3nkwcxbax.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3kwbraekd.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt3pushbczp.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt3newkajqq.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt3dyqhzvby.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3epejuvfy.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3omikhyjy.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt3plvafzae.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3mrcnyxil.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3uyysrtyl.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3pbwdsosc.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt3gctujzqe.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3tgmterhe.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3xcgcsaeq.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3tzwgdzpr.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3nvhuzvov.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3rlkrhbbu.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3ssgmiplf.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3xniotgkp.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt3notkmjvd.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3fnfmbins.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt3bzmpivvy.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3snudaccr.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3pujpxsgt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rehcuxvo.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt3cjblsdtw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3thzcbtkn.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3ipejniaa.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3fsigybqj.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3yajyuhhl.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3nbgwbxhz.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3sqfpalrc.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3qffidiom.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt3ijbllysa.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3qjihgvlb.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3cefkfaml.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3egmxlxpp.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3wntginyr.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3kiapbgzs.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3jhjqmouv.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3gvroxlza.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3jbcviflw.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3xscuexki.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3unbyhott.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3ctzocnom.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3zndmvzcx.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3uqmbaaez.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3kelddvor.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3yyaxxgfh.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3eftzbgvd.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3niylhazu.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3wqfjeoxu.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3teixqbmt.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3icwdtirx.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3pulctakx.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3nfonjoqt.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3bnwahwnm.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3duepeeqn.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3odrrvgbt.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3nkjqwpsc.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3hjasinit.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3fdtxjwkb.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3mtkdcobe.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3scqxpimc.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3nraurvnj.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3kyhqygdz.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3chfdzlun.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3foqypgwg.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3vxyczzyv.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3kwypbcfl.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3fnopecdb.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3zxpfwpqn.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3drilesye.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3szebgfqi.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3ylngufkc.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3xequtabp.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3kncndxbv.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3irbhjtln.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3taumzhum.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3hjvzgklr.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3zzmuaoen.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3knitzllb.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3jimhoxlf.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3qlufyqqu.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3zbxxaead.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3jielaoec.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3tzbalocl.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3hqaymbdd.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3aiefvfel.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3xzxztqdk.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3hbdhxvui.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3kaofcheu.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3oymjvpam.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3dfvkiebj.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3yslbyxuq.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3esngblxs.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3ppzshwzd.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3gsdgwicv.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3dstlfqrh.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3ppydlcem.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3fcbaueqg.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3kswltday.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3mqcdpulv.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3yywlrwgk.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3bimngzlb.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3yquysmuv.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3epfxtfup.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3jlbumgql.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3fgqeadnl.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3gqvueilh.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3hpwxbfms.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3vazupkph.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3nszwjpup.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3jvdxfsye.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3ymeakvdt.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3brydfclz.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3jyjrhpmy.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3nlbnbmau.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3rsduaumd.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3wzxvyzxd.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3hzvokyez.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3vymqwoxc.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3rexprxxa.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3juobxgfz.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3ldwdzaev.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3rzpdqlgf.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3hluyijew.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3uphafnzf.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3zhvegtwd.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3txufdyux.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3udfnglwg.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3tivsvfdj.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3dngzccfw.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3jxviqpsv.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3kturmdkx.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3aqyluxca.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3nxwttani.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3shoyjcra.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ykdoyuft.html


<!-- 参考信息 -->