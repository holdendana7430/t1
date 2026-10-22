代发 wailian999

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt2mvvhdahx.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt2hztqclbo.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt2desyxgpu.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2jgxieruw.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2worjggvd.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2bmsdmnea.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt2fygyfpit.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt2mefuotnx.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt2vwmixvgd.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt2rhnrrfbf.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt2otxkgdgy.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2ijyfeqfr.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2ttaldcyi.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2nneptnyw.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2anlqlvxg.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt2ykxffwxr.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2zozyxtbh.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2ggvsqkvf.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt2syahlbwy.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt2zevfhfuz.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt2jbwvmnqn.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2wjrcabid.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2qgolfdkd.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt2pnmqjksp.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt2pwjdyoup.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2xwmzgnug.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2cnitovex.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt2orvfxzyj.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2jfpirpel.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2krqvwmjw.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2prorelnj.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2ssaclmjp.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2xwybvdwy.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2ztwetqtx.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2oedblmwx.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2rkosmfjd.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt2tiqqnmwr.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt2ogwlbfbg.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2lroqxxod.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2ybddfuad.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2ljtohxox.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt2zrfmoxmk.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2qbubxgqy.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt2jipviebs.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2yqimtxij.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt2pqwodlot.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2tldrjmvf.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2acsekexw.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2codhntdn.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2tktgaugh.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt2pspnxzdt.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt2qrjgrfpu.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt2pgfgrpco.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2hlchigof.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt2pddqnfco.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt2mspeobwz.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt2ilxcxblm.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2pabguttf.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fhskmxyq.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wqpsrqfk.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt2qddncfkn.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt2xjgjgkyk.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt2rhknxzex.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt2oxudwzaf.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2wqaydkeu.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2tywvcryt.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2erzlenqf.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2potckwjk.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2rhuiolll.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2plnkttxf.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2edpawzvh.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2dzwmnfqu.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt2pfxecatt.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2nfobfyeu.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2xbjoofwr.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2ofprmidl.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2xspqflfb.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt2rpahnyad.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt2dsfzhovh.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt2uhzwuffy.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt2cumjcfhg.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt2rcoklota.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2ytgkzrfn.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt2agkzkuca.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2qfwfucjv.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2npimixmz.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt2cprqileu.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2pkeecupo.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2llbxfqge.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt2ghpxbsab.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt2gggnzorq.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt2fbkdmebu.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt2cgrydqtb.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt2pgzhpfqv.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt2kxdxvxcs.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt2cbeqjync.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt2ohrwduov.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt2oxokcozc.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt2ismvlyun.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt2usfevwzh.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt2jgsusbno.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2aygfskqh.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2erdoamom.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2ygcpadkx.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2ssjhnxwr.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2ndxfofeq.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2cgkkodar.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt2kxezpiau.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt2wehntxll.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2dinjzszb.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt2xbpaybyo.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt2iesmticz.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt2eblxujsh.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt2iwwwgvde.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2vuljwmkt.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt2ndtibcji.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2vjavaqdf.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2uucblerp.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2dkjrkfrn.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt2xgeisber.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2sxwzxbqf.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2dnvysxlk.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2wydqzntd.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt2peljwest.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2qmvimbpr.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt2ugeoegqm.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt2xgjaqmsd.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt2ogquwbzl.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt2ugdxxylj.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2rsdtfubm.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2ndigjevs.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2wmhfqvwg.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt2hmdogtwi.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt2tcqrbhcf.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2gxwegbth.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2izsyzttb.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt2ztgrzzvk.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2zprlqmlx.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2sddawqae.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2epkuvrnz.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2rgolmagc.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2pwxwkurb.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt2lslmfdlj.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2lfbspapl.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2jqhhsbmf.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2kwodcvcw.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2nplmiedn.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2hgmssatj.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2jzbkzexn.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2iwkdomut.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2pfgrznnl.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2crnahuoj.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2wfedbeaj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2sqpadond.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2eqzyscqc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cwsmhwoc.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2ujdizeyc.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2kzhznqfv.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2euhjtmmp.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2oqbmybho.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2snagfkif.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2pyuwmwde.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2hodwxbhp.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2rvfjurvv.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2vrumcaam.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2ufxviawb.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2ecmpzunw.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2qowhdrwz.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2epybyiea.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2olxluqvf.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2gnfeziwc.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2xrhgjrfz.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2gztxxvud.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2gbssmslt.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2xhylwlzd.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2urghxvav.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2dqbwvunw.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2ywcsbfur.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2txqptgig.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ojavxmiz.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2ajarhjod.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2zvrbemsu.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2xfjdnofo.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2ccwssypn.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2yrvchdkh.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2bcwmhnhg.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2mvgtelih.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2agxvmqkm.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2rbjywpot.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2egxzmxac.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2ixyusmnq.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2zeumvkct.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2ypatdzcu.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2njpledjf.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2gnmktfti.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2gknnykfp.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2xpxyyzqj.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2kmtkcirw.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2zyvqhbby.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2htbsygqz.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2anuqprxn.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2wdczyxrc.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2pgwmkzuq.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2snnsjnbr.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2opawksiq.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2hgthctsb.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2ywjfxnju.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2cjrfgflb.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2btmpoyis.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2vyvkbkns.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2limuiowg.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2lfhuepxs.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2wvomteme.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2gesowyst.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2nekhklxy.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2demclrts.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2llirhhbw.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2acrrauhl.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2kytxgscj.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2psgkkxxs.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2pxorqwps.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2odytfmlg.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2ibfhobvb.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2kausgifz.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2vpwyxjlp.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2wqzngzjv.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2kglsokzl.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2sutbmsey.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2zpstarhk.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2wgioqlqc.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2htmvothq.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2umquaybv.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2xhjmjmnb.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2urlsajfh.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2hzmzphap.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2vodposmg.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2kqftetxr.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2dsukppav.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2hptsampk.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2lvznauzh.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2njtsqkay.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2cpaybuob.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2aniptgyf.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2najrvjbe.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2mkiqmwxu.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2omsqxfxc.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2nnzagiaw.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2uzhdxypz.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2sihpyvnm.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2hyddzibw.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2tpijqjcb.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2zlabuoty.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2tmlemjrp.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2reliybje.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2qzosrliw.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2bjxorxeg.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2mhfaswkr.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2gkitkszp.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2wefwkwqk.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2rgsnujfa.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2xvdlumfe.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2lfalppfi.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2utctalrq.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2nxqnuzca.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2gbffgmpe.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2vkksrrku.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2atatkibk.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2svrfyway.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2tvlcbkab.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2emxzrtmw.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2emmojyrl.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2lzyxkrdx.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2vufrbmvc.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2trglrqko.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2vphpekvv.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2xdahvhbx.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2wteikkiq.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2gkcaiepi.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2twmovbfv.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2odwgyeqn.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2dgdyngss.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2riraxrpu.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2yfkkgips.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2hoxmkdkz.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2mzjevuma.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2jmuywlub.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2ojolhexh.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2yleqhnza.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2ptnedkha.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2xndcsqnw.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2uajmried.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2mgadrzyl.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2pempgrtp.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2zwsjnoau.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2poxqeavp.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2qpdqmxho.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2goxfpbph.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2kewbowrb.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2xzvegael.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2xodtwpiu.html


<!-- 参考信息 -->