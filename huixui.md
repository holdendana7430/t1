代发 wailian999

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2fxgfczzm.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2jlnlunnq.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2tgqwiyss.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2rsmqfdre.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2hxljfawx.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2nvdnhnud.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt2tfiazvxv.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2uflmxekl.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2paetmzqs.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2chkfjzuh.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt2jeqljbzj.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt2numqcdkw.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt2kfluqqos.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt2skqkvgys.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt2kxmnjrxd.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt2nprxmafq.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt2ihupmlyr.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt2jqfvoxyd.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt2yvmdhyxp.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt2fodrkiru.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt2gryobugm.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt2isivgora.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt2aapxhlrf.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2jcxtqvey.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt2cyfesutr.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2enkhuhnv.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt2wgtjeckj.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2tfhjqadj.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2qabuxxql.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt2hdqzewez.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2ceggxgmy.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2khoyykix.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2euhrakwq.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2gfezmzpm.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2njtqmspv.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2mtjxmleo.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2sgnvswwc.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt2iaiubwds.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt2ffowfywc.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2wabtrmtn.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt2rukhugyz.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt2owpmdylt.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt2yavgptud.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2bermjdio.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2tzzyeeiw.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2fasulaql.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt2tqyfbgfq.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt2gtmzfikb.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt2utgqpvoa.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt2aiolwkbs.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt2zewoxrli.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2iehmrvwe.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2uhgepqkq.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2tcxgwugn.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2cusmbvck.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt2hgavhznk.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2tpgpqrdf.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2vcffgvrk.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt2rngjwrvt.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt2vnvvbwgy.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt2waftqzsb.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2fkjfztqh.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2ldumtrev.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt2pbpzgmbi.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt2bflkdmgs.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt2qgamjsgg.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2rlmqwizi.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt2vslcvvlx.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2ffefrikj.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2ffezsmfu.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2sjuufigm.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2dklieqmy.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2qlpvkurf.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2rddusgkm.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2uprilddh.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2zqwmwopc.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt2jvqyruja.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt2ipzwdumf.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2mckbhbil.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2ffrwbfzd.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2ndxelsxk.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt2zellmost.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2wuaanszk.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt2ivnyfyym.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2vsqixmjn.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt2rfffbdlb.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2zqovzafr.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2cxrzuojs.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2vyeslcrn.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2kwdsbmku.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt2wjpyuibz.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt2osydjqyc.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2kwygivyf.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2mcfnvoxb.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt2lpsgjiyd.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt2hesredxz.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt2cyodgvwi.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt2fuhbpouk.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xgcnqphb.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2kuydgmmc.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt2rxzjmlvm.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2siydygij.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zaljhdkx.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt2rbtyhqfu.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2xftwmftu.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2qayyfbww.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2eeclirdt.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2hgjizmyo.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2jkitczri.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2pwlfeafz.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2osfxgryb.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2fyvbkpks.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt2bildplye.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2zcuvcbgm.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2jhdyyblg.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2rizkwmqg.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2pkcvylno.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt2alrsfkwx.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt2ayslakrh.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt2sxqfjzvd.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt2kqsddawa.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt2gqmzhjum.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2ngkktqhi.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt2biflibhw.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2ogjhazwh.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2zqkuguue.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt2ouofrmpa.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2bezzcomq.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2rqdqdgjw.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt2gftaojyx.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt2aytknkth.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt2ezbzykfv.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt2wtbifudl.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt2winbvnuo.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt2swmtbznk.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt2votsldoa.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt2kjollaaq.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt2hpxognle.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt2dojhgokj.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt2algxtola.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt2srzqmplk.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2jtaevuia.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2nqxcbgsx.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2yuvpaqel.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2laggxsgs.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2unlenkqh.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2rmbtyrwr.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt2lygajqgm.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt2zyyhxzyi.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt2auznhbhq.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt2vojqxjdj.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt2nhylylju.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt2ynvpwpfu.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt2vxiyvmba.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2bevwxrry.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt2rjtsmneb.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2lgunnosj.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2qtqxqqyh.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt2nvqzjwqf.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt2lcvehkmk.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2junjowqo.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2wijmceni.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2ufbnvrcy.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt2vwotwoir.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2taoxvdjt.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt2cnyrcmul.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt2gbbmicjp.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt2rvffwsmk.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt2ubmcfkbr.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2revdnckd.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2oujwicfv.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt2omfgcqmb.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt2wkfnlwtc.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2urmxdvej.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2icaeyghp.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2gxjngpcb.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2ndjafhyj.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2kyuecpvz.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2ullygdye.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2jmonvuac.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt2apfnibxy.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2akksnwfn.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2bjbjrlje.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2exihlfiq.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2kyhklsqd.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt2hagcyrbe.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2xhtueomt.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2ubyihapg.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2ctxghnhh.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2dvdxonso.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2bqlrhtqr.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2cdxyqzao.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2eyehdlmr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2oguehnqr.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2zkfdgjhi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2izqixcik.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2tzqvptdv.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2bfbxxjac.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2mnnpppgz.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2xeiglhqw.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2fahdchgm.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2ipdjgahv.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2rjxzatjb.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2mfbthxby.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2abjlltkk.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2elfuimjw.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2ykhwhbvz.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2mfcvdllg.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2xreojngw.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2evtsihlr.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2egcxhpxu.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2pfbbphqz.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2kqllyxoa.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2fatelbgm.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2uvtnjuzk.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2mrakdsqx.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2jhjwfwcu.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2ajnjjuhe.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2jjflewze.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2tetffhmq.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2ngddhdwu.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2nrkboilg.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2optohitb.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2qhekwslm.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2mhcjftee.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2suncvlfu.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2jcwyptkw.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2jbvtkdrd.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2ploedgoq.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2idhdbgmg.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2klilqkvg.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2hdjmxizk.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2dbuvlmav.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2qexhbqis.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2aeslutvy.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2gdrjpgfr.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2risebgzs.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2luqykumy.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2ytggxubs.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2zdjjylmh.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2viizqoso.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2tpwaxjsh.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2tmnqsjvc.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2zsjgffde.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2dftlwifc.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2ewarpolu.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2agppkzwy.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2caasadzi.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2lsyuwapo.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2hlthycxo.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2ycjxkifp.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2xicolhwv.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2debktndm.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2rzymwdnv.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2ifwgcodk.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2ogeivfcd.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2hnkkkrjw.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2zsexhxhs.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2wfzhahal.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2mkeqzzoy.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2hfveeipp.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2rnsatitq.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2lwyhdgzx.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2galhanvb.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2qlewjxkv.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2totdsino.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2iwvapimk.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2ykarxowl.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2pffywijo.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2vcoracbq.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2xtxwqgbs.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2zxauyaik.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2qehoerof.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2fktnaxks.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2exdtnlyr.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2skwiaxgc.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2hqaiqhfn.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2wzhxyswr.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2nphpcmre.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2zkxgevui.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2pfpnbaty.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2xfxxsyik.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2yndainlt.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2kpndijff.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2gzscjjak.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2drugtnom.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2ypsqoiki.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2iwghvdxb.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2hkhfaecp.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2fjyaztpr.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2hbrvkbsy.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ijgcaeqx.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2qjfrteal.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2dtaflowu.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2msmeqxnd.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2sandziou.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2oktzkkwx.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2drcvaohu.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2ypxiqgys.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2mjphbfey.html


<!-- 参考信息 -->