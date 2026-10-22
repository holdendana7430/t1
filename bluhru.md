代发 wailian999

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt2hyckglpn.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt2zesvvaih.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt2wzdlzbyk.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2rzymddig.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2afbyuruz.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt2aalfezbw.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt2hutheaot.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt2xqeordpp.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt2lfmeedvq.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt2hhyncezy.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt2cqzltmdo.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2vkxgxyfi.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2bwsjfqoc.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2oqolrksl.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2rhezvdcu.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt2pizloavs.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2ohcayirz.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2mwwhyrom.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt2lsecwuua.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt2mwktvjpk.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt2uhbkupwk.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2hhpbuyzg.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2rzlsoylb.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt2mvljcual.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt2vaxxnepa.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2hscwmbls.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2brktwqfq.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt2qewdghis.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2qmhmsilw.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2abnwcyxa.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2wdudwlbv.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2smlbsfwk.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2woxfnjwj.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2tmzmzqfm.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2ajwwahej.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2coiogyyd.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt2fiajklbr.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt2dopobwmb.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2corhvgwl.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2plpqdthx.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2pdrhycop.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt2ochloyrb.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2ufrlztty.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt2ywwqlmeo.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2cuvhkojn.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt2rzdjwbfz.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2baxdqrrb.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2ueycsoyg.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2iokynegv.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2msjytxfh.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt2hnvihewb.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt2xgwvkcbf.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2lduaqann.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2avsgchti.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt2mbncssqj.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2vxbrhgxd.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt2lwcrvfhk.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt2oeqqxnis.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt2zmiwnwvy.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2kubwfule.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt2fpxxxeyo.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2gmnrngbl.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2veuxgqlx.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt2bwpyszsw.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2tqgehbaq.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2oawwzkeq.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2ccbctdqe.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2qrjkxxwa.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2nuhvrfej.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2ajmxjeaw.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2krpdrfoj.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2axqdilra.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt2jtzhcdfs.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2jwbfnokb.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2jcxbkxtl.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2olgzlxsm.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2aahhgzgc.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt2aktlculq.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt2xqlupdbu.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt2pnelkyax.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt2hqszjtnz.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt2dngrravd.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2wtwyqnea.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt2qyooyayl.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2rvrbblcl.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2knwhxyey.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt2joibweki.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2yczveinx.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2fohvttgq.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt2hwzlbedp.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt2dbzugehn.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt2oijyrpfv.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt2rhehdpdv.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt2peqykqeb.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt2psucwzus.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt2nucsqmik.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt2jleljsba.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt2aqcyknir.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt2kfalerxb.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt2booqipzk.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt2uibiorfa.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2aknarqsn.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2udueggwm.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2dzfjwbmb.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2laqukbtm.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2niaamzal.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2hacnbwpv.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt2idkjqdhv.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt2kvnffskh.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt2njmhhhnp.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt2wfotmqjd.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt2rurwurvj.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt2qlrjglro.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt2uhgypjvt.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt2zrfahxga.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt2evsbalil.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2qmtimcer.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2bmvpsghz.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2wvospwve.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt2bwrtyekc.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2ddlwqiqo.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2wcxdivjm.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2vmlypges.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt2zokrxlqa.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2lezjingy.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt2jyqbnwcc.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt2hntmmixx.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt2boxamkcn.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt2khjfxfvf.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2cpfcscda.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2nqmrsaik.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2sfqocrol.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt2xnkhvvym.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt2pgkexmdp.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2gslggeeb.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2naoqetts.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt2xmhrefdp.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2gvyjrkog.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2asgdloxi.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2lwzhoswf.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt2hbolzvdc.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2cbluycte.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2wpbcubhn.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2duahxnhz.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2qnzcoobn.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2enbmqsgq.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2kuikuyuh.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt2mpvtmssn.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2ccqbuonq.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2cixblyap.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2tibyrofd.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2ogjhjocr.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2zlxjdzbe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kvagwspu.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2ydtapopw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2oyoytnck.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2iecvaqhc.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2ifodoujf.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2dkgqcgft.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2hgpvgkjy.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2xfioyuqx.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2sawedjhy.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2ktuckxyl.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2mtsogdof.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2ycrwmuhh.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2zlkrmkol.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2dldakydt.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2mpvqxnxt.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2tpdfneje.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2qwifvpnt.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2yqoblgvl.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2fpjjyyck.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2jcgsffay.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2cqukujqx.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2ddflgrfn.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2nnesxmmo.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2uvhoisnz.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2qhsmvyze.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ozpiclho.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2glukyffr.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2fexcddsl.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2ksvclujp.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2ovjhrudm.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2xzejclwh.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2rnfexcln.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2gthpdytz.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2wpjkgwbj.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2shatdwer.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2ezszaror.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2prqodgko.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2aclfsxex.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2uygbrgvg.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2hdftgwjd.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2mrvvqnor.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2yybebvtq.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2xsjrgqwi.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2wcughxzt.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2hzgqwmyv.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2ijmupokx.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2qomodqjb.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2gepqvooo.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2smlcbklw.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2nncpvkuh.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2ojndamch.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2kzkcpnpa.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2proowrqa.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2uarslzli.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2ytkvhmnw.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2wuyjdvmc.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2pyxqtesu.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2meftfztq.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2cevcwmec.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2svwzuggr.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2ftzzzxrn.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2kfnnnnlb.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2hrohfrzm.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2qsdthqlq.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2zwcgixij.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2yitofbxk.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2uodvjdnf.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2rzaiztaw.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2efzagtqg.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2iaxsiunl.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2icmbhkqx.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2vcuscwnu.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2qohoykhx.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2bbefksxj.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2txodfafk.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2srhsqkjg.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2sqdfweod.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2nfgcfypx.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2xtqjzjuu.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2fhcilmrr.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2fnbnxkre.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2ejulkyvb.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2gheynvmh.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2tqrlqmhf.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2qeraedbb.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2nwpbpgld.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2hwvmwueq.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2arcxshar.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2jhykbmux.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2ulkfpkbz.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2uqkogude.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2tgiklomi.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2xlckvbgq.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2jqxkxrll.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2pdizccas.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2kegntwqo.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2vsidkcpx.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2jbsdzamt.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2gdupkbdr.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2spafjpze.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2olonyfnb.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2innkvfzm.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2tlzxmkvk.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2xkazdqag.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2pnuzntpa.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2fxexwjwg.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2qiskpcfo.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2ysbqisgy.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2efsgkcep.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2wlldklda.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2hfqxhxvr.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2mnyuphvo.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2clzxsyvs.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2wzmkgvwc.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2mvugsxur.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2bqulrkqf.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2hjuwszdw.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2dbrnadtu.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2omnepwde.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2yvblmkzc.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2wpujpwck.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2yzryjwla.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2ulveczcd.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2ygxdeopd.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2pstjqqqx.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2imndpnph.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2jnsaacvq.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2bvbnbdil.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2gpffdvth.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2ainzixww.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2agliwxpw.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2cvhpuyuc.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2crhvnuzd.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2fuubgevn.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2dscxejfe.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2lbyggmcl.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2vxfrtewi.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2uwqmcobv.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2guehersn.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2dzqhtxqu.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2ktmfiedm.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2pyiktvwu.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2zzpycday.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2wubggvnc.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2duqqfhhw.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2ntnthptd.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2eemxztbw.html


<!-- 参考信息 -->