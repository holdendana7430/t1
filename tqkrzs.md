代发 wailian999

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2pguhnydt.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2efvxfrba.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt2ypixkajb.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt2oplzmdlp.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt2mkztggre.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2eaxqenao.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2pqgtuvgs.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt2jbvejowf.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt2zifsqocl.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt2tziiqnji.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt2szetxydt.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt2jdiumxbd.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2vflswykp.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2wdiwgqyi.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2omgmafma.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2rerejzcz.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2nfmsccff.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2cdhxrnyf.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2ttqjxole.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2lcjnczho.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt2rklykspw.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt2swuhbjej.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2uvitiigg.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2agiljvzh.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2viwiosph.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt2rakryyvy.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2wkldpzol.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt2poabayie.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2dxhuigau.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt2fqdchenp.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt2nraciybv.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2qujuubhq.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2vfcrvzsw.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2dyarfocu.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt2carquipz.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt2bdtsmglw.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt2tbgbxhgi.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2hizmiohn.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt2tlqrudxf.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt2vhvqscor.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt2aorrkqei.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2spyyuqyi.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt2gevkefds.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ygtlsinz.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt2dmjbfusc.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2euhrwicx.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jpxeaadb.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt2dcwqdvxp.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2yhjxtncb.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt2ekwakqus.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2ruunxkbd.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2qwrlsgtc.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2odmaxdmp.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2ojnoxbfg.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2dkjqkych.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2vtjoynad.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt2nowyjeog.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2zhvkrkxl.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2rbjldwpe.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2czjfprzi.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2mpwlmqsf.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt2zmbxhwuq.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt2nuqitfud.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt2rtoddqab.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt2wmkmcifz.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt2rfqngwjx.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2csgzfldb.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt2fiaqfesb.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2ocjxwany.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2rdrsudim.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt2vawjariu.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2whziippx.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2hvihsymt.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt2vwvfwmdn.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt2qzinyiyl.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt2fuvefpck.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt2ueerksyl.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt2ldzfvcbj.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt2hcjohuuv.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt2pjauegdu.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt2wdtmaqtb.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt2ggdggzac.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt2enevemml.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt2awrgqecc.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt2glkxbjpw.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2fdorxxqk.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2xtlhujwo.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2reiehgyp.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2devvgoah.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2tsqzcrfx.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2npsrewdi.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt2ygdhnljy.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt2qljztajw.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2qtcztmfy.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt2qszaucji.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt2mtdwscqb.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt2nbuniaew.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2anlpmyta.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2hbwaefmp.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt2aluzvsjy.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2ddnbiavn.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2rqmhvlej.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2swyikgmj.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt2tllasrjs.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2cvwllzdv.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2wrzkarap.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2iwjnkpxa.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt2wtpaxeng.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2wufflszq.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt2xluncsso.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt2uhobreku.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt2aepeawdq.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt2lrsqdslb.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2ustlevbc.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2wscnfbhv.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt2gdjdednu.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt2rpciscvn.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt2naevonkl.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2ixllwzso.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2clfongme.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt2oongkqbb.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt2vwyagzmy.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2kgktehkp.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2frmdxulc.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt2vqjaeboj.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2madcoyql.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2ufixaqcm.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2bksnlwdq.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2tmtrmfjf.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2jlubfwmo.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2njzambqe.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt2lygxbdnx.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2upkzgbxb.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2acptyecp.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2hafbpufj.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2aimkgsau.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2qylrbpya.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yucosupq.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2ralkkide.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cwwuzurs.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2kjslyqba.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2plmnjnwz.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2kpevrdpl.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2jutteewd.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2bncppzce.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2lhmhlviq.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2zapjnmcn.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2dmpbpdrv.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2iqfwjryz.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2sqfnpllv.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2glsamntr.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2cehotnmg.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2oxjgnfst.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2mxozbxpm.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2hzrbmlpm.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2kgltbufy.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2ptwhyiev.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2zjiadnop.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2bgyaieym.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2rpkvtbjf.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ezmdavpc.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ojmttrdc.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2htecypej.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2gaatbvjc.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2sbcgjtji.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2ovbmlxlw.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2rdntucwp.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2vjgjgtoy.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2rdeaopxi.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2rhdggjtk.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2vsylumae.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2sqikxfjy.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2cfavbefw.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2uquzodcd.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2rtyuaezm.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2oetrsqfr.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2yasvdudt.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2ktugvrko.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2zoglaeee.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2bufczvls.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2sggglxkl.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2ytrlpahc.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2wbxlrpmd.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2eawpjpnk.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2ksuynbyr.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2sewnshdw.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2dlhsradu.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2rnhybhuz.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2ktuwpjqe.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2lvjhihqx.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2huxoucrx.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2rvfcvqpt.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2retqnuyz.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2umfzoozf.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2bspndoma.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2irnsqdcp.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2wvqnyytu.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2mccmbapu.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2ehiqfyvw.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2osmtgfbx.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2eaoxbovc.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2bgqctxkf.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2jiggeysc.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2jddizvho.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2zzknotny.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2errbjwse.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2fstryaqq.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2zviskkqr.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2jihgghep.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2gefcyplz.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2ljnckjlq.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2zforcmwx.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2faelciax.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2dzenfcee.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2bvyzbdgo.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2wvrezxer.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2gwhilbmi.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2aiuoicza.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2xxznzlav.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2iciyztfa.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2yidmuggf.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2ljeuyuvc.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2hbnmcuxv.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2tsleshxq.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2fbnnwqrp.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2abwkwsrd.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2klbpopzv.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2wrijqbmr.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2avrosdqh.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2umqsvrit.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2daulgypd.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2ldhgzbxi.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2xrgqglpf.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2zapehkmc.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2vzmfdped.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2hursdlai.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2ssipvpec.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2pkurcphz.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2houcvbfx.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2ucdxchyx.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2qeaelzgh.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2kmztoqil.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2ldewxssx.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2koccikbw.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2jbvjpryr.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2sroskypt.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2vovwbply.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2xqbsqmbc.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2titxvojk.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2facsjbhc.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2buyuyuei.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2xflemqre.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2oysimees.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2ppqiwoye.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2fxaewdph.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2ustvalgx.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2frmpqoog.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2lodfmiss.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2haajfaua.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2wbhzlwgc.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2hqvrooyy.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2evwqywkj.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2qqdkonvv.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2nesmxjvw.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2gwnnjzii.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2hjitykdx.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2wtpsdldh.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2rpiuqowb.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2tidiowfc.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2qqudfbbl.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2usxcwjkj.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2dvyiikua.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2ezhcaqzl.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2nxhneyak.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2dszgixhg.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2hsujfybf.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2gyhcmzhe.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2mnzvvvpc.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2wmmrqtpb.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2kcjpoivl.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2vhhpzvhd.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2lrnfskos.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2zimqwxdl.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2vcjlsafv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pngfbhav.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2resyxzle.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mkzlnmzx.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2ygpxfwyn.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2zvwkesmz.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2ejbnndyg.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2lnvejqje.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2tzywsdxl.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2boutkbyl.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2fhvshset.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2rjcrxcda.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2utrkdbvo.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2takwnkml.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2xexfupsx.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2cmybxeum.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2hrxpydok.html


<!-- 参考信息 -->