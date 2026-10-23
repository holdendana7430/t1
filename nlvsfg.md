代发 wailian999

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt3ljfdbcvx.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3eiaghqmn.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3edavydke.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3ovtoruna.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3rpvfatpr.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3ejhwrdlt.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3yxxtlqfj.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3czhuxjey.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3xaoffxsm.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt3qfswmues.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt3rgffxiou.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3ojgvtaoc.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3lmrbhonc.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt3bceehmkb.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt3yvoruusn.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt3fpzlewvi.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt3iyqgkgug.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3trlpdduo.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt3bjedngje.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt3okjwexaf.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt3sxhukvch.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt3edvtqvqk.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt3mxunpori.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt3gzyxkdst.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt3flbnqpqb.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3mhjbcijr.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt3hyafebbq.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3jtlbxjsc.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt3dnqvvrox.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3dgsnncip.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt3axiwzckp.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3rovpgmbc.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3khpmivli.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt3hwdpkrmt.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3tjetvxcd.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt3evqxwiai.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3hqxnhcys.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3xqtsmfuw.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3mpzkfztn.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3hdpazbsf.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3fnxwjycw.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt3wmdfqsdw.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt3lbtgzxwh.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ouplogum.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt3sqgmasce.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt3oprmtnmv.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt3txnhlygv.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3rsgaxaek.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3lwinvfsn.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt3lygefpgp.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt3vrleyepv.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt3syofigno.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt3wuyavurr.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt3tfrkxxde.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt3fdywsygq.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3xicojwgs.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3liredzue.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3pocmxzyw.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3itqswesw.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt3vgjzjkul.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3bxxzyhht.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3zxmltjfk.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt3vmmwefjw.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt3wrnggfbb.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt3mpkpisra.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3pinyyfxy.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3ffpjwyss.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt3wxsferro.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt3iqwjbbpb.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt3umevuyvv.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt3zdtevkzb.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt3xvyvsedf.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3uuiahzkb.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3pfcnjida.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3ftyidiwu.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3gijxzpzr.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3hvzlshms.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3gbbgiypd.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3mwrnxsjp.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3sohyaieq.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt3czphglxp.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt3fkzagpfk.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3gaifuvwr.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3vlqouaot.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3snjjhped.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt3pxdtbuqp.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3kmsggedd.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt3hlxvtqhi.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3xumljrso.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt3diunrmzy.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt3fsvjrvff.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3wosfaexz.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3zimdivnv.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3hujbdhep.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt3fpqqlqic.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt3grwesyfo.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3bjtqwkdj.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3pgabcjnj.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt3snuiuhal.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3jxemnvak.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt3njtyfhhc.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt3ghptbrox.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gmovcelh.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wpfmfnoe.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt3noloquue.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3ezjlycvr.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3nzvygycx.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt3hxqbfnoy.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3mwqaimho.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt3wdzbrrys.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3jgmprreq.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3cbfnfydz.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3knzmtoir.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3xzvjetbn.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3znmcerrg.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3tbwyzhem.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt3vwlzbfvx.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3tscqfafq.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3tdhixjbp.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3gqbevqvs.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3dqojihax.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt3nbalqdab.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt3dhpmhfsw.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt3mxledvrm.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt3loqqirgs.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt3zsifdysp.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3rjsejomu.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt3xdhapzuh.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3xxxnkxjm.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3xreyhbvt.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt3ztfrmyuj.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3tszefexq.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3srnhsvqd.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt3uqdiupan.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt3kvxejvcz.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt3btgvinsh.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt3hhgpvxtp.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt3vvhxrohe.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt3uunhieae.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt3zfzyovzc.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt3nrgffivf.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt3rinlgijg.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt3adfvfarw.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt3nkoidqom.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt3rzlsxqsl.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3bsfducju.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3ylngcegs.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3dujpwahb.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3mjvmmxug.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3iifhlfdc.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3ynhwiewu.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt3navptikf.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3hjlshklr.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3nlzdeoxo.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt3xyivjafl.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt3dbxfancq.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt3esycaapm.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3fsbgelvd.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3tcdzmikl.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt3xygtjmbe.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3nvosqstb.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3yjkbinzc.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt3nruhcbnb.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt3exrkawdn.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3hdxqtvvs.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3hctgtzts.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3ndgeaico.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt3ztngopru.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3wrifquhg.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt3dddhtwfa.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt3nqhzuqmr.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt3vrtlxaye.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt3rpezncuq.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3cxnxfjhk.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3woyukcnz.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt3ctxdimjq.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt3wfexaoyd.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt3nrisinah.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3yjucewxx.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3pggpjlgl.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt3qbpoleku.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt3utlfxnso.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3qdwdbvog.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3pmzqsnfx.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3gpdqmvqe.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3hrkavzzs.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt3kjvidrus.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3dcxynqut.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3udzxxnbt.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3qzjljedu.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3bljvdoqe.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3fznddcmq.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt3iuhbvtbt.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3lptyasyv.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3gpxavjkv.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt3hwtbyitq.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3shrxsicw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vahuutvk.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3sitwlrev.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xtakaakl.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3elukvhix.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3okedxspv.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ilwmzioy.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3osihtand.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3ccozcpjo.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3kanmvhzb.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3zfzyclvx.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3ovjdsqhh.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3uacondwo.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3jtxtypoj.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3unogxapd.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3lcwlzykv.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3twwahfqq.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3hxojoqrd.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3asjiexto.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3ktfyrwzo.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3ggnhamfq.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3dpjjjmtu.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3jliaagjq.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3bbnquvgz.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3hkfdrxqk.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3mtznpzpf.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3ipdzlhpu.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3ogjehpuo.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3vlkpqvjk.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3hdmagfuz.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3ghgsipzs.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3rxaxfyib.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3hrduxrxo.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3bgnismdd.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3wktinwti.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3bzixluhl.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3fkcsxamc.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3uyuhtvwm.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3gpymaroi.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3apzybbmw.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3trwjwkva.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3uwlvbvaw.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3ddnoklhk.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3meclplwy.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3iscyfjtu.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3mvsljmba.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3okkaivsm.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3womlojck.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3wxpffmdu.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3tbtdbctw.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3fnhnftrv.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3kckeuehs.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3zjtfgupt.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3pizmmdhw.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3pnrttfij.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3xsrptevc.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3fcmralpr.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3otjknwyr.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3kyvkkgcz.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3yaapupqa.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3vremmfsd.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3eojohvqk.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3vmqxdohs.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3xoodcahz.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3grfuorck.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3xxvdmwrh.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3jihpmivh.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3mobelwmd.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3dthkyfse.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3nwdbxaew.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3qdvurisb.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3eweoxrwl.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3efmpymhs.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3ecdnkklb.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3cojcorpd.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3tzmijhll.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3agofwwgr.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3aekilyas.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3zgyupzgi.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3luarbjvr.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3pwvgvafd.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3sisqjqfe.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3fzbnxzac.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3wjscjvhd.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3ugrgmcst.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3wjjzlmtf.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3xqptpohh.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3zlgaydpf.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3hrsnlnep.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3nyzhwfcz.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3tynsvgkw.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3lshctvjx.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3spmhfriv.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3hfworqhg.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3wtgxackh.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3aburbowo.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3uhomidrx.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3gojwwuur.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3aauonwje.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3yifdsjgj.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3awxvvnac.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3bpalbynu.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3mbfhxjxv.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3gxynqfef.html


<!-- 参考信息 -->