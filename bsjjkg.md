代发 wailian999

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2sczzwbrq.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2msezukka.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt2jycjltrs.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt2sifzbord.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2willrrgr.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2uvqewher.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt2nbjgyqzq.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt2cnuoiyjw.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt2qwziguvz.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt2cjhnvzgi.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt2abpftmtm.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt2mijoidvg.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt2yeainbqr.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2jjxhnzai.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt2edkjuqgw.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2ldbzvxxl.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt2bcesorom.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2jqhcdjka.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt2spanblme.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2knkmnoth.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2dibebwut.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt2tnxldsin.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2yhjfnnzj.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2bfnzisax.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2qnzvpgnf.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2jymllcpp.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2klqhocau.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2lfxrcvhi.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2quqqwkqx.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt2orftynpa.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt2emfnabsc.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ttoxejgq.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt2pvyqvzbt.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt2nktvnxpk.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt2vhzvyxmx.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2djgkrono.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2nmjokzzd.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2rlxpsazv.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt2cjnamkgg.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt2nbjtvgry.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt2azqmvhts.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt2gzaqxerq.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt2raxxiyue.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2rargcutd.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2tsnlchcm.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2hyyhzrbx.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2ratcyopk.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt2vpcjuhhw.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2iljfbelr.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2gludwabh.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt2eqlofmks.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt2ymjhntwb.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt2cltijeyr.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2ukwvdbka.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2ewccorrl.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt2mdxfukml.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt2dvognegm.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2ldvapcof.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2oppeibeg.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt2bywpijif.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2mukdssqh.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2gcruioot.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2qdmfkdha.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2uobtelmt.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2dkbbutcg.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2bhepyuvy.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2bmthsyvi.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2ebkvrbam.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt2kndtmtxu.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt2vwcactuh.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2oxcsbnuv.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2ddyihrwq.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2bnnlxtdw.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt2zuvrlfyf.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2wwnhjgoa.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt2takghfya.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2ugphigil.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt2zkqopqdg.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt2dvpsxnxh.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2dxirahav.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2tvdfxccw.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2dxqujcoc.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt2ttpoelym.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt2kesejlrt.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt2wvarovgh.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2ivqpxkux.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt2zdrxrqlp.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt2ibifihfq.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt2eqhbotmp.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2xmcnhzrb.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt2bjgdiuuj.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt2jndehzhy.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt2dtkpsoel.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2pncdnuec.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ryjlfifs.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt2uxanwjwl.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2ttexqknu.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2gqmymwmg.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2uqwfudxn.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2yvltgyfe.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2qdymrgry.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2cvzczxzg.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2ioklrenb.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2ydtnajdc.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt2bgnlltmf.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2ibryyvfg.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2zvxdbufh.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2xhwizmmj.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2hjsejxlk.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt2zwqngpmg.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt2muwiatxy.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt2vohoawnc.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt2sfbzaaox.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt2enlgouer.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2giukoqku.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt2wodabeek.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2dfhwnihf.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2bkzmmzlx.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt2indfjrhy.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2oeeqeyhr.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2rvrgmjwl.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt2klsqolpq.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt2pbzegxvj.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt2mbanluhk.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt2jtdayeob.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt2brdpadjo.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt2pkajaate.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt2ntekccla.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt2zocqxzii.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt2pgtdddhy.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt2ijihzhiu.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt2advsmghl.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt2mzifyqce.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2agjfxhej.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2erontzwc.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2jwqiiejb.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2cmkhwnld.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2dzndntnx.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2tcwyncsu.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt2lbpbhkvi.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt2bejyuxbk.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2pexgtsax.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt2vrcvfibx.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt2bimtffxh.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt2whjlonis.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt2vvcopmqy.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2jnrcswhw.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt2revzcrps.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2tumpzira.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2vfcpwnio.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2pgmzbfad.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt2siprtgpq.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2ylntybgb.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2gznbviwh.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2lqyqxrsx.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt2swijufdo.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2inzlxgll.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt2vdtjfcjd.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt2capxmmyx.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt2vuvezrxl.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt2nbzacidf.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2byylteeq.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2qdtworaw.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt2svrqbqqy.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt2ddozsajs.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt2mbbhsbnr.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2fnudipss.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2aodyoube.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt2uvlidfqj.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt2naedpaam.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2ydbphvwz.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2nvhqryqx.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2cwloarqe.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2gihjnbxb.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt2gcslcpra.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2iejuamlg.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2ddklbaoz.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt2qcubqqtp.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2ltpykowx.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt2rdswhbsf.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2pfnvmafn.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2snpmnzrg.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2kbjlwzbb.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2dkisgrmo.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2ddmeaeax.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wedovwhk.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2ihoxtasw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vtmvqeje.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2smjzuyou.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2brlqjbfi.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2aebzeqrs.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2pucxeuik.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2mkazkijt.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2yiqrdyok.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2vsjiwjuz.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2snenuqbn.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2zhjzxqoo.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2pzkllxdd.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2aoijxdbs.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ovgztpjw.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2qahmcewt.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2whjsxrlx.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2tmfbjlwx.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2ghcqrmvz.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2bohdtlwb.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2gsoifcsy.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2eyfxttoo.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2fcvicger.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2wojbddqj.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2umbdhzum.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2zytwypws.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2cghajiec.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2qxqbokvy.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2zsstyher.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2wetxhere.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2jwsgecjw.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2taplffqd.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2dpygypuw.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2hqscmvhq.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2wmcymnld.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2ffsznxcv.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2tzfskeex.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2dwypzpfr.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2totwqnwi.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2nnzhqwet.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2gvbwfpsu.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2ccjutdfp.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2zzdhbehc.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2khbbpbky.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2asootdix.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2dwhmesvr.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2imwjkoiu.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2lasdqanl.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2pggehhos.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2orjwwklo.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2ggdhzjhn.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2seudzggc.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2rwkedukw.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2miqkcwnx.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2yozdxceh.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2qfrzgrxh.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2scasjjvn.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2wuetbpnw.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2ecwbirak.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2jfovixcq.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2lakdpvth.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2oijjpxyz.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2lkdovokh.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2iobrkodx.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2bonqnjhg.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2fytwohus.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2naosgivc.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2rebxnojs.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2rzleggcn.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2zaibzfrn.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2wnmeyoml.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2jxsmxglw.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2zxepvnls.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2biulxnut.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2yfyuxgpj.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2dzyutmco.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2btpmofit.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2zumstyro.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2igmatvrb.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2cukqfvco.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2qbqfvfcm.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2ahkscqfq.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2fsksfihz.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2lmmvoaon.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2evuodeme.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2krnvjjfz.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2xugwlcvz.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2gncjsojy.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2ybvwoauo.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2efgxhfvz.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2qituesvi.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2uxracsvk.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2mdbvznye.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2rxkrhvyw.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2fgparxnx.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2mixsvtba.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2scdbfpic.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2jtowrgye.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2owrmfrex.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2gvgyfnlw.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2nwtbsitt.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2mfgmftts.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2atxylnqk.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2qqmnxvoi.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2cwzzqimk.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2wxrgjcef.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2yqnltrij.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2awomzpbh.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2mbrnepjq.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2xbvsainm.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2csgfwzvy.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2npcqvvfi.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2wjtxljuv.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2ojcnbjbw.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2acnnnnfk.html


<!-- 参考信息 -->