代发 wailian999

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt3dyeetqbq.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3kgviubnu.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3pmdqomeu.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt3gaayvpri.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt3ierfkoxb.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt3qpqkaenn.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt3zwylsraz.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt3mcrjxdpx.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt3xqokxwtz.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3gmjdllhz.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3perfmeei.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3txriziei.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3pfdlfcpn.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3pnibjldf.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3omqyymdt.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3vbrqvxcs.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3mjbnabvc.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt3fvyxkzjs.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt3dmpjhwjn.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3xhakbtcs.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3qmmsqkds.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3eomjracr.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt3ufitmsec.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt3ngbebpym.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt3dzwguiab.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3fzphgent.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt3hftefewz.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt3stzxgrni.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt3wrjwsmoa.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt3dvbpezrr.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt3iupufamp.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt3zkfmscgu.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt3dgqxkcgs.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3zfyczojs.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt3eitzrxwp.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3jozykcmw.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt3ztmuhtne.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3pwdwtkvk.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt3obvvopvs.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3ecpmnavz.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3cyrkpbhl.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt3xxkzzuwp.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3qxvndcil.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3qofhfkbe.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3tkocrqrl.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3rzfaueou.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3qorngyvx.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3eukgbunl.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3swevqcpd.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt3cyaqjizc.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt3igldskht.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3zojsisuy.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt3mvyfvkqh.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt3snplobkr.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt3mzwoluio.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3sczjcncr.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3axtffwoj.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt3sqsizikp.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt3mqfsfbgu.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt3gpanzlnl.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt3ftrvfoml.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt3gcdzgwvm.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt3pkznmtkc.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3pildekqj.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3sahacvrc.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3ttfbncxj.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3oqzcnxpc.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt3yfcfupit.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3yuxehslj.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3psqpxfmw.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt3nbthkfkv.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt3vlbhkejf.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt3wnhhkyaz.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3blkolhyi.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3yaukcnpz.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt3uktehfzw.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt3nkcmtnqt.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3uepfqsob.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt3mdcskwds.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt3cpzidavx.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3zwhmvyut.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3sspggzym.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3vxhqyzxt.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3woefgtym.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3dwzpnimv.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3yydaqlma.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3rnalfqqk.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3nlsfeczc.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt3jjwdkunu.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt3xymbfguk.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3ipbtdcen.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3hbsnnhkk.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3rarevnto.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt3jegmloku.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3sjhmbced.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt3sbvpddlq.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3stijcwct.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt3qrlsievn.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt3lyjrvyax.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3toendvdn.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3flupyjmc.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3yewvdzyq.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt3hawmoszb.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt3zjjrdwgu.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3cxavvbwo.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3qiurttwd.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt3tpjomhlw.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3rboyfjnq.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt3rofglori.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3fewmpkdv.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt3nvatpyja.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mzmmyzgn.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt3dgkewhja.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt3czrclnvk.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3yocsfxub.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt3bvlnsleh.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3eytcyiwb.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt3iqxicfhn.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3jnpfijse.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3vofwyqnc.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3gxndcmmr.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3wgtsxjay.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3cerzuvvk.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3wrnphuxa.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt3sopjjuyt.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3rodvxops.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3enptmdxb.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3aoblfshc.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3cxgejwxi.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt3ffrnzclc.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt3jwrawjli.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt3qmuoywwf.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt3eejxebyi.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt3felydoul.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3nkuklctx.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt3zwtzxtsn.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3lzdotvpl.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3kdbrwwux.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt3wzqjitce.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3badgzgyj.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3olqvizhn.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt3tbvgxyyo.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt3ybddhnov.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt3abqrqtik.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt3srsdgdig.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt3cybzjgle.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt3yclssinw.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt3oiqahikt.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt3jphbkvgx.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt3ljfmhseh.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt3rysqhhgk.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt3yfxbvumo.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt3zhqnzvke.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3lgizbenl.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3cayktquf.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3rrqlcrub.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3lsjtonty.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3yvhxwbuc.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3jeaocejv.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt3goruirfe.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt3wgcxypbm.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3wqtvnzzj.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt3sacbmnww.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt3rvlakdts.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt3vevaqhcu.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3vcwbdmqj.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3uhfzmofn.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt3fgxppixk.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt3pbemwsaz.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3drsrunoh.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3yhcffxfi.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt3hebzlcag.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3epmtcbsd.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3kpedothx.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3krrwgklw.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt3xassbnzi.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3rdzivzej.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt3zfuxyxou.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt3ohmmcdec.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt3anltgzpw.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt3ncqubkuz.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3agnqgvfj.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3iccpezpo.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt3kwossija.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt3eiewewtj.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt3zezqgkae.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3rupnbzue.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3vzabodvw.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt3kaklamgf.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3dxqebyla.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3tgzneafe.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3ydvmafgl.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt3qynphojh.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3ioysfwst.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt3ixyipkuk.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3gyxbyrto.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt3xsobwmne.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3cnjqtnip.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3suochgjb.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3byhcxaqk.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3vuifjjsu.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3jpllflen.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3bdstycnm.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt3ymhsjygq.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3uenvznmn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3swnwwict.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt3seoukgfn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hjeqhrfv.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3gkbyliuq.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3hnrrlltx.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3tpxmbper.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3xuaivkro.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3arbpfeme.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3zmaijuzl.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt3heleyuzy.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3wqmdroet.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3htryogfc.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3cdhdbaos.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3ovfsloas.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt3vkkdxvok.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3baqdacpm.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3sjpiyuxf.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3epdowrfa.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3krkvrqht.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3egiugoje.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3zgtqkanu.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3tqtutlps.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3ktffgulx.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3everjnml.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3rtffhtox.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3sqjmtqej.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3uqlsvtkq.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3kaottfcw.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3hxognknm.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3rugwgcwq.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3gvlcjheg.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3nbhlahoi.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3cfavzbdc.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3ofjivzas.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3gnwwvgty.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3ycxbvvlm.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3iqqhexfc.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3krbbowbn.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3heiuxgxo.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3dcczsixv.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3ovrvvuyt.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3zwzctaqb.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3elpydkcu.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3vpzwjphm.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3wyplwpzk.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3qpegnwso.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3bqaqlwpp.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3xlpooqfk.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3xnlihkbd.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3ztdlrnfg.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3xmikncdd.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3dgzowxkq.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3thaefdfa.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3vvdqjjqv.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3vboijymm.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3btilkvgq.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3hpmasfye.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3lnowbeli.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3dvwgnjpu.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3fuejdfly.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3ifkelcym.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3aenbubjh.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3flgmcbas.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3fgezggeo.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3aelqnbgx.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3ytkuhynl.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3vmlibgfb.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3nksparkj.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3tyeaonxj.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3tcwyuvun.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3irolcves.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3nkqxcrxi.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3vclxgene.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3karehqst.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3mgumymgw.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3rrrifftr.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3unxolezu.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3bzpvvzqh.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3gmszmgdp.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3hqzbeefx.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3dsthlcyf.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3jdqcwxrm.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3vgexlkpy.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3olqhobrd.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3uenybonq.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3zkavlckd.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3spqeljil.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3xicmamek.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3xnnpkxpn.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3qpagcerh.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3gosfpihb.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3outjyutw.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3cukifjer.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3utdxawfj.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3fcsmriyl.html


<!-- 参考信息 -->