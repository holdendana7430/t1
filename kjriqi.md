代发 wailian999

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt2qrsbbxjl.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2jkfidjzb.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt2oaaapulp.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt2pdfwuhqd.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt2mwyhuxui.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt2wlzceuzh.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt2wirgavfw.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt2wlbuyngo.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt2rkyxyqis.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt2cuyytubw.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt2xzzwwbhf.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2znmidwiv.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt2opwemozn.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2tvgcfdyy.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt2lhswapxj.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2xrwhlzsf.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2htdgdkgn.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt2rzgolbnh.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2bcjetbjl.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2aiiaentb.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2dtsarsiq.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2uqoofwqy.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2mhzpqahv.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2ehwwgnql.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2cbhaunze.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt2abjecrsw.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt2zhdetqrs.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2fmmgfoct.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt2isuonhyl.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt2mdqithdq.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt2qwxrkgpa.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2hcvxkanc.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2jsusjfzl.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt2kjdvdctr.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt2hedefayn.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt2fxrvryfo.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt2mgghpzuh.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt2atotiezu.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt2gxgqkrfa.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2nfwjyiix.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2gqojmzxf.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2paanrqdc.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2symfrenx.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt2sudrpqmh.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2xmrhceqk.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2xmfwxvnm.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt2lavxtbrp.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt2shhpavmc.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt2wzivaoyo.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2eyugjxpv.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2zfhzvcll.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt2jwrodawj.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt2zeigyuvu.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2sbmecqgt.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt2jxoethlz.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt2friicuux.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2xustpvrj.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2knllqphs.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2udxhcvma.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2qhtmbnxp.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2ajdxyqxp.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2wcgkvkkx.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2dzuexgke.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2tgrqggee.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt2tvhpbyrj.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt2aoualyrg.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2olypoemj.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2ypziowlw.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2jkluctvr.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt2glgslkea.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2sbpwsvis.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt2nesnuvdj.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2admxyymf.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt2kzqrsvig.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt2ozdgvksx.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2fnpvitie.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2jbjgckmj.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2owxeqxeb.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt2cvyhtxrc.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt2vdphsnkp.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt2ymjimvbc.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2kxrvejkq.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt2cvfeipqu.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2ggutdvdr.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt2idpiswpb.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2aiptyweh.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt2yotjwjsv.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt2aapnphob.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt2urowymwt.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2bsdxswpj.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt2wtppoebi.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt2bzhbjqzs.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2rsomtdpw.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2lpaalpmd.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2musmsrlu.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2hiirtwyw.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2cwhldtvf.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2feppdnge.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2ypldnvnr.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2xcqtfecu.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt2mpuozauo.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2fnesjped.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2tacslkyh.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2ybonbrrn.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2nnpebagq.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt2gulrvgrs.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt2euxspkjr.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt2egltnwle.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt2kjnnrnyt.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt2wdixylxm.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2assfcwpw.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt2nnlixqyg.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2swvucqij.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2yyurtctl.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt2hyatvrvb.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2gtyzamza.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2xbyneppa.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt2ltyqjcpn.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt2jqvpqjuw.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt2whfvpzrt.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt2xkvynmys.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt2hyxdtsnu.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt2llqmwija.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt2rsrvrhqs.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt2ahpbyozc.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt2naoxkmxs.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt2pbgjaofq.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt2rghmaprr.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt2tqtjcwyj.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2evbwmgfm.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2zrypjpuk.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2zzjcuhma.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2ngfbqiyq.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2nczujpka.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2mwoiaare.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt2kfotgaaa.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt2obkrqcax.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt2opnuveth.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt2cejsktxi.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt2kwcscscz.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt2ywdehmll.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2woajwtks.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2yyfrajyc.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt2jmwkatke.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2wdmikssj.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2gujjwnqn.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2dmxcqnwo.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt2swdreqoq.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2mbedazmq.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2bcjsnywc.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2athcjbss.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt2dcxjadza.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2qfvadxcs.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt2hnblvwqx.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt2uurjkfnh.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt2mmsuswbt.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt2ztxjougi.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2nllqdwpt.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2pyfsqbdu.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt2jxrlwpnb.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt2cframcuy.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt2tthyjugc.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2yevnuwky.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2vhdytcbg.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt2oashajhd.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2hjyucpxj.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2glosmivs.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2erwyhcpp.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2zskhccrh.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2kwveqwbm.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt2ilgbcfzi.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2rzynrkrx.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2qlapdpyi.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt2nmzxctqx.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2cadtfpao.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2odjfzten.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2poaanmtk.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2ycivhozm.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2ekvbgknp.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2vvsxlnsx.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2qtcvpgro.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2syssgijg.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2karnkimb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mqfntinn.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2jezcvqze.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2diptaqls.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2capemcwk.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2nkljvpoa.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2kacgjgda.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2ocdflfjd.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2yjbbmlwf.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2cxgavvsr.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2ymqttist.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2nohxutwf.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2hfotxzxn.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2ajztarzm.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2vvykwoky.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2npwcxedb.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2kygneycf.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2rcnpkahz.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2obowzpax.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2uzwhhtbk.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2kdkkzqak.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2ukdmhaja.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2ifyocxyl.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2uvqeqsnp.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2fzmdgans.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2vreemaci.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2ruazqbwd.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2fntfldxb.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2oyuyxllv.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2acvyaluc.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2jlejdbnj.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2kedhaxbu.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2zzrptuwb.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2bysyyqfg.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2hiandlee.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2eedayhjq.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2wjiasazl.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2imgnwuzk.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2qkuixdfs.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2fwzywnhu.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2ihuztegy.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2mldlhoyj.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2lowydlnp.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2lrjqcwud.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2rwetjkpa.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2zwabskqt.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2vodlxbri.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2cjmuqegd.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2nrluqvzp.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2wyopicpj.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2ufiinwki.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2pbxfcogv.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2sipxotcd.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2whxleqwi.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2yfjmbhvn.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2dzwbqcrt.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2dezjronp.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2tfrytahg.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2gdewfdxm.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2hrabntao.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2xapxmppp.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2mmczgciv.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2anndxmys.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2xvoimzpn.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2izyzbdxq.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2weipcfkg.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2kewqzgjv.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2lbrpwbkc.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2jgtdlofl.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2sotdxlnk.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2wydctpma.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2rmpdkpvz.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2aywnbxwl.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2jizompar.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2olvjggar.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2akiawhja.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2wqiogkfw.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2ptanmekn.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2mhnpfwkd.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2ghlnxzkv.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2fwciesgx.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2jfuvvrbq.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2ccjlmfvu.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2ihifgrxq.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2jijvpfjs.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2gnhnidyk.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2emxztalb.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2kjoanjgl.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2ebmtwsxy.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2ewyfytkk.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2uqzxeqro.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2qqhjllph.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2udafxjwx.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2ldtvmzir.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2vgxrqykh.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2pfjoevrj.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2almswttv.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2kynzbjqg.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2dalkvmhf.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2okndygkk.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2lajabsjd.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2nlzlbqny.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2xocvphfr.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2uwbadrfq.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2jgbsrqna.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2livtfbkr.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2ttjjvkwk.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2jmlhzjss.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2gqsbmgec.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2nykaoxeq.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2lftgrlof.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2elkmleah.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2gxqqxsoe.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ovtqruns.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ctcxqmas.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2oudyuleb.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2tlnefbkd.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2wfybwwlx.html


<!-- 参考信息 -->