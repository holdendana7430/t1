代发 wailian999

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt2rdummnoo.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt2mzxwpewb.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt2jmpvyfgx.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt2dwqcmitq.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt2gvzvelme.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2lrwdolly.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2yfhqrsfi.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2ckbykjlp.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2syoombvv.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2tbnbjffn.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2cusqnktd.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2uzsftiuo.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2eeeezkoz.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt2ignkkdnv.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt2qmbbwjwg.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2wmyyrigk.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2ckkfeskj.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt2dqtsabeq.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt2dfeblrle.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt2gdkkzkvc.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2raqbcuvw.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2yojsinta.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt2jzqnuhta.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt2lqgjntnm.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt2bjomdgxt.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt2mcwcdewh.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt2iroksslk.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt2wvjcvulf.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt2tcolbnxj.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2oclzkoeb.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt2coolhlzx.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2eeviumkl.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt2xhaubzpq.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2pfvwvbwb.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt2bdicbvip.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2wbrqsics.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2rwusntnu.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt2jhdoujhu.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2ekoacxoj.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt2heujtvts.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2vddqwbat.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2haffmnxu.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2yzwmruez.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2eryfhnow.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2apdgftxo.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt2ncdwgwjj.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt2bjjixbrz.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2jkihjzxr.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt2mjqqaeze.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt2jnzixmdw.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt2gtopsxoi.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2uhpjabrz.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2ldacbxqu.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt2tfeszspu.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt2egutuadu.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt2kswpuavb.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt2shfrqnqz.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt2zmnakocb.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt2xzarvcyt.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2vpomzfwl.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2shvbbzmu.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2apjyschi.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2axzbgmcy.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt2wpmdijul.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2vvofefdm.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2azppkwiq.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt2ncrtzwpt.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt2egfheyjl.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt2rhzxlivx.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2cgazqthg.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2nyobilsb.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt2wmaytnnu.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt2hfuctvuv.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2ufwxrvoz.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt2iklusvps.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt2pvylzrqa.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2qljckubc.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2xnnfuwzq.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2yhwutcru.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2zzvmydkz.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2ixzytbdu.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2nghjxqou.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2tlaqflya.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2glsehwtx.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt2hvrtlcqz.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt2mdywbkia.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2nsosnopp.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2engxrikk.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2npdpynwi.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt2aapizbwh.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2bhkpksrr.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt2azvidavo.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2bxbyqfmv.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt2jhxapkhi.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2wpkbgelu.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2mntdhhoc.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2jdsxatvl.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2josptqcf.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt2opmjqscn.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt2gqtgycsb.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt2udhdrpon.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2rwqsziqw.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt2uhtjvait.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2tqbiynyv.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt2rubnwyer.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2ztlpxjdr.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt2cprawrfi.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vmnorxcd.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt2veizfpwp.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2bunbkkpy.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt2mjkrjbmo.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt2wviaanqx.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2whpubxmu.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2uewenrdi.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2kcjiopjh.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2yvtknrvg.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2gvveptlg.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2ptsjqzlp.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2uhktypgg.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2ithhscnw.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt2acohocjk.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2vfqqvqkk.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2kmdplsio.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2lhgehbuo.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2xbqcrrch.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt2eivtygoq.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt2pdamgfmc.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt2odqsjmnp.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt2xcsvwaqh.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt2qzkvetfa.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2mdwbwxpq.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt2ianoikfn.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2ujyuricv.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2mpajieij.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt2cvljbrub.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2mkodjcgx.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2givdqazr.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt2ivqyjsxy.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt2tjizrxif.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt2ekjihqyf.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt2ouxpvyus.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt2eygtgorc.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt2iaobtfde.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt2icwpnfkd.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt2mkatsvjm.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt2fatllzhm.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt2dtcqxgnf.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt2iylaxgca.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt2eiowgvef.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2zvvtzrjj.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2avubuhix.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2fviecxvh.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2syxziyzi.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2cfkekvrs.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2iqaojmyv.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt2nokvakoa.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2qyzvxdqw.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2dhiggbwa.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt2hakhwykz.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt2bvjwscjl.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt2rxqvzmsr.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt2ydgjxouc.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2bauwrkko.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt2boggczyj.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2syxdctou.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2thifqhuk.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt2lfxncmhx.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt2trxawvdl.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2siarwzgr.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2ymddhqke.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2tldvsmgc.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt2jwxbjoiw.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2vsrfcage.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt2wglpdndj.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt2lohemoni.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt2zyvmdgrv.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt2lgfsaxmx.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2xsjjhhxv.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2yeaarqmx.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2tgtozzqw.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt2rdibzcak.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt2nrwokzux.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2tjemjjxa.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2pumxkgvu.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2tymkwxcj.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt2ftlhvoqr.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2mjemkqwh.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2efpkfvdo.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2cjqjsyig.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2yzxkhbpb.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt2fuxsyudl.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2mowczxbj.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2tavechmh.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2eesbdebf.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2wwgirtgb.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2yvnhmcqp.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2fwljyamu.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2wvxrigbi.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2rchylusx.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2bhyqdueo.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2fadbdsum.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pkwwtwes.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2quyamexi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2khhazdcg.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2nxedleov.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2wmkkvpzt.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2hspsssig.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2zyqppxdb.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2yjftjfqa.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2jrmmviky.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2eewdasib.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2yqbfmovf.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2haeqqezm.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2yqxmkopp.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2rlexfoam.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2slyrbnjs.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2toayecqa.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2lbzvxubz.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2mxlhbgyn.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2xjtzexsx.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2vzpvujjk.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2upmtgbkm.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2skvtkwar.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2xyltrdss.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2bmbsrcco.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2kwvzrgag.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2hrqaanmz.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2cpvebppb.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2iaejisvs.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2xaclrxgk.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2rjilnvvm.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2sgvmmjak.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2ubvfeucq.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2pzzbkehs.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2iqswgvmv.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2qdwbejgm.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2flcmpxmj.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2eljobvav.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2lpfhwfnb.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2moaittix.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2evugzguw.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2ajlbfosn.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2mciunvko.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2ojaazrkh.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2utkixrxn.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2eumtssoj.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2nnzlqwdk.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2xqhiblrs.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2vlujcgxu.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2pxbhhgkt.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2yiuheuvv.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2rcgvfjlg.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2ypqynlxk.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2azdloxxv.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2emjlzftv.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2mpqxkvwn.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2kaqzqpzq.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2nzwjwcis.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2ukekwvpi.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2mvfcasvz.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2qeeetgbl.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2enpnhnaj.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2fwxgazhy.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2ccagbkqn.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2yblozzok.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2jnnanbyh.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2wpucyvtl.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2sdxikehq.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2hjlrqrwo.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2xxbdzmyi.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2fzigvthj.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2ewctniaq.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2wiyijwsj.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2dkacxyis.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2kozqxuzh.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2qxabwiwq.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2efaovjyr.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2lbzyvpbn.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2pohksvan.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2xjhyyjmw.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2tmjgckxr.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2hzffrhii.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2barlsvrk.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2hlcprdsi.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2dqxczoiz.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2zdqqmjkm.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2xcpgwdco.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2imjembku.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2oavaumio.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2gqlypytz.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2qdbhyjpv.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2qqaehwul.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2fbwmtzbv.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2kpqyljux.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2tauxtrhw.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2qwhbjjig.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2enjiuwpq.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2qqelmmab.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2wtfpxdie.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2uqnynctg.html


<!-- 参考信息 -->