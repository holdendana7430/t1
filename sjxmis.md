代发 wailian999

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt3ttgpnglj.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt3elohfenu.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt3sxlpjlds.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt3winjfcnr.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt3iecolyqp.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt3eqrfhowy.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt3iwlcspua.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt3loacblex.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt3osawcprh.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3jketxqwn.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt3dgbltyjg.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3fyglvrhs.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt3gmwkqijq.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3xofqlaal.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt3sekptpjk.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3ctinfeqv.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3osbntlaf.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt3ihgxwviv.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3rdpiewpx.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3ccmwexdi.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3knvvyfle.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3lhvisbhq.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3fzytoxdi.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3dtnrtmvk.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3bbtcoihe.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt3fdesdjcq.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt3rjybdwxj.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3ksbpxsyw.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt3iamqxpvy.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt3gocvegib.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt3qavcpphv.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3dugcxojj.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3hnrauyiz.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3ewlqqzya.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt3wnbpqvlh.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt3eqnpyqgn.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt3frixqhoe.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt3isswwacj.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt3brohpbla.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3dgnzcasw.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3gzaynsbe.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3rpugfywa.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3bamdlswf.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt3orqfdtin.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3gbzxubaa.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3bbtbuhjm.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt3fofuukxy.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt3obqhnrpl.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt3zwiungka.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3pfbobjmv.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3kceanarl.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt3ifcgpaad.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt3twozdxbg.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3ehmjpsdy.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3wowbshdw.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt3jmlrsfui.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3lsnmdjyk.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3tdhquuhi.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3bahokkam.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3bzyxjhuf.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3qwldonrd.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3lkzkimgn.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3jdjttkgz.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3oqqkmdbm.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt3bnceoiua.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt3nkweatrp.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3tcfpcome.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3tjgtyytb.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3kodmytgd.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt3bmybqvxt.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3hjdvosri.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt3uhtgrduc.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3blhedgmn.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt3yofjuseb.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3yszbppty.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3pbrszksh.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3iltdcnhc.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3gusxxzpb.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt3xzrxdrah.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt3cozrmnyb.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt3ojzxaikk.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3ykneqvsw.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt3rsflyxam.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3qifoyegc.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt3xbnslzds.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt3vyfmimsq.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt3hyedkepe.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt3yfledasi.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt3mpujyclo.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3kvnlxtse.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mipkqwgf.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt3hphggfzr.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3dgrunune.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3jknwhchy.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3dkqtseud.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3atxgbxom.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3drwvalll.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3xutirwxc.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3mkgtglbc.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3ypvogzaa.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt3zafeyrhb.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3mjypdtyh.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3xaucrzig.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3lgdcqjji.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3fcqlujec.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt3ojgrqprq.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt3mdgrnyhz.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt3zyxyoadt.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt3tovpzjvh.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt3noqlicff.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3tydlwwit.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt3iilyagzz.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3hcoibcxq.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3czgbmyxg.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt3vtzgiepu.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3huvxaqgp.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3zvdekapj.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt3bibzyndm.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt3brkmwbfp.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt3fmmxklji.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt3vtjjdxlc.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt3zzlfzehr.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt3yfonynti.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt3omixtven.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt3zvxegucm.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt3yczbqwoh.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt3qtycefqw.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt3pjobiruc.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt3ejpruohk.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3lmwkckao.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3afmmsnjj.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3qgxbjpya.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3mbyvxcyh.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3pfgivdeb.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3krrtfkwn.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt3kljatlqa.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3smvshpwq.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3farawskk.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt3acnoaixm.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt3thccdkpd.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt3ahwwimvi.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt3zesnsaav.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt3emnttont.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt3hqikwzfc.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt3odvdmblk.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3jaqhmyte.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3yccfhfje.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt3scbhtych.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3dcooaypx.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3ierggruw.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3gwosggof.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt3kgbarbol.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3mnzrwtyd.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt3qtllbtis.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt3yxkzvsmc.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt3ponecdnz.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt3rllokhae.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3qxtmqbut.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3jwfdhfyo.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt3emleuqzt.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt3hxojproa.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt3bfhhltlr.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3gnchbpki.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3ejxhpcer.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt3vvkybuqu.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt3ahkaqvww.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3exvpaqnh.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3juxsesns.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt3hixjtxpy.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3ozcicgwd.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt3vyzhjcvh.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3iafcgnrb.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt3wolbasqx.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt3gvmpjvie.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt3eihuymoz.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3hqqxanex.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3vtwnosiz.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3fbrokinh.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3jptiegko.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt3uvnlqgei.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3bjizcpgc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qnsvtbjn.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3kvdtvcxd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3iqdbnxuh.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3muplqawf.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3xuscppqv.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3htkigsiu.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3tvzyqdlc.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3hxsqyict.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3rksvejfc.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt3ymhlcutq.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3wtbrdjuf.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3pnnoeogr.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3zihhrkke.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3epelafpt.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3hocseyeh.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3gkdlwnhe.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3tvinfbsk.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3cvqnmppb.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3hhjqliox.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3wmquxbbz.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3gwjxjgwd.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3ruchtrqm.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3jmvrbhxz.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3tfjcxxnp.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3mdkcjvih.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3boighwar.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3gfkufrxd.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3sgtesvxa.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3diboqkmg.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3tqhxqxre.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3cjvheblz.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3zojrnznv.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3libllyyk.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3molilqnj.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3ixfnvxzo.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3vleimjal.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3yrkawcpy.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3cnvymrbr.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3vpnxpluw.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3yklavxfo.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3kqmaseyt.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3xhfgtmjs.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3pcsgntlm.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3hbetnzpu.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3lseintxi.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3dxnoiwhw.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3fvxhhhcu.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3bqqdaybm.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3uzehkgpg.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3nsmxkciq.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3iihmkqwl.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3jcygdxzf.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3bwyfhpvx.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3gbjcsycc.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3plmemhqz.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3hfwsspvd.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3lcdvjkoe.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3zrpvlgfe.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3cehmbjpd.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3zprffaiu.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3cppkufns.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3xmejpxdo.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3mioznwin.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3wlpoturg.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3aeonjhgn.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3inmposbd.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3btjfqbkj.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3ccuhalxy.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3tnyzpztr.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3eyugrfvz.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3umnnhllf.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3vsttkkhd.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3cenohido.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3kgaateha.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3vbhwcqjf.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3vfesngsc.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3xjvewmvr.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3twcncqdm.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3yczqhwjn.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3rdmajxcd.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3okaxuvhx.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3udktelqp.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3sphhlmdo.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3iuokhvff.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3hnlqyssl.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3kuklghsz.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3nuyiviep.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3xugvtjvu.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3rbsvwirb.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3nyegkjot.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3zhgfpshx.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3sfknwriz.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3aecqszqw.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3lmrtqwsn.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3epbgxyza.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3fduejzzm.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3kbqttfbe.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3lbdmyvvw.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3erfarovd.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3ivjlxtin.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3lsjkuuzb.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3musluzeb.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3nlupobew.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3qfffxnhk.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3legavuyr.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3ljtpuwxq.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3poifmmpw.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3doyjzhjh.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3nwqznoir.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3vflnbgbt.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3vtbwmoxd.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3blogfoln.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3pyfkdebs.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3jixnmqeg.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3yuldtkyz.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3odapgzvm.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3puhauhvz.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3xbaugftu.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3rzczacvi.html


<!-- 参考信息 -->