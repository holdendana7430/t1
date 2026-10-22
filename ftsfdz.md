代发 wailian999

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt2ilwllqlm.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2rjhgtplc.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt2enrunqti.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2uarihvsd.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt2oqtxesqq.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2pbemppfp.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt2ubtkrvxy.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2dmrjtzvi.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2rrxfmoqb.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt2dkqjwbwu.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2fmscjsum.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt2amabnjvn.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2coffnmdc.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2zlthelkn.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2dewhzbyg.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2mcvmgcyy.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2rotcyzxh.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt2jermnlzn.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt2sqwhpwqu.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2zmfcttab.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt2bgqanctz.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt2vjjmkqfq.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt2buaqgatb.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2nynvhbkz.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2pcbzlcma.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2oohceluq.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt2jdlfxfmd.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt2ilbrwoqo.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt2fvgomagg.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt2pdnfqvlb.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt2qbgzyfou.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2qwozpmtm.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2duhbywty.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2kejpdhph.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2bfyrgmnt.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt2wfjondko.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2ajfyfrie.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2flvczenm.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt2xoaqmgyw.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt2jlrxjbkk.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt2yewdbtml.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2sysksxxt.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2rzugagsd.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt2zhbwycpw.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt2xbelstbv.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2uaizbtjv.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2gyjaeojn.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt2ngznbfog.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2acleihlb.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2kfukwemc.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2kjwomosu.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2qhuormxo.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2snjnmdwd.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2vxtnrteq.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2cwrgzxyo.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2uehfbhjh.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt2glzxnqsf.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt2vaakfcbf.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2vgryeikx.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2eouudmlo.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2tqczticx.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt2uutsmpws.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2edldnjfc.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt2scfihauo.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2uwvsmajo.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt2ujapneeu.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2gcrponro.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2phnvakug.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2vfoktvhu.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2kdrwipqp.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt2pqlllouh.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt2lkbmoubn.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt2nauqwjja.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2gkrbpdxr.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt2baktonrd.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt2frnslbqv.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt2gtlyqroo.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt2aqlboxli.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mqdxwrec.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nvpulfpv.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt2bchnbmfo.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt2mdapemex.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt2jlfjjrfo.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt2vifwjupu.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2ktwbenzw.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt2ysbrpclt.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2gbkgujvh.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2ftoauhcu.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2jpwxialn.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2xeyjecoo.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2ebmrfybn.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2xgsrzivg.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt2ttpbowry.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2vwmujyle.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2egyhdwtz.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2hjgewiev.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2iicizzaf.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt2hqoxlvmk.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt2yqkpixuv.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt2vupabqpk.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt2yckmdydh.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt2zgzvskjm.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2auzafcgp.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt2pjequqvj.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2irsznidl.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2eidapvul.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt2blvgcjok.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2ozxmciyb.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2imjjaray.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt2nuzcewsw.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt2ucjqylqw.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt2pcjxejxg.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt2sjytwqey.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt2xdglzpfr.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt2drofscks.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt2ijokatcr.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt2kgpxkznm.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt2jetpzpwm.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt2xgzddyru.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt2tiwgskuv.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt2julwzpxc.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2hcqjyrth.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2siefxppo.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2pqnxiozy.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2jiieuhon.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2uowyzdqj.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2jikcjzbb.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt2bglqwyyv.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt2kkconngi.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt2xpkqakjg.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt2vikfvodv.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt2tilyzxah.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt2cpreaunl.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt2qgsfewhr.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt2gsgugtqd.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt2hrbxmrut.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2yvqeapdb.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2hobztfju.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2orimdcys.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt2sqotjpvq.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2zedhwdxl.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2nazyimjm.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2ajjkapjk.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt2apqjpfzh.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2ljgshajq.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt2kdrrpvtj.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt2batzezpg.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt2moylojmu.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt2tkjfwpif.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2dfjyfbrl.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2aqlsggql.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt2shdmbysv.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt2nzczczah.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt2ftpcsgiz.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2expqofpx.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2vegngcmc.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt2fyudpveg.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2lwscecrr.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2mlhalxoy.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2nmgraime.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt2asaewfgp.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2inglpplg.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2ofbvfwgs.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2ikqkfmfw.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2rcszrmin.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt2ntpnqdiw.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2dfejzchx.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt2qudvmgsr.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2amwdcaxw.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2dvmsrtmt.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2sghqcjfs.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2ujyzqhsa.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2ojyxspqz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2imrdliki.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2dkhmcjgl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yzbtswjx.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2yomvtize.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2ygayirme.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ochchteg.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2wdvvdfuc.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2mumeqyto.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2trwnpbns.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2xohpydri.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2rwmxbihx.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2owcgrwdo.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2kuxqylwf.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2eiklmwqh.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2gtidocfa.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2ucsbatjo.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2upzbwcul.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2sfqagdct.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2evsarykn.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2kkpolyas.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2hpybcbde.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2ihmbshgg.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2sryghsgm.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ujtvvnhr.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2oiuatbbm.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2kuvvlqza.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ngcudfgm.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2yujrbyvk.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2ckfgkafu.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2zlwnxlhk.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2gcgxphck.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2uijigklb.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2ykfmveqn.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2nddclvot.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2yzxlwdkz.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2xcghksic.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2jhndybcg.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2icfzewqf.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2wquujqna.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2dhtnvykz.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2alxeqnrl.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2kvgjzsfw.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2jvkxyhew.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2jkgbspjh.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2innliumi.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2azpnbwdj.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2tgsjbvty.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2cbtbldrz.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2fegrihlt.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2rqqepbzz.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2jrrrklzg.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2gjaazbax.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2nkjbmlbn.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2rqlrhven.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2cclyxkss.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2pgpjjgqq.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2khemingz.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2usfdgppz.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2knhpqzzv.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2nvvojvcu.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2oprmdnen.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2fqsbxany.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2dtpgfvzh.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2fxzizlbf.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2obpirnvp.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2hthadsvr.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2dhcruuwm.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2wsjhoryh.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2bnaihkkl.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2iganipdf.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2xcrndazz.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2ttlldgie.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2qyfwituj.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2kdmbqrbl.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2zjuadria.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2unltcxnm.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2qpojxulv.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2vfcvhima.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2vojbqrxo.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2stsvozur.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2npyausvr.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2qdatbctc.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2loakzoxr.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2sqpdkhak.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2dzjzmdeh.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2mzyehzck.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2mvbuytcq.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2lkbsbfpx.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2tgpdjwza.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2ydtnlflt.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2oyqvsgii.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2pedwnxtn.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2hnqlosnz.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2pxdhpxhl.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2hlutdhfv.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2sdouxijc.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2cqauiigo.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2xbaptkth.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2vrgabxjt.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2ixosogbk.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2pkkfnayu.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2pvfthsgf.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2npwifbss.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2xscovgbg.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2uszbespr.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2ighqttad.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2rltoqbmm.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2csqxpbni.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2srikxhej.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2qzfvmefn.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2fmihrmod.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2ajattmqh.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2xvbaxbzo.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2zmlhaatx.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2ubjjxhlg.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2rjeiaefz.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2wusugpzr.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2kxyoeuef.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2zmdteiau.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2krfpfjiw.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2oozvsioy.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2cavcqgpi.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2tpueerde.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2mouxsnqr.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2hjprjnls.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2wklypftr.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2jwgqsstv.html


<!-- 参考信息 -->