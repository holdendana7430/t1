代发 wailian999

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2aiincrhm.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2dvgdmyzx.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt2vttdookw.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt2rueenlcz.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt2yacjdgbb.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt2mrksdhew.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt2zbezsmwa.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2tickodfw.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2jejtzcin.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2xccpmqqy.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2mhimxfcq.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt2gjudhddt.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2frjzwckc.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2aefkyauo.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt2jwzkxzmp.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt2vvdxdpxm.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt2mvmmclpg.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2lukncudt.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2ungrdckr.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt2pfgkuoik.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt2oepeuvxe.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt2zofohmps.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt2ttingenw.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt2rxfhzlni.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2imgfsgwz.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2nhvbpljv.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2dwjpzwqy.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2ixpfrfak.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2hisjwdfs.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2acrwjobt.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2atnloeji.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2tqivobiv.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt2tdvaoesh.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt2ddwibgte.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2evlmkemx.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2ixxcbbwf.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2utljbkdf.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt2zinrlxlj.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2pznyakty.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt2zvzdogxx.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2qxiznbzw.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt2cksoqehn.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2zxzawbmr.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2gyutugtx.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2txzjytjn.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2fntawvpz.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt2geovgict.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt2mvwitdce.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2hfrgqohe.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2cpupqknw.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt2yhdaxqlt.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2ewquwfev.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt2cvlydwov.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2fjxdptom.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt2owjydrsj.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt2tqtzible.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt2wvcrlvmk.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2ktytlwje.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt2sgohezva.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt2yetyvqtd.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2ckcyylzu.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2pvvbntzy.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2ygqfwasz.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2ktqkgjey.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2cnkcgtjo.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2urrgoewf.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2qkaotdlc.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2idpsizsa.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt2nrwnelsy.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2jsexqrbs.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2eqlgspdl.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2gzabgbae.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2rygctdtm.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt2egwypcim.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt2paxblfqg.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt2lhyozfzb.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt2qhbammml.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt2lzrsbmzk.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2anhvcmkx.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt2ppojgcen.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2jykyhewm.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2czlwilao.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt2etadnowg.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2xakpaljg.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2hahheaoc.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt2ophjudtw.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt2kvuwzezl.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt2ifrmjewh.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt2jlfxfnnm.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt2bhpypbhc.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt2gdpsxwbu.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt2ggycddbp.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt2ppetanzr.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt2itrbzwdo.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt2excptbik.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt2avszmcuc.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt2emucfebg.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2ofhfuwww.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2pazekpfd.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2rstsgxhu.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2hmefxuvs.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2qkfddswp.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2csocflth.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt2obsxuwyk.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt2vqukfutc.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt2lzidinne.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt2lplspkii.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt2uthtqalc.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt2vklwnzqo.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt2ucrdqpbv.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2lysaajuk.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt2ccwsllie.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2lqrducuf.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2pcjxinlf.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt2exsmonfy.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt2owxtayjm.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2dwobruok.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2gfbkgpba.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2qmzzkwpr.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt2oehyjeyg.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2pcapxbvt.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt2pepwihxp.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt2njabksxa.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt2qvqrnopt.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt2ybppaexc.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2utcaszop.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2ayxulwlk.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt2bmhmdflj.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt2dwfshcdl.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt2egyhkutd.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2ncciqmck.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2eogcegvd.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2hoszcwyv.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2rsyubjrj.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2jihaxunp.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2nkpgcmqt.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2hnlhvjab.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2iwbrhkqp.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt2belbgkul.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2ebirnixq.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2ddnqhysf.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2bmckddzb.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2ztgwsrsk.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2aebpduzy.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2oxgppvip.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2aebthfvh.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2nhkpazxb.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2lwrdiwek.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2bfhpetud.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xaltuvji.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2pggddfcz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uhchjmny.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2lmkonwdc.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2phtnztim.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2fdgpjynn.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2lbjklnoa.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2tdqnvxlj.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2hkgqeydi.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2yzxfjgcy.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2oqmmtvir.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2czfdvxoz.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2nakkdhec.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2yhewdwyz.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2yfohyvyr.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2eqzhloqx.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2ijgbfcvw.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2eknscmci.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2engoyidh.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2ojfggksr.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2qvtojffy.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2evstpkqr.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2gcfwjbkp.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2towzoxra.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2smbvrtzs.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2yxdpswno.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2obrflqpb.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2hbqbqmib.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2gidhgqgo.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2neeubphb.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2yxrbikfy.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2rjthlguw.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2grcyexlz.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2nfqzakts.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2igcplcmj.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2tzadsegy.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2ejibwttx.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2urimrxqx.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2yrqjaafz.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2znypbndl.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2zjjzgejd.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2tkucuovj.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2syxifzaa.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2acnixulb.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2gbjacgbi.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2mjaolnym.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2ciensoxj.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2haupnmvm.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2tbpiubyn.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2vmnviiag.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2igwzdevj.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2ipigobsy.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2wdezwqfo.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2icueqfeh.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2spbwgkeo.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2alriwvat.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2utorsdic.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2xhufhynx.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2nisjyvqg.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2ylgpxtld.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2lrubohru.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2yckxyusx.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2gltgungs.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2aurkdses.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2ukoxrsam.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2ufeddrof.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2qmscdoec.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2ibttsueg.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2oetktzkf.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2yuxacjcc.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2kkrrfflp.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2acelevvo.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2huwgmkva.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2rvxkubpt.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2addxlxov.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2noqsikie.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2pybgdjnu.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2thakgnhu.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2qimdsaix.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2rzwnrzvr.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2jabwncaf.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2xwtmnmru.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2vnatcvri.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2xcrqeoqj.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2kkiachvz.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2jwblbkhf.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2tsxdyhth.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2zvpcyaan.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2lpkfiuqr.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2eniwspwe.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2tmsorwvz.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2wftpgsuf.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2trmeplmn.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2lejdxxnk.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2rbkbvrer.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2jdkyvmrf.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2ppqbthuv.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2lustakst.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2izwvujyn.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2boqxzxmd.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2vvvjmaet.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2xyyyktys.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2qjbfpwsh.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2ttuxqgsz.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2edjxnoxx.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2hqfrbtbv.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2tsjqucno.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2iraxbiul.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2wtiteijc.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2kybyqzwr.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2dtrdmfbl.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2virxdrrp.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2dypzubmh.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2lvcpbrky.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2xfjphaov.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2qnviplhd.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2avystidc.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2hjqgseiu.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2irelumtt.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2hnmeozem.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2axfpstuh.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2klkhksni.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2qctfvaem.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2amnhvhez.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2almvujcs.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2bpqpokxn.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2yolhplwj.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2ltvypqwy.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2ihkoyaoa.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2guljsfko.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2ayqmmumi.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2bpnwpsmz.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2hiwuanno.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2nkomzsgt.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2nzouczwo.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2cynbaskh.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2kxavprcz.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2cdzezmvi.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2feecidcq.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2tfcqntro.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2xdnvjojd.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2xiyeuprc.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2mruhochs.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2nmiepipo.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2bbbbzmfa.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2cgqrimce.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2nirbgniz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2okpdljnf.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2bfetmfmu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fsfcqelo.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2riabgcjk.html


<!-- 参考信息 -->