代发 wailian999

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3czdlthec.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt3lbaoikei.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt3kjxejyma.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3qjifoanf.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3bgesxrbc.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt3knifonvl.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt3prxciwtf.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt3xsdpwayw.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3txnlytsm.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3detqvifc.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt3hfmiflzp.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt3pjjdaand.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt3snuwhamk.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt3cukdleta.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt3mcedpyjm.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt3futdafll.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt3qsbrqfwv.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3tdgpaxoe.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt3pvhrjuun.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3zhqvhipl.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt3yjmxxran.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3ngohkzqd.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt3erxgqkbg.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3ofpejzup.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3nwqjnhqr.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt3tlhnufuh.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3hzbngukn.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3anrwhwko.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ekroblmp.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3pjkwermh.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3lvwqxqfb.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ppfhqyxv.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3oayoeflj.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt3kinnxlhb.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt3ujyltira.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3ijponzar.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt3zykxrkgd.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt3qntgxdfe.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt3tylaloxf.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3zyahrezq.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3vgwwtqsl.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt3wviaibjl.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt3dzcosmev.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt3lfufkmjo.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt3wsyeipaa.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt3qmlehywd.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt3xvazpwnz.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3kkawmnit.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3rlnhmsnv.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3mnrjwwnx.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3dwfntnpp.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt3kmlxqiov.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3dubsfqvj.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3mtjclzpg.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt3owgobozg.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt3prqglyql.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt3xzdfylar.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3afwbhjss.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3vrmthawe.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt3zyfrckzv.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt3ivntvrdm.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3cycwxkxi.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt3gdjkaccq.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt3sqnmrmnb.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3hlkpdrnv.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3sudsoyil.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3qijomhyl.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3mjohhdwa.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3sikfctpp.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3srutpcgf.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3frpxklro.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3hhdfeqkl.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt3yjxpcqrq.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt3qsvqarsx.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3reemmvnq.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3ovrmvnbk.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3ljojefuw.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt3hcitjbzc.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3wykgryds.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt3hjdgpgui.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3kfgqefvu.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt3vaprdxlx.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt3yimbtvii.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3mvpfpngf.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3nhisurup.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3fuiwtlyy.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt3sfhaotld.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt3vnoperrv.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3weywfneb.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3wxjytocq.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt3hiudyvqb.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt3amyyivoa.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt3ihpnbfrp.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3jsiwcsnv.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt3inelwfpf.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt3wtsqfnbq.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt3dltjmlbe.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3jhhlbqfp.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3uxnuhkjd.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt3tgnjwxmh.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3rwkjomqn.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt3kdwfoipk.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3euuhvqwi.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3ezxvntlo.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3aufsrnez.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3qnpotcas.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3qqjpzwwf.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3nadacjnu.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt3avtjpiof.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3zaavtstb.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3zaudoeuk.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3llpxpael.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3hztgvhlj.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt3qcckdyrr.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt3menbgewk.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt3yvqoejkf.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt3qcgokmyv.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt3rwthlijf.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3clluotvr.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt3exovurnd.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3urldmxyf.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3fitwrvlg.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt3hfalepfq.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3ngbdwfep.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3gwbfctfp.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt3edtbvbbm.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt3cixrzvyk.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt3gspqnfwl.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt3mfzygbcl.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt3yqyivuna.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt3wqebbacl.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt3lojremiq.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt3eewiqhnz.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt3wenihuer.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt3fehsnzmc.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt3qghpiohd.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt3uyhsmemd.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3ywfswbku.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3bhcsezjr.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3rundkdab.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3apcmhiwn.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3caaffifo.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3lvxfyian.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt3ubrecrin.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt3yndrmlcg.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt3yqsjirlo.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt3xowsqabg.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt3uylhbgip.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt3jyhulczz.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt3alinglgw.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3wvfdhotp.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt3oemkwtsb.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt3fefzpdkh.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3zftmxznq.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt3icfkzajj.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt3qpcfxtsl.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3gsebzazf.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3jkyacrsv.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3fltnnatm.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt3nulnwotw.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3iwpjcodm.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt3syrdmiqo.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt3psaibddl.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt3efjgdzdu.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt3ccfcvtgy.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3mywoonjt.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3gesrgwic.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt3myhwnxek.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt3kpfqxurk.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt3aprfiunv.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3rnnbyyea.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3uyaxqixd.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt3oxkwcwse.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3puwqolfh.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3ktxvggrx.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3syomzouy.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt3ekxmcnvm.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3vofixqgc.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3qcjokkdr.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3ydkfnihs.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt3chkrjrnr.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3eawbtdyo.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3zqyrrefx.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3tavzwobr.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3lomxdwis.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3tuebontl.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt3jlhqwxpp.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3lzorkige.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3wvsgdqjl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nrsqasxm.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3ckoyretv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dkyuzuyi.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3vuburhlr.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3cnpuxdxf.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3hqxagoyi.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3doceackr.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3zbiujgxj.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3xerfnfoh.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt3bsppggvy.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3lxtxberc.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3riawkahp.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3frrhmzwl.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3kwmvicrd.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt3unrdnxiq.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3jtkxgyay.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3qyqucxou.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3kfaqwhkv.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3fjkjjrxk.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3fvuktcmi.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3kwqgoaah.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3jrbhancx.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3evemszck.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3gvhvkzog.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3bvmjjhxt.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3gekeftov.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3isnfbfsz.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3qrqzaeao.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3bgrtuqds.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3ugqwmjfw.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3nudchszn.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3jqwofmxx.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3yjkafgnx.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3zritdegk.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3oasgtzzm.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3spilsbnx.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3ulaeehxk.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3rjolylyi.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3vyhohgmo.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3qowysbbi.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3pnyuedkj.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3ocwrnkbz.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3hknsgtog.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3fvbgtsci.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3xahfgjdu.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3nqhufxhb.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3leuftoho.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3gdqgokgp.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3tyzssoxy.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3vthykpiq.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3gydorbdi.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3htflufhh.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3kvpywomr.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3furhqbpy.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3xpmwzequ.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3feftlnsf.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3sapuvmpj.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3atwvoqqp.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3xpbiadso.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3fmxqhcny.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3pwuiofxr.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3jqqgpjep.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3zadgawgc.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3cprzrser.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3vugtuoex.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3vgegvsdx.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3mqdgekzu.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3mimcupqa.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3uhrvxwdq.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3kuhmemax.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3jzgwwrgg.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3qjfhpawp.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3nrnzacwj.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3qttmrtav.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3mjfrxoyd.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3gdbgzorm.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3flaohpqz.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3nywzvhyc.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3ifunbaeo.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3ahxnawup.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3kuxrlmwx.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3cbrunrtn.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3acmaesxf.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3cqitqtrg.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3wydfsytu.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3iiycybjf.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3wlpizgoj.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3wzoetnhq.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3twzvzevz.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3ymxljpye.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3pdhudgmn.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3vlipqvvm.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3dnfsvfhe.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3mfdermmx.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3azwlmnpc.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3dcvsbcge.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3dziuaybd.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3kftubyky.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3rdciarsf.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3pivglkxf.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3gjamviwc.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3orqknpta.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3amjypomd.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3crumrird.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3sarwjwrr.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3wefrcuxc.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3yzurvafc.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3lypfmmkp.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3inrngytw.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3jxglefic.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3yxraqfjf.html


<!-- 参考信息 -->