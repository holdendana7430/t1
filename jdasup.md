代发 wailian999

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt2zpzrndwn.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2qfccbqbq.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt2kzrcirle.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2fqtaxqyr.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2esceoqni.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt2cinbdfmm.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2nncdslop.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2bvotricg.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2dregcpmt.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2duwynidr.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2dttapbhh.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2ntrerooi.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2vtzavwbz.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt2vfqqvhil.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt2zdcaufdp.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2qcxujfgt.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt2syvgfewg.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt2idtihuii.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt2lqulaexx.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2usnwmpfc.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2fxalazot.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt2zfajsmdu.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt2ulzmjrdj.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt2bqgpjlsd.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt2bmlkdezx.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt2kfuwqyhp.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt2azqabpyi.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2piwjgors.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2zhszxayl.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2ouagaafg.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2ftarpbta.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt2nidowiqm.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2eokdvmkw.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2zcdtstiq.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt2uwynrstr.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt2zvimfcam.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt2czqxxifv.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2syngghbf.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2cypjhbuk.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt2zvumsyvd.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt2xmktnklz.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt2mfkspmuf.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt2uztjnllt.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt2ttvsorki.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2gtwupdnp.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2klwbvvbc.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2ujretxzw.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2fjqangsm.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2asrerdwz.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2snvlkdrg.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2eoyqsylh.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2tjqolseo.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt2jxvlrzdw.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt2yalzvzow.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2zarvlash.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2yycxkupb.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2cuqgplci.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt2gukljoas.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2akrkfzoo.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt2lffvrubz.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2zfktoufz.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt2sidqxwpn.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2rqhqurwz.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2dmssifil.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2rxyskbnd.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2wgxktwcd.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt2ymdxsahv.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt2ijjavewu.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt2gfvyefdv.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2vlekusjf.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt2jryqhnrg.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt2cxuyyvii.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt2vyjjevjn.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt2ckwhftfp.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt2uftdeytp.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt2zehikhxd.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt2iijdkoor.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt2bqcrjukt.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt2zylrlvjh.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt2rerasekr.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2gylehlzq.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2pcgwmflx.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2tvznpzlz.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2tjktufet.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2hxtgirho.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2btwntfve.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2cbhgqmrl.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2rgiunund.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt2cxcegrxx.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2nadmkhfh.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2zuioadzy.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2qiutagyo.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2qjdkcxge.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt2vkcfcpdx.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt2dkajixrq.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt2bfajgexu.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt2karobzjh.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt2iizmsmsz.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2kgxcwwpk.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt2xgaqaxlx.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2wtpkcwxt.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2nkukhmgt.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt2wbywxfmc.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2kriifjln.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2zlughwpa.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt2ngyvargi.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt2lqouolba.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt2srpimval.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt2puhpctui.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt2vockbmgs.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt2vurgmpxy.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt2ihahcsod.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt2qfmjqooi.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt2zyuhoxbd.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt2jymiqlky.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt2gmqwhyaf.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt2kihuhvsh.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2ypgsddeo.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2eeuuxmrr.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2iyvjoctb.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2nsunhrpx.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2cayynxyn.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2bnzrxphe.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt2qjhrfjuo.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2gqrxjsrz.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2krhyocfc.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt2gipcqwjg.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt2xiuvfpzx.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt2dpqjhyij.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2lpqlsvld.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt2aphihqpz.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt2unzmhvob.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2lbnhjlah.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2wqbvzbmk.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt2adrheffg.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt2wgrzxldh.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2lpoeppyb.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2vzqhkxun.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2vlumvcxr.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt2uyfrkveu.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2lstdstby.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt2wkcbtweu.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt2rxehwxct.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt2fsxhwhvv.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt2tcuwebby.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2snisazpn.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2ggqzdowu.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt2zjnvzsew.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ycjhmdvu.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt2nuhfwjif.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2vlprdgqj.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2rfpxmbpq.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2sifcgsyy.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2brhgmrml.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2gtxpqnwc.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2iadjwnok.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2rckoyjmc.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2eyjlstcm.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt2odihdyse.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2abthafyx.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2bqpjwyow.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2orrqhugc.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2wbhfuqur.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2malywcda.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2krxesdez.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2pjdrabpy.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2bjqmnrsv.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2cnsfiymv.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2cedxxmrv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2idmkfxfl.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2umkqfmrb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bucjkvjv.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2vyyitdjo.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2pjsyekvp.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2bvydvmjt.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2uodepmbc.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2yoktzhne.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2ttztfgbl.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2phpayghs.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2gqxodktn.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2dkitxxjv.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2sztjrlrf.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2opsypuqg.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2bqfdtwwi.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2aqyggwjr.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2jvjpxcij.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2xvgsgqsm.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2olzdcqgu.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2jrixpubu.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2kjwvgzmk.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2aszfgxwv.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2bwiluwku.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2pljrkgzn.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2aasyveul.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2jzflnrfl.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2ktkrjzkt.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2hadurnky.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2rpieprjb.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2xhxbqbmj.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2hxcjgyie.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2bzxrhnom.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2ixiyvocu.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2dfauaqjc.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2cugzsyxl.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2stpgnzjn.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2vizrwkjp.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2gzrdmmun.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2nhdhcxhe.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2nelofvpg.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2xluiikrv.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2uykjdlzo.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2rfbfilgf.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2hlpkaxln.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2aafpesxu.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2zpakbsnq.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2ivpktuyc.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2hsokgbyl.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2rvtpjmpp.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2aaqdnrsf.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2xtjikfoc.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2fitzwmsf.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2bunvtkqn.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2hyguyswr.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2jykmvtfz.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2koltpuai.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2wjaeugpw.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2nbwokrbf.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2gnkoqzla.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2uomhywhg.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2wbgervyt.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2wudttgon.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2rcybiyoo.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2twsvzsiy.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2vhjhdzqh.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2yayzdern.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2nwmomubz.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2bwchfwbx.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2tnwnbfml.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2ynfgizas.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2zxnwuzep.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2rfqxqads.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2idjyxtvc.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2dlsnkkls.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2wuklgzck.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2jfdajipf.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2iaouunun.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2bsncjeqt.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2hzyhqftd.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2skvnnseq.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2cgobsihx.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2cyjdmqzy.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2vohfqzth.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2goslergi.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2iofsmdub.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2rpvqzoql.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2yxmlvdbb.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2vttnnswn.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2fuwfkaas.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2ahocoran.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2cwbofpui.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2wcbodibu.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2esdtnfcw.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2sypqpfpg.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2hxreofbc.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2npyrvelu.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2cbnqcvlb.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2dqkdcayj.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2akopdxru.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2hamgkwbc.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2rbpqftim.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2olajdvek.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2wnaxuasw.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2uvhjnhlm.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2dpvuuwym.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2nnhcyihi.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2kabfulpi.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2tcrbvsdl.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2nuxzfang.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2rrqvhxog.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2zkfhyotu.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2evhysfte.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2gnoqktyb.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2ymznfaot.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2trjowqcl.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2wqpevwku.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2vdbllyjm.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2eymsbsif.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2tqcsfbsi.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2xqjuaeya.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2gnkwvevw.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2jnnqgcny.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2obotxztd.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2waurzrdo.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ssikbwxz.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2lojfntnu.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2tkboxvbp.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2pschwuzo.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2hnjxhxbe.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2xvbzgrao.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2klfuvxei.html


<!-- 参考信息 -->