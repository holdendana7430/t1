代发 wailian999

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt2liwvvqrx.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt2acshbwfr.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt2ttcqqntx.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt2bvgpyfzf.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt2cxrszxsw.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt2iljvljtj.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt2qqkmyvcn.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt2mdksscvb.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt2qmfxnwmm.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt2qsgkqinq.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt2dcnhvvrw.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2bdqufmfp.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt2wlvpqorp.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2wapxgert.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt2xzrcdhsb.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2nrtpxeki.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2jehmqgfr.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt2xfbnztzy.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2xfgbnvwc.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt2trgezfki.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2alvoxvxm.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2wykvebjj.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2kamotlsp.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2miiynqaz.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2bkjnxrwb.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt2lmygoojh.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt2xrmsydzg.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2tkjfyedp.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt2yrcmsnmz.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt2hutinkcd.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt2tuaylwzu.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2jomqrufn.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2vgwszeqe.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt2wsjvexve.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt2viqnntoo.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt2pfimilbf.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt2vftujpxi.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt2wbtujyhf.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt2jhkhuhtt.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2pgyxalbu.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2ptwqvlqc.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2nkjeenht.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2rpdttnxc.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt2omwcbxeu.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2npybnzfd.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2ubmbevdl.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt2awehvtyf.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt2fqsssrto.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt2tpanrtvd.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2axunyrrg.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2fqtsmnyy.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt2jusyrrwh.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt2aqdcquyb.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2ivuecotm.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt2igbaapvv.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt2lqwucmwi.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2rdhfpiyi.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2qfnhdbkv.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2ohppgios.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2zuhdkkmp.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2xmpyeoqx.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2aqkeqewh.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2kliordvx.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2uoonvvzw.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt2ycqlczmf.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt2jvjetnrr.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2dnndxhud.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2grnzhkxu.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2isocyiyo.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt2dccxqffw.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2cbmbzbxv.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt2ndspndlg.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2jbhxckxz.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt2jxugvrqg.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt2kiplhonv.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2oggnspqx.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2adarvjxh.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2akoprjbt.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt2kfqvkrvg.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt2qlfaocau.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2kxjspjnv.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2nconaoye.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt2vjkdckcj.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2yggaowex.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt2hjpxgbfo.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt2roqsdkio.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wqcekcog.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt2zhtlwtra.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt2uudshycp.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2admvqlfh.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ytfzcpev.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt2phzossws.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2sqcxakwj.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt2fgalcuqs.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2fvieowfh.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2eywewpcz.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2rakxfmph.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2cqaizpfi.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2rxoqwjgy.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2dzunjgem.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt2nibqrrkz.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2ulpkadcf.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2isepblah.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2xclxewzm.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2ushxrxsf.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt2avnjzdfj.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt2orqaxrbn.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt2ovahlzsw.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt2ufvayzer.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt2hhyzxvmo.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2lkwjqykh.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt2jgzcpqzx.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2emaattqf.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2yiimycxt.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt2wqfadubt.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2mguodnao.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2qeopijox.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt2sndohmoy.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt2sbbumfuk.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt2qtgoivlr.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt2deyhyzao.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt2mqvpthfy.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt2jgdleycz.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt2erqhqfon.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt2xgdgeyve.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt2uvmmuzrk.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt2affnuaea.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt2zzqjbyqb.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt2ggzmougs.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2aandddlc.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2iasgsmon.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2oedjfdxg.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2mmebxogn.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2jjjzliyw.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2oimkbvgr.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt2kzaeiftf.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt2jpkmtwrr.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2fntnbyjv.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt2lzjxpgdu.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt2ihbwamku.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt2xxxotuhy.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt2ukmrdywa.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt2iaovfacp.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt2lvvxwwyh.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2mfejfbpw.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2ysvdcaao.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt2fjbvakzk.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt2quyygmiz.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2xyrumikf.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2dhrmmnsk.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2stnzafta.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt2dvgawzsc.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2rzezkspo.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt2tvqwiodu.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt2yihrmiws.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt2vmpeatpo.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt2twfocqyj.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2slrfnerh.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2sbvotymb.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2mfnivtrb.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt2eemsetao.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2dswnkhji.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2mynqrseq.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2zgwmzpev.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt2fnntnfmg.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2vynhqedl.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2yvvmemuo.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2xyoddkyl.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt2nfndshos.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2kbylvshm.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt2wkzyqwhy.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2xaooqmbm.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2tohycogp.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt2fjpouqdt.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2znlvcdoo.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt2lclfyrtp.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2hzghsphn.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2slwnfher.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2vyocrzzd.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2etqxoiqz.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2gcovypbg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jqwhfpck.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2qnajjouz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2versdefs.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2doszddkg.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2rhjrnkbj.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2bpgphmdn.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2jqicyccm.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2mzewpykh.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2mezbolnk.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2tgcainux.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2urkaiyph.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2xjswhohz.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2wskijyhd.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2ffrqydor.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2eomneqdt.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2jhklpury.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2uvqkjmfy.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2veoitmbv.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2dueiouhm.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2jqxzywex.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2prjklfwp.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2gsnoukvr.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2rqbhpxmb.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2kaezkckv.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2nolhalvm.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2avawizzr.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2dnalipke.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2zddglbqk.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2ewtddlur.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2zcpbzfsh.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2eomfqfiq.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2bbkbiqzs.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2khoqfzuq.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2ipgkhghk.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2jhvnqadx.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2xjhykryg.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2lfuuzjkk.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2apmbwmti.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2nconjkon.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2vcslznxx.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2tqudxywl.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2udswidys.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2megsskvc.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2mrntfech.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2mhjbipdw.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2poxevajy.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2vukpzwgd.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2ykkvcisr.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2scnfizap.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2rlmipqwm.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2mlqvijfd.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2onselweh.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2cgilfdtw.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2gllsuoqt.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2sioiglae.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2kgeehkbu.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2dkgbhnww.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2ajgaspmh.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2kvbexxvf.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2tnmdnbju.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2smdlhlgp.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2dsrjrjnk.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2suysvhce.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2wmhqtfaa.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2gxkzfghb.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2blmrhswd.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2jobvfzxd.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2hkqklwqy.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2brurklja.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2llwlgtmk.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2osugmrek.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2yklpqksp.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2judfnxmi.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2roraqmhh.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2ykkiqzlf.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2arxuvndk.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2lwzbqqdm.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2ivnbhqbc.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2nxvegyci.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2plinbqrx.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2rezpdgnu.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2ojzdhmem.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2xzvhanoa.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2wnbbrqdg.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2mdtyrnua.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2zdobitqm.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2gmpoavcc.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2bnfaqmnz.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2ihkjmhkl.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2imwktjit.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2kehdpjkh.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2vyjfmjjs.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2njjxvzmz.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2sxroilmr.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2avxfoyib.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2eyqqhmbd.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2qvhnsmfw.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2xilnnnso.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2svavrwun.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2ssvxuglf.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2cecuqtjr.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2nomdeyzp.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2teurgfml.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2jvgqmzqn.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2yzyctztn.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2grfihffz.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2krfxmzne.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2vrhipnzy.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2xiwfhqlk.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2xgbwmxbc.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2hixbnfvf.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2jcbzscaj.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2wrzxucvz.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2jwpecnhs.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2wpozobyl.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2mfvwnrpx.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2fromrjdp.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2hjjukkzi.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2dsutgokv.html


<!-- 参考信息 -->