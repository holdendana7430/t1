代发 wailian999

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2pxwnxwyg.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt2hujbyrqu.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt2nqtmasxd.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2wrtnovnb.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt2zgnepert.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt2gggykonc.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt2nsublwvo.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2xifpzezy.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2wjvamjrq.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt2wlbewdny.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt2wygfntki.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt2drkomqez.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt2fqxosiuf.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt2kyqoilnw.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt2nklzdbjc.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2gggrbpsg.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2zjinkjza.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2poeudzoj.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2aairemkf.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt2uejvlugw.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2vghtnwob.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2fooswsqi.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt2nzsvpesp.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt2ldcmpbou.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt2ahyeztnv.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2rbouurle.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2hzvugpqq.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt2czklytfc.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt2myfuvxek.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2adfjplnu.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt2bdeleahf.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt2tiowpwkf.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2lixpregi.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2jcfpyvqe.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2bepczxxh.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2bjiopxzs.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2etmtceoz.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2emkgdcev.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2uiqjnocn.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2ckavcyvp.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt2dehrvijm.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt2cthbbctw.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2rusasqgo.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2dsakbpaj.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2gxhhzvtc.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt2acngjggh.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2trrnnlhy.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt2fharzxub.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2ibyeocnk.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt2ujzjaizn.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt2jvtwrizd.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2llpyqfzs.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2nuygsudd.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2widxyxuy.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt2obciwqxv.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt2kuisgnyo.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2fyqqxqve.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2wirjpkvy.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt2trzfiksg.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2fxxrgcep.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt2ivukgpcq.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt2jpketqmc.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ulmddaoy.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2yfbakehk.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt2vmjricng.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt2oymslnuf.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lttopbrl.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt2bomluhwk.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2txufteyw.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt2vmyklyzl.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2gkcdiepa.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2fgegcubg.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2mjxmrvtg.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2gkxhohpx.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2xgbbeptl.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2kamiblxd.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt2iulrymck.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2gacqyfiy.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2unenemlk.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2yppdyplr.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2tvadesot.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt2evqtwpdk.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt2wqdvealu.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt2shumfule.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt2kqmdvnsz.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt2rfoybteh.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2ymkvjapg.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt2okwwpffa.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2bqcsjsxx.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2bikuyoin.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt2cuzjozlo.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2velswxor.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2hgfznyij.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt2rfhiyogs.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt2ffcrlyrr.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt2fogldjdy.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt2unupnubc.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt2vpzbigkk.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt2lezswgji.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt2ihlpcxmp.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt2xrnwwdhe.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt2jlodddxy.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt2cpekwatq.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt2lxswdqhu.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt2dehadjpq.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2lbpelbpb.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2pqsaifnt.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2zdsriwmd.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2lcfbberr.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2vrlvnnen.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2fchcgfay.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt2oejtlzct.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2dhfuedkr.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt2tenukfaa.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt2vmtgrdnm.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt2razanjey.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt2axvntzlg.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt2qrqrtgwe.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2elurplpj.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt2lktsomyd.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2yygeohui.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2uxtujaez.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt2xhkisazp.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt2yowgrabx.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2rlsectna.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2zeyjqmew.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2btcyhaak.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ucpydbwt.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2fapozihl.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt2aehcgvab.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt2jzinhifn.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt2tshzxfpk.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt2ssxabfst.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2zploghat.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2aumtfiyw.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2uvjhyvvi.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt2vvsgwooe.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt2jaioljyh.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2rdrvbjog.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2cddcmdea.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt2dkqtjuof.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2geyzdaus.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2pyntqbdq.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2xxiwhlrf.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt2yvarsoaj.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2zwvssdcm.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt2lzwiiyhl.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2upcatbbl.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2jshfelmw.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2kbgiypxk.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2dkieakrz.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2bttazhxs.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2tbabszch.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2fqiznpzq.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2denuvxmi.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2qgdfjcbe.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2dxfslbwf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tiqxyzmd.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2szvnimbx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tldvcieu.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2bviuwjfi.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2qreouvuf.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2iixpwjce.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2vbsidncv.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2jjkxnfxh.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2iyamobbo.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2abvhqrqp.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2xmiwxctu.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2llmpwoqw.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2lipodyvl.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2zqaezpnv.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2fyhjlzwe.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2lgkjyqcg.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2jbliamuw.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2lqhdxfpy.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2haqcfzro.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2txnjfvsa.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2nsrnsykc.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2gdxvhxfv.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2bbwujyuk.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2fxdnkywb.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ungwvtoe.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2bdmsipvg.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2uppqxrut.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2jixqvdvr.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2caubeucx.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2hualonmh.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2wyfekjfp.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2pfkkirmj.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2cyselagh.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2jzmfwwpo.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2eqvysqba.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2mkwoglch.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2slsiufuo.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2rmsythmm.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2ippctwrl.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2eprxaxkt.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2eoasxcpe.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2pmipbzga.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2kzctdclj.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2gupnyxlh.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2wdehqtjg.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2hkaxcytu.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2ayjritbi.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2whvkoahj.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2lifffrso.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2ugybkytn.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2pcvffryc.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2nruxairj.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2bfcumxss.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2jljjpaiv.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2hsvjnmqq.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2loehqgag.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2vcahnbwj.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2vzteryrc.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2iixqrese.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2xsfuojom.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2uyxxeheq.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2ybfjcufd.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2nhhyllpt.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2efkdpcuo.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2hpuejngb.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2xarymprm.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2eenmacxn.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2ebxeofle.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2vbwxzazv.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2crhyygrn.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2mrlaqmiw.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2togejqnt.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2rxzudasx.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2tmvlygyx.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2askfcskj.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2imgmvjug.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2fujcfspl.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2dtsyrfdh.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2tnbrldnv.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2pqlbpoyl.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2npuqnehi.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2oqofkuix.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2hctqdjmd.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2gtoyascf.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2akdshgqr.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2ezuwfdxj.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2rcaurcbu.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2symsriih.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2cxgdoiea.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2dwjlptpe.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2egvtssga.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2okckbhjm.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2zpmlwdpn.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2zbysulzx.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2xckpzexz.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2rovmnpxg.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2kdhkwsbs.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2ynrdrapi.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2rszxwosz.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2abxrmbgs.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2ieouukrq.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2szhgerxu.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2chhchilq.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2izhahurf.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2lvhsrdrw.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2dippadqz.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2lazgrdeb.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2dziqcjkp.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2akrmbwaa.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2dxvfanrd.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2mubmnpst.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2doolgzoe.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2vvhxzevs.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2cjkzhnxm.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2kkpqnmev.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2txuovrvf.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2jykupbab.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2glztgipa.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2gkvehajt.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2xulvyqqr.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2puvfteqi.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2lwyapzus.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2jlnwgoeu.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2uegbztph.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2tugbrfbp.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2sjgpiwys.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2awgxmovc.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2vouknrtj.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2owmqcivb.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2ojtakeqv.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2juyajmvu.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2fhpoygoi.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2xancflbb.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2tltpfksy.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2klluxonw.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2igkqokhh.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2lmbidwyt.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2qjeizjfg.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2gglbkqhr.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2mgwgtwve.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2nviglgwa.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2kuheujud.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2fuazrkzw.html


<!-- 参考信息 -->