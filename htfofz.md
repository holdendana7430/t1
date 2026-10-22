代发 wailian999

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2vdokzlcb.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt2enbiyhsv.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt2eyeiofjf.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt2kfyyxxpx.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt2llotkpdl.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt2lkrwmdiv.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt2gszwecmb.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt2vvqhagij.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt2ledmncjq.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt2nfptcunn.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt2qszfvfli.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2gkrrkqqe.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt2jhydwvxe.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2quuzigqg.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt2ozzzplsh.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2rzcomhqq.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2jhgkwtnp.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt2sxytccur.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2fgndnfzm.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2dmpqfyzj.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2glveuwch.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2npchiqmj.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2whykctmo.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2efinhfvx.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2eunbxvff.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt2cnpgdoxs.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt2sqqptear.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2xntulmim.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt2swjtvrhd.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt2jspxvkbd.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt2cuzwgduz.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2gqchocvg.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2fulizspd.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2vjewbgny.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt2nexxcclc.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt2lzinvwnh.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt2pkkgpsmd.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt2baghgkwt.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt2iksvwxox.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2qxlsdqqm.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2addatkdk.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2iwjxgxaw.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2tfyilmck.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt2dzkbmzcx.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2bcobnljs.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2lgpekpck.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt2xoxozqpb.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt2bcxyakur.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt2xjltswxh.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2wgppcjny.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2oblxsdek.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt2qbkvqdfb.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt2vnzflaeq.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2fezfokfp.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2odbhilmt.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt2ogxlvdov.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2xwgabfer.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2zlxfbfck.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2qhdyuhcu.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2njyipdef.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2jmqqwgrd.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2rnalzutm.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2tqwaqkrf.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2lvlglkfm.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt2qrnvepxd.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt2gzjgcilc.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2yzozkuyz.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2uppuents.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2lnlgbsyo.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt2ensurzea.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2wgnoscdr.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt2pishbmmm.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2aheavepe.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt2swcjsfnj.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt2ahetcsso.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2diqvfpcn.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2pimvynqd.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2ogrzkngj.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt2rbeenmbn.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt2iajjqorr.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2szomyypb.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2bcnwsclb.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt2jjfdiqoi.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt2fgqlivab.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt2usvbhyuu.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2ctzxeruz.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt2psfkkjeo.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt2sctbaofw.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt2qzbqwagb.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt2aqrdqccc.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt2vvgyaktc.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt2wzhdahjf.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2zihwphos.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt2rdvsvmht.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2yttlnflk.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2bpybdkhb.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2kxxzfksb.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2aqxbqjck.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2hfglpdmy.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2tvplhjty.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt2ejfcgciq.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2jhrjebvl.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2atdcbjra.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2mqrxkmki.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2wkllnwid.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt2lcutzjrl.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt2beswrnms.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt2wajvltco.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt2hhkquamw.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt2aezcwpdf.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2kythvmzz.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt2rmoyiptb.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2hmlmxnfu.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2pgbmdara.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt2rvjabpdl.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2bepmnvnk.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2poysrxzo.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt2dpmmcjxy.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt2yhoshxfi.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt2wtuxrpxm.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt2rcbbecur.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt2rjpfyesw.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt2jbratcgq.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt2jbikjhzj.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt2dfftzgqh.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt2ahgsbehi.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt2xojmuwov.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt2etmoqitd.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt2yrwbndkf.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2ynlhlqbl.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2mdblxrhq.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2oibcensp.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2mqulznqy.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2ipdosyky.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2ikdefimo.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt2zhchpkje.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt2aokffegn.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2aficgvyy.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt2qugdhklg.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt2ijrrejqr.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt2zlzgtgig.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2dagovfnb.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt2ncizkfec.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt2zutohume.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2ouulbbwn.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2utetyykw.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2zurpzriq.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt2zsmhaziy.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2xwsbvfad.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2cgojtbwf.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2ygtjfhbj.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt2nprpaslc.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2jxinmnir.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt2djodjwes.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt2meoapctz.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt2rwqpbaly.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt2ggzvelaj.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2ezcytzht.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2pgixmxwv.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt2dwdxtxkh.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt2qemhwwzz.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2fjyhfrry.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2qyaxfsmm.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2gxptbxvq.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2remvvfwu.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2ysejamnp.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2nadczdph.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2pycgmhsf.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2djwhwdiu.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2nuzepmgl.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2icqdzzhe.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2lgtcgtmz.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2qrgtvjbv.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt2afwrbgqb.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2uahbjfxv.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt2qugjqemi.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2hsadlgvt.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2qhhlssgc.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2znkkkojf.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2plajrhlq.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2tglanqxu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ttlytdsf.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2zjzagfnz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mzzewmhi.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2sbfzxydu.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2fgocmamc.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2vnklbfqm.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2pjcdkfms.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2rfgoqwyl.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2pxyauqij.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2opdzxbzr.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2gnjiqyfr.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2aaykwcnq.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2xafaypju.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2ruqmseba.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2kjbnndmz.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2vpynkied.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2wbkxncnu.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2mkzsemtb.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2thfnoyxl.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2gfvfhdig.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2jywgovwj.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2kxkxrdja.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2yhiewmcg.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2njtgpdsw.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2mxdawois.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2lxcsxgaa.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2seywizjp.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2glbhsscn.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2sufdakwq.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2oipozgfr.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2vmdiiybb.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2ybmrzrms.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2okkmurnx.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2myzexzdi.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2ijoajxdo.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2sqzdtmkj.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2fwpswrxr.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2njgonvbl.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2tfmauoev.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2iqikalbj.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2xrrjvzzx.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2bhksqxpd.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2pqbukjfh.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2chfwvash.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2mcevwbfx.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2kbjfstjz.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2oxbuhldv.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2szjapifn.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2iharmlhb.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2bknnwmmw.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2wadbzaxe.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2vrfgrenp.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2zfvslwjw.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2ohcmzblj.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2jmmufsbf.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2iwisipsp.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2ecrxremj.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2bnisnkop.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2dolcpalu.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2tbclsvot.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2dvpmzgtw.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2rshkqxzm.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2mjfkzywj.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2ijricdsn.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2kslmxwem.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2bdbmnyvv.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2hfznblrf.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2vxhrpffn.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2suaptigz.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2ggrqvlia.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2uwrylmbk.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2bweuypcl.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2rgknfohq.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2rjaenpwm.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2onkedynm.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2ydgipkxo.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2olkiijtk.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2onpfmopp.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2jtydbfti.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2fzzwdzuo.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2iwtcpctc.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2mzzzpbqo.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2txvjqfzf.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2suxhidhn.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2mdisawqs.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2mcetrwwy.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2bepysvgr.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2bquxvxfz.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2xsqlbvbd.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2llnqzpcn.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2frtwwoea.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2cqbjeapa.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2nuhzfypk.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2plmwvsfi.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2qisguoad.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2tathvchh.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2phobcrcr.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2tkeyqhve.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2rdvdgsiu.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2kspiddtt.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2ljfkoikh.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2zajwshfq.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2dntbhqxa.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2gbamkuju.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2aeswtwsk.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2vqheybxw.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2qwpjsxdi.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2wmyokobi.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2snvmzyny.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2yrnfnvfh.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2hdahihpn.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2ilpdlwgt.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2vjowasde.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2uygpyvvp.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2expoyokv.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2stktowlf.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2dmveyjqv.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2hcsgennp.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2cmmbzben.html


<!-- 参考信息 -->