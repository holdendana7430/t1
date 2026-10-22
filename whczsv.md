代发 wailian999

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2pwzuztck.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt2sadhdkio.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2ibnddsjf.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2qfgimlyt.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2vbgkbxzm.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2kkwnpqis.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2dgbycbce.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2rsfcdsoc.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2dhfjoefx.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt2omkexnae.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt2wffvphtx.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2sjiivzza.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt2olwrtiwl.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt2vujpkhdw.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt2kyixirsy.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2nnimsswz.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2hyljjvvh.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2hgmrhhkg.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt2egzsytky.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt2mvmzlncj.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt2gselttnd.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt2tryjyvnm.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt2hktayfzm.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2xgzhkrxz.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2heknsufd.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2jsvuggxp.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2zaybkgxz.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt2czjadkzp.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2tpqtkqfj.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2mlepejtv.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt2xrrrllrc.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt2heyiprlb.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt2sefovosm.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2mzbeokka.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2wsuojjtr.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt2aswdmmrj.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt2bwbtqnqu.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2ooudmnkh.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2lizcbzuf.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt2nsidbvbj.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2gwlpyflt.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2xxhgkvcf.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2vaunbcbf.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2umnadwda.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2bebpzpym.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2falrubyh.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2htibjgmw.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2aslbxfft.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt2ebvlhxzs.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt2naxixtck.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2dbcparwg.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2zrdnejih.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2olkmisqr.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt2dbflzqwx.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2yunvytmq.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt2mzvgxnof.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2cjgjsplm.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt2zyoytuzi.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt2ffkwxhki.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2fqojvgns.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2imeweekf.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2bfcxhqkw.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt2evotilit.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt2bppkxaqq.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2anncppbl.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2wlkldnbq.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt2cpbqxkgt.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt2ympgbzzs.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt2kwywitge.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2tpkfrfez.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt2jbpoktun.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2csqjkvth.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt2quhiszwd.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2lddvdllk.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt2sfkkfiar.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt2bfxtrpqv.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2ceagegfp.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2wimawibx.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2xjpujgxx.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2nuuvcite.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2fxtoddtw.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2jombxilv.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2caggzxhl.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2cnezdxft.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt2kdorijga.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2qgusmfbd.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2irfsbrot.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2aonnjtzg.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2dihyxwud.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt2bbvnqjxv.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt2aexxyzrx.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt2utljhsyn.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt2wrclhnpw.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt2aqkkxrvh.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2gecneifa.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt2kqgftiux.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2lrkbvyji.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2lvnvokkn.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt2oyuznlyc.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2datwviex.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2uobvnkhp.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt2odniemxn.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt2fnsnwvjo.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt2claubkmz.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt2xjekcqyv.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt2wrjaasjt.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt2bjuaobsd.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt2biruljjz.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt2kvnehikk.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt2zeckvpns.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt2srglvhxo.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt2bjbfpuch.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt2hwvniobc.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2vntugipy.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2cdqjuthc.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2qjpvoonp.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2mslwdlra.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2opktgjfb.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2uxakeeev.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt2sxjooscd.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt2cuwatpjw.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt2nmbkxave.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt2mxtgcvon.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt2ixfcrtgt.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt2gptcqsbe.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2drlpagqr.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt2kedcevgv.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt2xfwmxvdn.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2xwhhjeqy.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2awnibmjj.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt2qellgwhc.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt2lfrdhsug.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2csngsudo.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2ukokqynr.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2cvlqmrbq.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt2vfrfyile.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2timmpaat.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt2ucrlqaln.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt2ffusxcif.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt2jovygbxc.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt2pzhbbkvm.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2lxjshulx.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2nzcomyyv.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt2tintdlnq.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt2xlplecwh.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2pasvskxj.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2svnheoxz.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2snpgbwfj.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2ywfqtxth.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2glhbzttw.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2qvxmdplr.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2ntqnwmvb.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2tapdivki.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2wnwvtcia.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2mvlofeww.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2axjecaxx.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2guprhhyn.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2kajxsnzj.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2xzafucxs.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2mwmnertx.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2agalcrpd.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2ojmhikhc.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2jenvfbri.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2vvztjyso.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2asbiokcn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gvtcmqmy.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2fmkxcbjn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2radqcxrd.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2tkhxlqne.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2edzcomhq.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2daagczqr.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2icnhapfv.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2okejletn.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2mjjtyhyf.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2zxpfpmcn.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2pqimdtbz.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2dijphcvl.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2umdbbchj.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2dswxiwww.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2vffbmkdn.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2umjemolu.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2eqktmpoc.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2mtzhgjad.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2nnwfgaki.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2ovtvkhzq.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2lzfuxyrv.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2bqxtqpsy.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2poxsnbur.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ovukwrrz.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2cgzkxdto.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2cupaslne.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2pisxvitn.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2pyrcpqca.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2zosectpw.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2afperebg.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2myynsugm.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2afmqkqjk.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2wdywazfk.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2sxdiuauz.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2jfiberte.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2ygfdusta.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2xmmaazft.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2liohvshu.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2cfcvfrdh.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2umindlsz.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2zixbqnrz.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2ykofqjei.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2figfimof.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2vhdqmkav.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2bjxbatnl.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2aprydugf.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2igekpqxc.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2knpwuhkr.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2rdnbssvk.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2egmjfpxr.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ffqokjue.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2jowzynwr.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2wkhybxzy.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2cxjhlgwd.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2xwrjykqr.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2kxcazsxj.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2exxrmgeo.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2xnbcoylw.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2tbtiaobe.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2kkodjkfw.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2jnuomgxu.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2gmnwqmav.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2dlrwyrch.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2upvextad.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2gdpifjnq.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2useorneo.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2pemzoxoq.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2zjyanmvx.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2fxqosffk.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2oycvfqsg.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2ifktssgp.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2jamphqim.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2ckxgrulj.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2dmrnpuci.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2bzshllzs.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2ekujkgpe.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2jkbebvkc.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2goqmbpgd.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2tmmwnlzh.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2ghyetnwz.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2acrqwssb.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2ciousqsk.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2sznweajo.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2gdrqdhlz.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2sppyuowl.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2edvtbawy.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2ppmawkdu.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2dcmfebyg.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2hqkzrmrz.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2iwjefhvg.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2rjwdfqnu.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2kniehixg.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2kotwwnrk.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2gixilemg.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2slyhqeis.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2dhstlioh.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2rireryyx.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2aetpivey.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2vvhhdnfi.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2bcmgvngp.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2qhatyhui.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2oohgnbev.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2wphragxj.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2fyfncnlp.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2norisocf.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2pamcplvi.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2unsilvsa.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2mlzpytpd.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2codkugum.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2huovkrbp.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2fhhzywzd.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2mqmdcmxi.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2vekpnyya.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2bhzwrada.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2cuhyhizw.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ideochld.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2kzumrfrj.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2bisjjbyu.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2ewemhrfm.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2mbwqqgpy.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2vtvvnprc.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2gtapjvmv.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2vxhmbvwj.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2grirqyzh.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2jylrvxop.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2tjmshtvd.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2afagcoji.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2paiuzomi.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2qxjvpllu.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2apmixiwg.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2wcwwvlut.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2cozpmkug.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2qglrkuxt.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2bodioplo.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2jbuqejll.html


<!-- 参考信息 -->