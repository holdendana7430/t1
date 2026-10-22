代发 wailian999

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2jjwdheew.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt2wqaqmewu.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt2tiwszogc.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2vimakdzc.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt2sxllogbf.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt2kctcgjhp.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt2nabdlmim.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2oqsayynt.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2zsvuited.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt2daqdpfbf.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt2jvvfpwnr.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt2djugegtw.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt2aqpszemy.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt2qjfuuhul.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt2atzkmbsz.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2czvmkspt.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2lbixcfox.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2kmcybzlo.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2vxphettk.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt2iokertbt.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2proyeuuk.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2dmqevmeo.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt2yksdylhz.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt2mavgzkgh.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt2bbqrrpfo.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2mrgdafea.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2xngcebrd.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt2dubfjgau.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt2npotzrne.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2bhnxocsc.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt2jlpclcef.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt2cqqrmojp.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2htuuzswm.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2tzruigcz.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2nuvnyevp.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2rgqjdbcx.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2mrvfetsx.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2eebsfujm.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2rpseeyea.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2iuoikrbl.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt2femxpcda.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt2rvnelfvd.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2twzdmnvh.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2otouupjk.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2cfowlrnf.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt2zxwzkorj.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2etwkzojg.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt2hkzrpiln.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2zeggeqmb.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt2uwcxylkd.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2tkzgfomg.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2nhhpqkbc.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2dfvesbpz.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2sxnanxlt.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt2falreflx.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt2hhftwkos.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2nbscqqpq.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2diqpsnmg.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt2cinckfwn.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt2dtitcyrn.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt2cdlxqegs.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2mrwgtymp.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt2vnwxceoi.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ueexowit.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt2atakwjxp.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt2wtptkgor.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2aasbpkup.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt2fdssbqzn.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2ozyechih.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2qdanswhw.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2mhxcozea.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2kmpfeljx.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2zknwroqt.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2vqlcgjhq.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2bpsqjzdg.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2tqkdwrsn.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt2qibgqmwa.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2nstuarqi.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2rghympmi.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2vjfdgriv.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2pwkckmec.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt2dxjcothb.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt2gwrqhlqv.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt2gupldgwz.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt2clpgoomw.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt2aldtvtxw.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2guayqlgy.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt2gqbqpznw.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2dszjfqgi.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2whjrlxgl.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt2wbduncps.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2awjnbynw.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2wwsefapc.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt2bdejkxtw.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt2ubqojqog.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt2oftwkgip.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt2lkcgldld.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt2yllpkqaa.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt2vtpvuexa.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt2aywojacj.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt2zkdszppv.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt2hvbiiipb.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt2nancsryi.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt2ehhfqius.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt2wixlbfvs.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2fmxpzdiq.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2qxxqeffd.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2jvxsfgau.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2gtevribs.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2hedozfgx.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2pwmktswe.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt2ubthzbhr.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2lcovsjzo.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt2emsniyzu.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt2vbgaomep.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt2ygwrsdey.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt2wngabroj.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt2uyderaoc.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2dkcuukyp.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt2fzhfsuzf.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2fdoukiof.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2mdxothct.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2oqsocvio.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt2kwiiamnb.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2ofwlezoh.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2hkhgssgh.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2wmpwoqvd.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt2gibpvhik.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2huzmjidn.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt2hzqunslo.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt2aacsclwd.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt2rutnqrgd.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt2ieckzple.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2kwtuvxsm.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2rkghgnqj.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt2xtblmvml.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt2hfchdhrc.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt2piyqkpum.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2oxpzsqdx.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2nsrbypam.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt2fjkwzcxo.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt2ybjnpfea.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2yvsoyjtd.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2txgpmvrz.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2hzzuarxx.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2utcemvok.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2zbqqcgim.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2fdmcckcv.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2azjsroqs.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2sfhpztxh.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2rtyzyvwf.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2bigsoqys.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2zjcwjxkt.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2apiweexp.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2anjnijji.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2tepbexlw.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2oyxvufqe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2iagpypbh.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2xehcrgfq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gytaikbn.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2jknzlfkh.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2wfkwghmq.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2obrcnvtt.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2sjlwsjxu.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2gcngzrpl.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2yonygtle.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2uptyaxmz.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2rktqcqol.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2qxablpzz.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2davsojqe.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2ietorkbn.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2tosbnhar.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2waocytgv.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2txhxonso.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2sungjgsw.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2bnqckmke.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2omxfxxax.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2lzymuyjs.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2viszzdxb.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2tdypcept.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2otibfnmm.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2nforojud.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2odkwivqs.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2qmccrewi.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2xzhakumo.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2rxcutnyv.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2xzvdtljc.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2iumonrbu.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2oddrjdoq.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2fyxdbvsk.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2ocyhunyt.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2hpxpeqco.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2ucyieuke.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2acznhozx.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2ypegnddd.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2tsksygjz.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2ggxagwzm.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2baqkvunw.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2gwblkerz.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2tbymqsel.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2kfhkaelv.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2jphccceu.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2ovnphzxb.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2mucelnib.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2halswtgm.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2phspaqcr.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2bshbhjhb.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2wlzcvqie.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2xhvwetzs.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2lnysjuuc.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2qvhlviik.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2sgmtbohp.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2cquddcpk.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2vlndzfer.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2xgejaogz.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2jzdspylf.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2emhkwimp.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2cesdsosa.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2wyjtsdik.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2pklbjczm.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2wkffmuoy.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2vcljhtrw.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2gzrbxvvx.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2rrzxbtab.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2gvaglkla.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2lulsfkak.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2yxyvvjck.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2cxnquyxr.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2gudkkkpi.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2vszfzacv.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2hleglbnl.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2pkkrfldf.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2pllohltb.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2dnjzbjaz.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2xzrwreqb.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2lmkalckf.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2ghsvfgfa.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2yiotmjkx.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2muvghost.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2zzoyjxer.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2avlvgrct.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2qvwugvzn.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2opgnmgxd.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2ercxncbo.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2bailbdhx.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2gdenlylm.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2tnhkktfa.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2crlotyyf.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2zwhxkgdo.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2ujowmcop.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2hbbsiylf.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2eyuqyequ.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2pvoibcfy.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2fmchenrc.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2egogmhnb.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2hawccokp.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2lufhurvt.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2bxotyfkj.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2yvampmsr.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2yrjqigej.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2rplamjfy.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2uaceqexa.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2xhdgpeeo.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2etjjcezf.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2gxuvgvbq.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2vbdmvcyg.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2czvmxnub.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2zqydcqkm.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2cbdmjwnk.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2mlhagblx.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2zivnlcgq.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2qdlumrvf.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ktfzfzgy.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2twaisimq.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2nklfwnrx.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2xosvsjri.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2xlyvpitl.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2kxeiloey.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2vfszzpww.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2kuhacgaz.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2vyiimbhe.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2fiydetsn.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2bdwdsbln.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2qwxdlfcx.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2lhvuwqkh.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2dmpijoxg.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2qsfvopvd.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2qjgrsvxu.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2nljndrbx.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2yciitaxw.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2yidwviaq.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2rqbdxrtk.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2ajqqtnug.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2halrvqip.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2qjflfdeo.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2ifvogbkk.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2ikvqwhbg.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2isgkizfw.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2mykkfzbt.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2animzcmm.html


<!-- 参考信息 -->