代发 wailian999

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt2whhjqwsl.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt2mawjbzzj.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt2paekpxlx.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt2icfwpspn.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt2recynldx.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2asqdgfmq.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt2srqpbwei.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2dywuuuzu.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt2lctrobrp.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2zdfuulag.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt2ofyjpauh.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2fypwscmb.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2iarsnqra.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt2yjnmcimk.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2fnfhttju.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt2tgtpfvrg.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ieougigt.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2dmymyggn.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2cyorvqwt.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2wtrzesdx.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2lkvwhcfx.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt2pmtjydxh.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt2mtqrvjqw.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2brpgdbur.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt2zptmvhoj.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt2jlisewqm.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt2ljpokxbp.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2kqbzehfh.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2dkbvaxlv.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt2hwypytpx.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt2hrgfrhlf.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt2ncpoyros.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt2vlofijso.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt2nellhqwr.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt2jbinmzbz.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2nhgkovcd.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2xraakjct.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2koltegbq.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2noojjeot.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt2pemibxor.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2pdhbzzkl.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2odbdyxgn.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt2wblktmum.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt2jkcxcdqc.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt2mzyawfap.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2kwkurcmu.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2vdmwbicn.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt2esrdsuyq.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt2ddhjweae.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2dbxpipoh.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2egtayqnr.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt2wdzeigeo.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2enapqonx.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2cbccmxck.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2trgcgybh.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2mwmdyxdr.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2iljvxkrp.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2ouzldrtb.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2ydtauxiw.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2lfupdmjf.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt2rmlrdkcb.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt2avskiknf.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2uvrsjmya.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2kirzjnxw.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2edjrtlwg.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt2wzxudcfh.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2riuwbrqv.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt2vtvorslx.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2rwozdhdu.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt2asmeuokd.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2eporunbu.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2fcdskonc.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2eideaadz.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2wrxpyrtp.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt2cdxyakrr.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt2cgwxqcxi.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt2vwlugsyq.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2ofqmjvhr.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt2vphpjqtd.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2nfiismma.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt2exumlkbq.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt2bdsvajcm.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt2jirfazkw.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hewhxcdn.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt2cpwlmomb.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt2aqyggdps.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2cjdfuqms.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt2kidhalqi.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2mvzvsedd.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2vuupsyzl.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2eqewdnjy.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2nirarzfo.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2lpmsxoix.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2dsdxjzvh.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2smqfylzr.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2fpgaofvi.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt2rvedtude.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2ulukcxrf.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2mcrohgin.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2kngwqwaq.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2ymijmqka.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt2uprcfrbg.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt2lxgovilc.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt2mwkkquyq.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt2twxpvraa.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt2rnfigghn.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2taqpqxec.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt2odflrgms.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2spzlftwq.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2nsyxrnbc.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt2bungsiuz.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2kzcmkpax.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2egtkuxya.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt2hnvohrqe.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt2fjwswgrj.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt2xpmmxgji.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt2opavkcpf.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt2sgpasimo.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt2ypbmzici.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt2zimqmpip.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt2vpzepwor.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt2vyoiubzf.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt2ymnsitur.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt2npbrdpcm.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt2jrudlblb.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2egeskxpb.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2lnuuxbkp.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2rxdikbfp.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2gvkuupms.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2dbiiwndd.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2haibcqwn.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt2mrdcxqxf.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt2tlyyjjfr.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt2xhctasrq.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt2sbnilnfv.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt2vrtzaipu.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt2zzyodnvk.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt2fuixcymj.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2lhgjlkir.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt2ingccpqf.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2wmwjshwh.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2ihcqisjt.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt2bjtcvqnh.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt2tqsxluyi.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2yvpbrkmu.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2crwjuwht.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2lmwfetad.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ledhnxba.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2hfobulok.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt2auoxffjn.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt2wfpoiscz.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt2fzalwsux.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt2ualuodtz.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2aqthjxil.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2jhhxbpii.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt2esnjcysw.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt2rmipsbsg.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2slwbmohz.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2solixyaq.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2gihlqucx.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2pswmmzui.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt2dalzefvk.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2qhkyffog.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2hstgjxbb.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt2wqoubhns.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2jqsrioin.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2aatihbwt.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2ziqcsghc.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2ccalhieo.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2gisemvgr.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2gtoarxii.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt2chhsqyje.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2wonbomaj.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2nsbnhjft.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2fpiolfoj.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2goiqkaii.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2fqfqkkzn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2agubzqzn.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2xtghrxlq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dqipoghy.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2uqahzcqn.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2czcwuluz.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2tukxarzi.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2ukkjfsdt.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2jcuwsmex.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2iknndaud.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2bbxgxzwy.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2pxxylxev.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2nvxhhclh.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2zjvykztp.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2ieybdazf.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ndjzhdxa.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2aaiheluz.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2zzzbfunk.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2lhikmnee.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2igjfefsp.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2brhnlkgm.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2rwzzymuy.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2aautekic.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2wbbjwnpj.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2xrxtjqrd.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2deidowvu.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ubeddxfv.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2zxypqgla.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2yaucqzrq.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2jcobcfwn.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2xcavvsfa.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2kixnhvce.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2ilikgius.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2mxijafhp.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2bseulrsv.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2nkpvhkkr.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2anfrcjav.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2hrrtnpjf.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2mrgpusdw.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2zhymghiu.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2ftkptjfr.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2auygfwrk.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2adtzzcpb.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2mhaajthi.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2bktcflbs.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2uctjtvks.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2epvpzwye.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2jninjxjq.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2ohhshvvf.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2oymgywxz.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2urixqawl.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2xtfnnylq.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2ymlmgnze.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2ydazlfqm.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2zfygcdha.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2ekvwfkue.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2dlmygkdl.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2jgiozasm.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2uvyevbzy.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2giwnfdis.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2orqxnpzr.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2zvdolons.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2cudvjdbi.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2lpcshaav.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2ffdupqzj.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2tqfdioyv.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2grsflqng.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2oivnyadk.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2rzquuxuh.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2cbtwhjnd.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2pqdgebph.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2seaxvqol.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2rerfvfso.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2lsixnbnj.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2hrbtcwls.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2jubkpkls.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2ltbikzoi.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2chmjlmdo.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2hwjwmlce.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2cnzxjafk.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2pafvaevd.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2unezdgyp.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2qhwzvbvv.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2wqteqsux.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2ppdzzgua.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2dsmqdtjf.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2zxkdnafn.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2lmfgkoia.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2vujglrfs.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2astlijjb.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2nauqvwbw.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2omtlvgkl.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2kliytuqx.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2urspykkg.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2ihvcuztk.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2yuiaafhz.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2bwbtemrl.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2altngdpr.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2gqbjdpvo.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2fsfkzwkb.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2tywqionm.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2pzpgssbs.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2eilqgwyv.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2ejawznus.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2xpnrelaq.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2clxvtvdx.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2muvhjykl.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2zrgjvyvp.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2qdmejgal.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2dnwwsorj.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2tqodqsjw.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2adhzwnbs.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2phinceqp.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2xxsumqfw.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2pyfmzoxz.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2znvxanve.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2xdouuaqa.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2davoximt.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2moxqmhrc.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2uthbupsl.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2hticikeu.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2jnymxrtr.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2hkzeeifo.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2rffbsrpw.html


<!-- 参考信息 -->