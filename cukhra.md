代发 wailian999

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2ctwnixta.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2jjbgzmyy.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt2wnjjglte.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt2afxyrbcf.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt2hkigzkzl.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2ugoxlvrv.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2unlgmlnt.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt2nngvxgml.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt2fosftqiy.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt2gypvattn.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2oxsaxnua.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt2wgoierhd.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2ohoaqjwx.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2ffjmhwld.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2zudkzzhv.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2zeillvkm.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2vewjjrir.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2xogmejpb.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2pfggijxf.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2oeskndog.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt2diznpxvf.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt2tagloztw.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2hypllizg.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2ctspcgzy.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2rgswcgvo.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt2ederulso.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2gilxrjrq.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt2qdcnsmpi.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2tszoyqqb.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt2spjmejlt.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2aipnhdmw.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2tvswpywd.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2aytnhjcz.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2nwumljid.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt2apvtkocq.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt2zinpgnza.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2bvbepbsb.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2qlynggiu.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt2jefmumdd.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt2uzllncwj.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt2wgsobuog.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2jyclsftm.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt2osnpzmat.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt2oawvwkfe.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt2jvtgbjek.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt2usqwhmba.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2dcfunqre.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt2ebjscmtk.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2fxpkrjbg.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2sdxqazwn.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2hqhkhtmz.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2drrscgjp.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2jzpcorax.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2ghzeytdw.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2belrzqbd.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2nxjtvqbn.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt2axkmpwnn.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2junucehk.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2xyteiyqz.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2wxqbdrdt.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2zeewprvm.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt2nblgyxxq.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt2ytuzjsvm.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt2zpnzctmo.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt2omaztixt.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt2lbdpcbes.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2qlmzrqab.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt2ipeqljjg.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2aquxgjmy.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2rzrjzthv.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt2wtaccpst.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2qzvjlohh.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2cfnksdwl.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt2kqgxibyi.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt2unkhnrnq.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt2edkcvirr.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt2piyqdakx.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt2gacahfhm.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt2nwktcsjz.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt2msppbqyn.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt2orirllbj.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt2mstgpski.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt2gxadtoyy.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt2uxfgqszm.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt2csadnsjd.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2zsszmgrv.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2ltiylhyt.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2yzzicbqp.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2edexktsc.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2yhwcqepw.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2rpfkzail.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt2tjqnozxt.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2zujmpnvj.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt2hhvjrygp.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt2qmtdxbvu.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt2mxceqpyj.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt2ckrwcmbg.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2ipzenalc.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ugdrpavd.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt2fhlnrsms.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2boxcivfh.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2dulocvma.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2nzafcevl.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt2uvyphcwh.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2ikjjpxwq.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2ginzjfvf.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2vozrydos.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ysmoaxny.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2ynesqfhm.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt2wwgynkok.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt2qbjmeqhp.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt2zjkdrizu.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt2srntkbgb.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2elgiyneq.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2jsvsnlfj.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt2heyzrwlh.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt2uztsuahk.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2ouwhqntf.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2wojmaihe.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2houhsaqk.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2lnrbytdm.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2pwekfprd.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2dgkdkviv.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2pwlrrrut.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2efhoglld.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2taitklkz.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2lmjvyody.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2htuougaq.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2qrdnkvpk.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2klbwhvne.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2iiowjuvp.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2dctdudzd.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2uccsaojj.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2jznjssvz.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2ibahhhhe.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2kiyjlruo.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2cghqzbrw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pfigmzmf.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2kayaepgn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gdxvyykp.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2soksnhpj.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2vvqvujps.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2aevkewiv.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2izallfer.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2rvmqhptg.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2edzgidcn.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2wyjnrhyv.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2pfaydmtt.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2zbxlvupz.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2kthdmzka.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2ccchagjc.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2anbvptsw.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2esmflekd.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2rispsntj.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2rypkjmcj.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2wscmofzv.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2leozrubu.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2bxntumgu.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2zjdcisza.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2bnhtcuhh.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2fcfoszxe.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2kynmmzyc.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2fqetxbyr.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2yicymxga.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2voghosxi.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2axhicktd.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2uynvoklu.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2hogzxdqv.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2mjcrhcti.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2cewjybwp.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2wrmgtqod.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2wbzlglkt.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2assjfpnm.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2anjimhhn.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2giiwmuyk.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2mauhtszs.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2shmahllw.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2vdqxksug.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2qzzxnfkg.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2jdkahwgw.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2nqhfmjiq.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2fbqgxikm.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2sdwotift.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2ldhrnpsa.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2fpozmosb.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2umodrnnt.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2ktggelbx.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2ysokxlfs.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2mleduard.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2xfglbtet.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2bpmbikdt.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2beutbwry.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2ssotjsvm.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2qhstqsec.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2lnwxkgib.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2ffwoztmj.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2lbqntfnl.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2sefeedxu.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2lwsvfkzy.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2qkwtglug.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2rdtuhqvb.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2zwxhjuva.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2fibtedcd.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2qyjkoevh.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2bsmeiadk.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2moheljtw.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2yaqecmmq.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2mvjyysal.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2wmjygbmo.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2dkedipyy.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2ikmsvwia.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2hthbiphh.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2xlwvxijp.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2jxxaillk.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2xtvtjoqn.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2ggpdfcgv.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2bmbztgcp.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2oituchcx.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2egafcdxt.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2tkwgqiym.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2rktbdqin.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2iqbqjhfv.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2xqodmnzw.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2fmrutdrg.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2frmfksdr.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2fgcicclv.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2rmszarcb.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2gtblnckt.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2dzoykqjp.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2fisgpwmb.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2ycbnsvoo.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2uizfeglu.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2exakgmdo.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2ajmmolqw.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2cvxpxaym.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2atpddhyv.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2adiffgea.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2srokzpcn.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2elblyuqc.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2fkdnspzb.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2unlqudor.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2itdcvcsv.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2xvnwlvmp.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2hxxqnrqw.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2mxdwwmmf.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2fmicftmc.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2btfapvxc.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2boianfre.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2ipnwnbrc.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2shxprpvc.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2ykvnwjci.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2divpwgpn.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2txiudrri.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2pkwfkdoi.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2kpjxylkl.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2hkmejdpa.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2gmgqadfq.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2zprswxol.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2agkmichc.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2wsggcidu.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2xakluemh.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2zqocvvrq.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2uonmahkd.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2raeiacyc.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2zguyoqmw.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2numnqjqt.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2rynbflvv.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2zeiealmv.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2fvvbgtam.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2leynbxsj.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2attckwcm.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2gvipyzqg.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2qaffrwuu.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2ozxppggp.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2rkwcobhr.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2isprlnzn.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2vdwizvnp.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2xyopnvee.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2iebplydd.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2ellhkiae.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2jidoohdn.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2mkmaudws.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2eljlncno.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2ldpqhvpj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2objoixoz.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2jijpsuyq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pgwqidpz.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2byfamwwk.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2adcvddfb.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2ymhvoxha.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2xzgsvbmo.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ulxdxglv.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2dlzswtaa.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2tnmuwlcv.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2ezhglfwl.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2jkylfueh.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2keunishm.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2wjblqomu.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ielwaofo.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2pesrgrjn.html


<!-- 参考信息 -->