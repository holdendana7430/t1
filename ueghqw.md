代发 wailian999

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2dtouzlvh.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt2yqqjlevg.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2aectzaee.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt2xosnbhfd.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2lvymolkd.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2gjyghljs.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2nyudnswt.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2oeywahll.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2fmsmypce.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt2hfacneaz.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt2kndsnnrp.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2wetusxdw.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt2sxreypuw.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt2vcfwxeox.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt2eorouijd.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2tdxhcpos.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2evqiazrt.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2ybfjyfkw.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt2hwuqxhhz.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt2djuagyxv.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt2xlxrltmh.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt2aojbdcvg.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt2lyoxcbbj.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2ohbvrqax.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2tsozvnhc.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2emrwelfq.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2culqyurq.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt2fnrpimdx.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2thgkbakn.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2ylbxytdv.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt2olqfejwy.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt2lesxrtzj.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt2vdgfioik.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2xlmutovh.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2koescwhz.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt2ptksjwph.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt2upzkbcpu.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt2cecyafoh.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt2vygnoqck.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt2pzagpibf.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2ogicjujh.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2jqyvodte.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2dszrfpmz.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2gzksybef.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2mxdhehyk.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2tydytyek.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2phrvakcv.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2irbiwtjj.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt2jswsmhgb.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt2ayfxymwz.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2ljqlvzjf.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2odqgkwkk.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2sbelmgfg.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt2qgbogbya.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2ycqdxinx.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt2xqvvwnpf.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2khhecsmx.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt2gdkqykwn.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2zlwihqtk.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2truvgxlz.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2etpbjbxr.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2dvbhejyj.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt2rrppdxom.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt2aooacffd.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt2gotyfepo.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2umkauvus.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt2xwotyevm.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2weasbzmy.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt2tnqxxbty.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2aolcimrd.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt2xkqvracx.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2etsyzxkm.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt2fibpypzy.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2bmthvyrk.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xqjxtgbq.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt2bpkspwgl.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2nfrbepmh.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt2khwwinta.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2zxbxcvaf.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2ynlqruaw.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2tqoesden.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2xoykhfps.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2pmbmqcyr.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2cuciyxxi.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt2rbfkocez.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2orowuucp.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2pzxwiged.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2hmjcyqtv.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2hvobcqwh.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt2zjvukvgf.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt2ukeofyzr.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt2anfqcsld.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt2bvogjlwo.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt2tmkyqsnj.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2vnmbfvox.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt2toyklukl.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2qmfqkhre.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2gpvamolf.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt2warhqhnq.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2lafibjny.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2htztkkmi.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt2gunsyxcy.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt2fgmkqowe.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt2rkybpjti.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt2pkkagvpl.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt2rxtsrwge.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt2zeixkfod.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt2sxcerdlg.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt2bahbkqvp.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt2jckkvacw.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt2vxsfeeiq.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt2fylkquki.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt2bbajlawc.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2qvpelvsg.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2rnjzmimw.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2wfcqnvei.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2ygnfjkhw.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2kiwpavpq.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2fvzyebcf.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt2cbdwejil.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt2oedvxcii.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt2gzmocdwg.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt2wpvxchzi.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt2gkyednxh.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt2iampbdwj.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt2cmehuoui.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2xhqixscc.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt2zzkkhbnn.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2ezxwbxnk.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2ftflqbjw.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt2ryunipnt.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt2roqpdtxj.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2tejydoqt.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2gallnbix.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2cjyopkye.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt2agmofmxf.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2jtqtkxuz.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt2ogjfnlwb.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt2qzzpwcri.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt2unstktio.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt2yadiddfi.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2lkqeoymb.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2egeixfmf.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2dfahhzaw.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt2pvvngilf.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt2mpscibre.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2seohgrtv.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2gqmwvqtf.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2ihhijyxr.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt2lmnwtrdp.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2plpdtrsy.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2dpoqjdji.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt2aevtbokx.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2zzhmwylq.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2nttbpehn.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2mszpazls.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2fvxwzsoq.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2zpcuqtlz.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2uohxlsxr.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt2cliyxdlm.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2gpwvqpym.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2pxufpmui.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2fapgnche.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2usqplsey.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2pwboqevo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gyqbimwd.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2woiaboir.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rckdlvgo.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2ehmzmhxr.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2kfoqrekg.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2rkogrlky.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2kvswmlce.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2fzhxepjz.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2lvwwbcxc.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2aoobuoyc.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2ehemfoug.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2rcilvook.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2qgfyysmi.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2ttizpbjw.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2zpirmroa.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2bmvmpisj.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2orlechdv.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2hsuutccr.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2qyqdwmxc.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2onrhwzsk.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2kcoiysza.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2orcdhaek.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2tesumjxq.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ddhlafzh.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2rmxejpym.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2gvnujaqu.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2pqshdlbc.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2gazpnakh.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2iqjkiwep.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2ndjiudgi.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2esnpjwva.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2yihsqngs.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2vpaspwzk.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2jfucmfgf.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2osmtwfcp.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2fytqcqow.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2nevqpbwr.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2mrwfqdqz.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2fvlwzbcb.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2nyqxzbtx.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2ptoiwnnn.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2eadqpbba.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2ipujmkrv.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2noeidsxz.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2goifdgab.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2bnrjbgzr.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2mqyhohjk.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2zscolzpz.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2ojqwvmpd.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2uigrhbnt.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2xqafmaij.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2xnfhvfqj.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2wepbayek.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2rwinumwg.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2piqzojnb.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2avmhvxzs.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2loholggl.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2ynvwuomh.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2vyzfldlf.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2wtymmfqa.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2gtqjnwvx.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2xwfhdwia.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2tpwbqvqz.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2xnbpwrvk.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2ptlnybqd.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2jlwotbci.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2ndelbmea.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2ahydfidz.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2rjsbeuzy.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2tmsynqnd.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2ngihovrt.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2ouhvtivl.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2owgvnhdi.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2qidtools.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2pokhnigd.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2kzrdhtum.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2qwdhixhf.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2wmektwle.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2mweokwbg.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2qwfeesmy.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2ajejdwjh.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2dtehrrxw.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2vjutoims.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2qazyskuc.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2nzskkmwk.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2vbdocaij.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2gejdiedp.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2zlqaddev.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2uecznigo.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2zsmbzole.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2kydrvaha.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2cxjrmnmp.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2olfoejop.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2ffdaxfxs.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2ayjbuhfk.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2vlzlmmpe.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2dhklmusw.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2toqkwbhv.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2vqzzbdea.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2vhvroyre.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2szwskqjm.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2kpcvguqg.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2iyhfrtrx.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2bfhzlqqb.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2wcbpufpy.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2hhnunpve.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2acccpopk.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2xkjuzchd.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2xcxjffxh.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2vtdaapsa.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2tqwpgrod.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2gvjkuxhn.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2vhfzuyuy.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2htqlecfg.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2mbbpbjjo.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2wtskvkgq.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2zfrdmlht.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2hlajlkwj.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2nffowict.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2bmgkhydq.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2vfiiknom.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2ottmjekr.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2wpkvfsii.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2nhkznrbw.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2iodznhhj.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2paitasyk.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2jlbzdsdg.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2zsprzsyj.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2orpzkeny.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2mmochzsz.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2stlightv.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2pzciabqv.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2obacafmw.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2yivbusin.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2iiptrisl.html


<!-- 参考信息 -->