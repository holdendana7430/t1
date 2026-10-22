代发 wailian999

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2ywyoatfn.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt2jhxlrasc.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2vsseqcti.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt2esgwcjfd.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2kuyswvxc.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2rqsycdjx.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2pecianzn.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2aublkrwt.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2azqqibyk.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt2atcfkzsq.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt2oywjrkip.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2datmysep.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt2orjabnjy.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt2cobmamyp.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt2btyehfvw.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2rlggjnye.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2qutphsyr.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt2xjgxazvd.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt2lzixzslk.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt2zogohpuw.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt2xjpctgxd.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt2eskvnarj.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt2qdsyjbgk.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2roigrsfl.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2foaiowrk.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2nthpdhwb.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2hqcaisku.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt2yuimbqaa.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2aofzujif.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2mdhvsirv.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt2tzglxarp.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt2nshqszrz.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt2fakwbgrd.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2rvgsrqqb.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2bewtdgtw.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt2ryvlgene.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt2cmfvzfua.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2auwphvdf.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2bhddyneu.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt2wqerlocy.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2jmecoddz.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2tkeslqkd.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2ytxinepu.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2cxlxpyxe.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2ugkdduoq.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2dbqlibcs.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2ajuthhlp.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2fpsaiwyo.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt2pddvyvaw.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt2nkmrbykx.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2gbcrdcbh.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2ulmewzkf.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2suladdbe.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt2kniqjhjg.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2xypnzumy.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt2ghafzdcy.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2qpweumtp.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt2zaldigbc.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt2aqvvvbhx.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2bwpgenqe.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2pynoyvnw.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2ewudceve.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt2blnfnmuz.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt2ihezuose.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt2uvlnxeae.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2izauuzgj.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt2oqrttwze.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt2yotxfakd.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt2lwqbxuab.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2reypjmvf.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt2haleefyy.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt2dfrpwiwq.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt2hfkypbsp.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt2agacjeqj.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt2tubywkql.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt2tqcyxazg.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2ebnqthrd.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt2lxyafaac.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2mjzwxufp.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2tduzbiqg.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2dobiofiq.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2mohqwndu.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2ajaefoth.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2qjvecoxz.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt2iatpjdad.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2hldrnerp.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2xotlqotx.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2eihefugh.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2rrioxaua.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt2pqrtrndh.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt2jekqdxil.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt2eixqzcxs.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt2flimhtss.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt2ugbtwwki.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2xngcvbka.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt2rnlapkpe.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2hpjbhvjo.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2dvlbbefq.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt2dmvkeosi.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2jpyxcqip.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2qmfuwhbr.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt2caqbyxpl.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt2jiecjzcy.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt2mebkyhbx.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt2srjqkyyk.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt2qmputsjx.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt2obhzevwk.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt2hujzixvm.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt2wgihesqs.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt2cwprpvtt.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt2penrwdcj.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt2mwyoarhe.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt2ndyavusj.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2rjemiwrw.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2qezlixoc.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2ivycidmz.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2uajvrjxm.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2tncamakj.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2wstxxfee.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt2yejkenwk.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt2acovbspw.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ralndjef.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt2agjlenyd.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt2lvtpzpuc.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt2yzltlsct.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2odagqfnl.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt2oyqltvix.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt2jdfwppvr.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2sditjred.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2vxlusono.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt2ndkkpsan.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt2uxuwhkcs.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2klbdthyj.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2qoxrgvzl.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2lvcbsslz.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt2jrrisduk.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2mvynwhmv.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt2fbvpycgw.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt2ywsqvxxr.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt2xmbeqkvd.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt2spmzhwkb.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2hqblseyv.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2cihjwgrj.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2jpvlyguk.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt2vjrtgnvw.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt2yjzlnmwk.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2dmjrktqo.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2heiivxey.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt2utvgdyqb.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt2xbsdirtt.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2duqdkarb.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2mhsemwaj.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2gwiqglwg.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2gzhrgjkf.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt2amencnab.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2coqwmfgh.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2sdiuqizy.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt2xjrnotca.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2qerowaki.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2mvedyckq.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2smebgcun.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2kotqeoee.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2xwivhbnx.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2jxyjahcs.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2agcgvfzv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zqcddklw.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2lydfndqe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xziekrhx.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2ywronwee.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2yxwkrivt.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2zvqluvby.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2gblwruuf.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2qyvfbpmp.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2oiylflvh.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2ctozgdcz.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2dziuabwh.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2fjejvocf.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2lmawnhzl.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2wxhhckfp.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2uyxtbjqp.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2meohgxlo.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2qaragokx.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2occyfrak.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2ochilxez.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2jbbtrzli.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2rfcmpelg.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2ijmyjgni.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2silyismy.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ahmccinj.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2fvlnctnk.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2rspsvjka.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2cxcgekwi.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2mduqwuux.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2iywkjbbe.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2leyirszp.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2wilitlvc.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2vihqoypl.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2koxvylky.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2mjpipffd.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2bmclgyhh.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2wwohixww.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2juqvmflk.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2sayjewjl.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2ccmhfpqu.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2xkerjtmn.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2vwmppnhg.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2yfxedhku.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2crqrtwfe.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2sqrvrphc.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2ackucfwe.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2kmanduuf.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2efeoghdp.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2kpqtefhd.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2ewcwndvs.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2bgxbqnjq.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2gdfinlhp.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2vwltmrbu.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2qhvrngmo.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2jkwulkhg.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2whstgfat.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2somehptl.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2josgqmko.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2vkhmhkqy.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2jbarfssl.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2rfxkszxm.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2elbmltdy.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2cynpswuz.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2rtopqzha.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2tkxdzvji.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2xrstesic.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2hbckrgvk.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2bjpoaysq.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2rpjorxfu.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2ygdkdhrd.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2imdetxyp.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2wykruvml.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2quzmkmyy.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2xqjzjqax.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2jfejvehv.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2tykickgp.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2cgqukpkv.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2rnqowasm.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2oppmvpim.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2jejfjgnb.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2zcnawiqf.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2phfjhjmb.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2aatxvvgg.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2wyzpdxtw.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2plhcjcun.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2gsgikzmd.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2ovhrwgox.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2cfznbxhs.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2xlxjpfvp.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2xwimntsj.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2jankvmvp.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2xicrzhph.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2xhxtmjeb.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2nneqeljh.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2xjsbnmdv.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2ugegcxap.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2sjwoblpt.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2uzdpkfhv.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2vxvmbwyn.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2luhakcnw.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2ndffyhaa.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2lepsrvjy.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2yrawqeqq.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2zfohusxw.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2ygfhoktf.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2ikvypsou.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2wyjzwdzd.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2ypwfjljx.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2uubslrbt.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2wdngwule.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2accauldl.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2lpwnsyrf.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2ufktguql.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2akkebyzo.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2qykbdscg.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2yvfmebco.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2hlasguha.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2szbzsthe.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2synyojak.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2hlbozcia.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2wkjubiet.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2fpnhotxz.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2cctztiqq.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2tfrprxcn.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2dxomfvjg.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2kjtqlxsf.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2rcyhnygu.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2dmhfnrkc.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2lfxzbbww.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2dgfplntj.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2ifxlewkb.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2efdtftpx.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2dkdesiay.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2zkbviiwk.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2cpadsiyk.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2ecetyuos.html


<!-- 参考信息 -->