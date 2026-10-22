代发 wailian999

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2swiebkoe.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt2szfzaezw.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt2lkqwlxox.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2mmzhdcso.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2ytfhwfek.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt2zcxwbzov.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt2yxtkbwmb.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt2qmabtbfd.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt2nesrjeyi.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt2mxltxkwp.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt2mgfnwzqe.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt2lcdjsaxq.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt2ndszwete.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt2exzpodzk.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt2esumvzyy.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt2nvueyobw.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt2jssqwnai.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt2bkvvdzet.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt2qxpxmmqg.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2lodhzeff.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt2lnegfcdt.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2rzutpgqj.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt2mrycvkke.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2umbyvgrc.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2irftccyn.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt2blnqcnkb.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2qfwtdjbn.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt2pcelenkn.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2bglnhcre.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2mpizudwf.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2mfitqlzf.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2wuahipsp.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2lesaucvb.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt2jqpdqxvu.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt2orlcbkzg.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2lssinlzc.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt2pvjpormf.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt2wmuppmvx.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt2zsqlughb.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2uixxqtui.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2lgoorjxf.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2tjxhaglv.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt2fegnuzfv.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt2ajznnzfu.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt2fxrfwbix.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt2xobqvuco.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt2metomana.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2gysuupjc.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2nlknkgwd.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2egqdcxsl.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2qiqlnlpf.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt2issoegak.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2czujauzk.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2nmeifkao.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt2sazgcmkq.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt2ljmdngda.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt2ibmkxpvt.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2shijjwwe.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2vjsxjikz.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt2ywnyaank.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt2spvysjir.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt2ocjbaldr.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2odjqmnen.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt2dlxtgvyh.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2swxrnfsi.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2dfveffas.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2jbwavtwf.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2cmwvfwls.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2bxyjhzbl.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2nqudyzxm.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2iykyeyoz.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2hljxhdgx.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt2ajegkiio.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt2ixfxujox.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2quglajnq.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2hiajivin.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2etxxkdyt.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt2mskumpcv.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2rvzntptc.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt2fnzocbld.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2ebuovdgg.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt2jnybusyh.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt2gzzkqjdu.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2vbqogqba.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2ujnicvbr.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2tcrlcrhi.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt2gsxmofun.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt2tuzfgpfn.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2sfaspvnj.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2whygyquj.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt2hmjsivok.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2mkppyiik.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt2ckrcjkpt.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2ecguopha.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qpjfhrxe.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt2dnsgkipl.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt2jopluwlk.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt2egvftzya.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt2nuwowjkt.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt2nxixpbxr.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2xliccvue.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt2zcgjsqzv.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2otnquaqo.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2nmrvlxvo.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2weeeijnu.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2kdtudgpr.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2grnrsqua.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2blyalyzs.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt2hirgxchh.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2liheaknt.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2dltpqwut.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2kwlstape.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2ojmvxldg.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt2pzaykvwx.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt2aonyhcrd.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt2rybjffzu.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt2snftszgb.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt2eexosccs.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2wjwzrere.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt2pwejhbxr.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2krazeuoi.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2laysurap.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt2mzawasxk.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2rvqkuagt.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2kvxrcghn.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt2patfjjaa.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt2zyjhnwet.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt2mhaezsno.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt2myctmowy.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt2lewgedct.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt2mnopmejx.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt2jrgtmscs.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt2rsuantzz.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt2lgfihkvw.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt2sheyfhmt.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt2optejlos.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt2wjvuxtyw.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2pgxsgpnv.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2gqevocdv.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2eqdwnjlc.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2euodqkqx.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2fluolrue.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2pihqnbsw.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt2scfqfaaz.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2unuavolk.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt2smlsrjwr.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt2vinoteis.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt2ivsginqd.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt2llsaibcl.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt2fxfthiqk.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2mrsyhfun.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt2gnshvrbs.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2rkpqdhpl.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2sapiqxoq.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2mpdwcqgu.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt2bfqhlcav.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2zrwcccpk.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2ourwnuyd.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2xxmdhozo.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt2peekmjyq.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2nptslbvw.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt2cssscbwe.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt2gpkgbjps.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt2xvybtwty.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt2qrpirkzo.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2ocpfsyjy.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2fnweskyk.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2tmqbbxvy.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt2julbzclj.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2efxhvfuh.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2azqjboua.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2tgbtfmwb.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2zsecmtpa.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt2eecxiysz.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2agnlgxtf.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2keggxtsw.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt2ksseplvb.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2lgtonpru.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt2nzlqzfgd.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2mlhrftfc.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2hhptjsac.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt2mtazcpqg.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2ymkazvaf.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2qfgfaece.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2gvxcvgiv.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2zpkqnzfl.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2yjucnlvw.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2larsvnui.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2vjyelkxb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tqimokad.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2tbymzayr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ckhteytd.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2yvkannjq.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2tnejjxqx.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2wukrensi.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2khfdhhxr.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2psmnguyn.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2dwagfafr.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2dienljyd.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2hwvbrmkt.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2lhrfsljm.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2uozoltpg.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2lzdgadin.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ryiitufd.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2rwyqaycu.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2hybgfutj.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2dyszvkdj.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2jbifztye.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2qrjxlmeb.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2kroqlenr.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2fvbaunsp.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2vfbxyrmk.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2darqeadn.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2fnepjsbk.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ekrwpnwj.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2qgyqrwhl.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2navokbaw.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2drboqrfz.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2faufsprj.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2kmjcugjo.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2kzpupcdx.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2qwojpgbz.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2nipwclcp.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2pntqhvyz.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2kraixydh.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2zpkwgacc.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2ylnoells.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2cntaurnm.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2yurpwxlv.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2pwdyquan.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2oytlojyc.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2bvssvtga.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2dqiitvso.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2mawvhlgb.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2elgvskbe.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2zvwqdnah.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2jivadqrs.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2ikrrubgo.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2swiqwwyn.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2rkhhjdxx.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2dpvwikjo.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2tkodqbhq.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2xrkhhgwt.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2zqjnmeip.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2yyoulhia.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2oruejjck.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2bmhnxwvx.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2gqpsfpwv.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2rbkclttf.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2tkbfpmbn.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2ayidvcaq.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2ljukbcyr.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2zbrtcrhb.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2oavrnwts.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2qbuybkjk.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2fimsoaia.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2fnngefhl.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2mjzogsyq.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2umgnhrcg.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2mybhsqew.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2wefgllyh.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2ugggbktf.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2texxkdzn.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2dwecqhhb.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2umnwbtff.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2pdpbhhra.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2kpotyhrj.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2uqjdtivx.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2odmarjrx.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2pxehjjkk.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2okckepbi.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2exkeyloo.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2bbmfwfix.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2ehwehvlj.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2srortrqi.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2plabqkxw.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2bppeptdz.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2zchiuzve.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2ioenhrzd.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2tsgajspl.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2bmniwwtl.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2elkffhtl.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2mapirrwz.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2yhjbqlof.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2cxsgtxeq.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2aesjslpv.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2pxiuhiwe.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2kmiafege.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2taabdczp.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2ubiybsgn.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2ftjbxyhy.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2iznmslre.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2pomchqeu.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2gnnezfzw.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2vjpmksoj.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2rkiaekfx.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2fzgslzmf.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2ngupofry.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2nnunzdip.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2dftugiyl.html


<!-- 参考信息 -->