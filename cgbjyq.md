代发 wailian999

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3vgdsziur.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt3wubuqpju.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt3rlofxwuu.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt3lgqgcxtv.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt3cpjsjluo.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt3undonakw.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt3bttvhkid.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt3sgcukfqs.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt3nfexsztr.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3pgstrunf.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt3pnnvqrcr.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3umfmbnpr.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt3ripzauuk.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3igvsfhgf.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt3xvnnscis.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3hxadymsy.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3tmrfwqbp.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt3xeklscho.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3nnmkdlwg.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt3fkptzaxt.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3qrlwikfh.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3udiralto.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3mxxmivvt.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3pwkryitt.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3lttwcrgc.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt3flgbbxqw.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt3hpnvbmea.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3clpczmnq.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt3agkiblrt.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt3qjwovblp.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt3lkevotjk.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3ibjtkvpt.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3urkvycni.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt3bdhsgdkd.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt3oxphelaq.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt3dbuhfibj.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt3yqhlfdqy.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt3lpruahqx.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt3ukdffxof.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3hslnlohx.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3tinxozqw.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3owqpxzfm.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3vvqdpuhq.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt3qutqwjll.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3vqrnjgtp.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3izbzomxe.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt3isctgtqi.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt3rdbzpmcm.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt3uhgnyyoz.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3czmjdnin.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3obgawxge.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt3aweqnamw.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt3rhlwwgwd.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt3xhbizsap.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt3olbhbbqc.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt3xsnnluvg.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3rlsrpovj.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3getqmvdx.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3zwuaouyu.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3enahyjhu.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3wnpzotxa.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3nmqydkwr.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3vevtswso.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3yzstzmtv.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt3jzgffuuv.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt3fuxxczif.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3uvcxnfvm.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3ncxvumrd.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3lrsopfkj.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt3ezyvvyze.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3sztikqzy.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt3cwbifyuo.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3aenyhwcg.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt3dkiguoom.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt3ueijfjwe.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3mrekkuxl.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3wlzjpvzp.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3kixldgca.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt3rpqxnmzb.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt3hyoitupc.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3ceujvzgc.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3zfvcbclc.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt3gfglmaji.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3hnepifsw.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt3dthjquvu.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3xpiklzcz.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt3mtvpuqzd.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3tfowkfkp.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt3lfgdbcyl.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3nfuszdnn.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt3wtzizpnd.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt3toizspms.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3bhzeoluo.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3vcdwxlpv.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3wwdilset.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3vaezsydn.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3flntpjxy.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3kvppoayx.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3fmogvbol.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3gwzqgljb.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt3xwsvioev.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3vknkvcip.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3tafxzlfi.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3cfyysjwt.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3bgsbjgkn.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt3ayppvsbv.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt3qbwugtzd.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt3ylucljfj.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt3mdlsdedf.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt3iuziyomd.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3gkthznqu.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt3fnpwtnec.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3lypaxytd.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3rejepzsb.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt3fghnbexe.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3acdwauqs.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3iyaeqilk.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt3rcfkmkrf.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt3aknbjvei.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt3wtynkipa.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt3uqsccaxf.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt3frlowtkg.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt3ufukkhzy.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt3bcbiimkm.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt3dsangdsb.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt3chztbhzg.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt3kbomgxeh.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt3ybyljioo.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt3qutipgos.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3zbibgfgs.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3dywaqhup.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3tzippnob.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3epbphnng.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3jeoxgsmk.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3qltswuhx.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt3kvoadpzj.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3hlzambir.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3cvccjuap.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt3tfmbahig.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt3rkqrfanq.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt3gooqlqsw.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt3tejwsixs.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt3zhogdqqo.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt3gziewlhj.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3ulkcfqof.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3rjmoqwsj.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt3vyylbeof.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt3onbyrhkk.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3brvbdjtv.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3sbhefizc.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3azydaqiw.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt3yaldtxmn.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3onweiycm.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt3huzuiqjg.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt3hsdxdlzh.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt3lavagqom.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt3mqqsebtp.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3rizoejrt.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3tbzgnqdo.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt3ifvyibct.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt3wsgbkgdu.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt3oayqrynz.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3bhsgwjvh.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3ficplgug.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt3bkajfrje.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3ydhfqgfv.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3sqhfcmmf.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3qmijqvst.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3njxczmtm.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3rqisphao.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt3lclazqla.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3xgiporpf.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3yncssgge.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3tbvtskvh.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3hoqgpkaq.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt3muzxbdtn.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt3goxneuci.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3dwdlnfju.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt3xlcpvznp.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt3slfgrxhi.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3nvkdakxu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uendxxdv.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3cnuwmayb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dcrrhauo.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3frrmcdtz.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3uohxtggu.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3yakwfpxg.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3cjahqbqw.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3eoiwuncl.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3foruawyu.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt3hxkvcwlz.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3xlwzazes.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3larahxpi.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3cdydzfgt.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3qnipywsj.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ieiommds.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3gynysnzm.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3jcyxawxh.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3swqfnpmn.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3ejjfywul.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3qhabdwaz.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3abxyfwsi.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3eupjsopu.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3xdsxcvwr.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3qosiilyr.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3igohsols.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3gyoxacdh.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3epnstemv.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3otylumpw.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3ocjqnien.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3nntaoylc.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3jrrpvzzh.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3ftxiyodu.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3brvcqrkw.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3vmksiizg.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3gvavlmel.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3pfqzyznn.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3vjcpzorw.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3xdnhackf.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3djhdrxwk.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3quwcewhk.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3wlhqvyny.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3yxkpmgyd.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3wfbwkzcf.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3ecbrqhzb.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3xduvooqv.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3xhlrhnkn.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3dnpwuhgg.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3damjigup.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3qsoncodu.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3ypswxvhf.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3gwlzihcd.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3lfrebhvu.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3appyyosr.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3sopyhpad.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3iyigccov.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3rtzcsrjt.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3jzptiaaf.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3eghyohmm.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3bhkdvbbh.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3oaphlbyo.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3zhhhuafb.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3ptamxcoa.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3ohplplfi.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3grawagwa.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3rnioeenh.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3edllhrin.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3amwxnryc.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3lankmobo.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3jpkxxkms.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3szcknpos.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3hicxzrjm.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3xdziserd.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3dqbrexom.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3xqvlyncb.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3enrwnndq.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3vhexhqrd.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3fenkobpn.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3ddstskru.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3sigmqmmq.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3ktpxaibi.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3gahpvjyd.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3fgvcnzgl.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3ufjtusmp.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3wulezbpp.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3iubculal.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3cavoortr.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3dxdjqzzo.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3aegqnyzb.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3rxbrsmqk.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3qweoiuiy.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3jgzgtaob.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3bwvdqkln.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3zziozkhh.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3idsvwmhr.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3wcqdqpka.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3yamkhdvw.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ptythcee.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3khqdklay.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3gvmhuloz.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3tnjctqxb.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3rcjbwewb.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3uamnzenf.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3hdxguszx.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3kspsaixr.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3euwljutc.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3nushdjtv.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3znnawopu.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3nudqidwx.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3cbidvlsi.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3puthdbmz.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3vzbodwda.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3qpkslfnb.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3hsephrmo.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3bknejcia.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3fhlwnnjx.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3flofctnw.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3vqfbwbbd.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3yffpueph.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3ravanbor.html


<!-- 参考信息 -->