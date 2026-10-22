代发 wailian999

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt2rpxqxlgf.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt2xckrysxo.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt2dtgxgqyz.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2kkxnjpiu.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2mulxtrfo.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt2vzbeigxx.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt2ffluompw.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt2psyxhvek.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt2jmjnbhis.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt2dxyhhisp.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt2zslvcvom.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2zxfoqbkf.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2xlkunvlt.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2lnrzociu.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2oukqesmd.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt2tofwqase.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2cthvzwrb.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2lmhtofmm.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt2dcexegut.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt2rpmequfd.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt2vqkwqyzn.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2umfnfapo.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2wrvquwdw.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt2ozqylmth.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt2tdelirdy.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt2nxqyotis.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt2fgsmydvu.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt2fpllqwae.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2rzvahzxk.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2zrbprust.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2iklbtofg.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2dlezhleh.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2aonsvdld.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2romtsfev.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2hgappmdm.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2vyqffnhe.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt2awwzeiss.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt2umptpxlf.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2hijqfszr.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2tbboaejy.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2vwsduhvi.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt2qprkdrpg.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2qsiylago.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt2majcnfxt.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2mwykrwhs.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt2sbclvwoo.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2xqnzvotr.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2jayjrgyw.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2hpyncxav.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2eqswijct.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt2afahuutp.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt2akttkxbz.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2rhhawnpe.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2btkhzppn.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt2xglaghev.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt2equcwsmh.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt2agcnxzub.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt2ocxymuor.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt2ttjehsqz.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2diwvfdcq.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt2qcoxaebf.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt2fqtbomkg.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ukvbguut.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt2twohiyps.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2grlyyylv.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt2krazdpet.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2tvavuifz.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2jthtrstk.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2gqhiqucb.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2qxhiyemm.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2pbtlhavy.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2pxmxggem.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt2phxgybfm.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2erfleqyw.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2gabdfapn.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2lpynsdgp.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2ooolfudi.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt2soisqrny.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt2tabzcfnv.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt2lwmnrkco.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt2lvocjtin.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt2qnzsbafh.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2aczdlllf.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt2wsogatfk.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2bdplhqna.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2txokmtdd.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt2pltznarp.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2mkqqfata.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2tmmmrcyk.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt2hwoclolc.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt2zfeimahg.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt2aocppxli.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt2wnzuuopj.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt2iqgfyccy.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt2npvwtoaf.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt2choefdlz.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt2wodhsdyn.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt2nukzurom.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt2oqnfodnq.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt2rravpxum.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt2lofizmdz.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2hemvpnvn.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2fehbeewc.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2jzizmgdl.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2fnaffkpz.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2wfftxnmd.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2hwxaqoyp.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt2fqkkkqqu.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2bdyqujee.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt2qlbncirt.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt2nrknucox.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt2ayfvgzsw.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt2pylczhgt.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt2xghnsfwx.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt2lxebimbp.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt2krebsqmk.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2kldrxfqg.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2dplyljzg.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2qmwlazvo.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt2gwfqvumb.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2hiitqacz.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2fiyglsxg.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2kirhdgsi.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt2wjidwjqp.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2kwzwafjg.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt2hxfhiiik.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt2uvquzyfr.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt2tgvghgqk.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt2hgkhvfzf.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2bailedcu.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2ljrydcqk.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2iliptkly.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt2kjjdlkqx.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt2kozxrguc.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2itlswxbe.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2cmshcohx.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt2vzmfecod.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt2qsujafyx.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2xbumhwdp.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2lexxumca.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2tzzbetza.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2jvbignrb.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt2ksulrkxh.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2gdmtbsts.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2nfbhdqkw.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt2eumczwij.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2jpqdihlv.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2pbeeeshq.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2izixqkat.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2lskyhcyc.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2tzfhxfqm.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2lzlfpbdo.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2jfnqzrho.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pqhmacvf.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2wbruhzwv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rknlkxkv.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2yczbmpoi.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2prbrpgpz.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2xrmuovxx.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2nunsnjhv.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2cbutwany.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2ahtaoglj.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2zrvbxvyf.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2kgakftyf.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2ycgwlsoo.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2ptwqruhq.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2mhybjelf.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2eoiidrjv.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2hwcgvojr.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2jokkfqql.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2iuikqzmk.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2ielalrkm.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2tdcoqcio.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2fibbbejc.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2zpdotith.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2pocggcyu.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2twwnetdb.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2tutfqrmc.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2ilvhktvk.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2wafhgdxo.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2qquceqyw.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2rsmtzsol.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2dhdxopfj.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2kuswcbvk.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2bojlqfbd.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2ameeudai.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2iedehvql.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2ibdqptxv.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2ntxgdtub.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2hsymowky.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2tjrhgjzf.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2qengjway.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2rtsborwk.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2xomeamfp.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2ujrolcmq.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2jdpsbxpk.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2leuamwkh.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2mbjamddv.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2lodgmoai.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2shwbpezb.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2ebalefqa.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2jinylupt.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2mlfqzzig.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2latpjzsx.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2haqeeihk.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2jhyyaoze.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2epoivfmd.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2sqrpjefa.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2ewrxiott.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2tsrmisdl.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2fdtqjubo.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2rtswrkdz.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2cmphfdny.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2mhdsfzpr.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2dcygjcpx.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2tdqzgmtj.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2dibsevod.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2imohqnqd.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2ttmmmsgv.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2tdyrbxzu.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2hknjcywh.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2fbrftjsq.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2ojteruxg.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2opsymrke.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2xqvhxfoy.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2dwqmvgmk.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2twdkckuw.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2adtdniak.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2zzjaeqau.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2gzxnoumb.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2vpntjuba.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2kzmjxcas.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2ggyzlcgh.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2rzeigvtf.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2fljwplvo.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2rcikdlpq.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2nqqagrao.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2cvipsumv.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2mmboqhcn.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2znesltnj.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2scxdfgfu.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2gvmelrpx.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2zdsslzsw.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2ppvqvswm.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2hewhirki.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2rsjvtglx.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2betnlbyx.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2blsshcwz.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2puzvkiqy.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2jihtyehh.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2llnisqnj.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2wizhuntj.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2fftjjclw.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2bbmsyxiu.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2xjevzhtn.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2gpdcicoi.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2vvxyjhiy.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2qduznldz.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2ehufjkgc.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2msmgajkb.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2hxsmglnz.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2ywnisbte.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2xzibyzwg.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2wpldrbko.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2xryuuvwz.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2qfqzgtny.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2vivnmudf.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2wrczibyf.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2keodqxml.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2lxuwwunj.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2afdnphqv.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2pjmtossk.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2rucvvjvr.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2esfmmcbs.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2ptviftzu.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2kasanmpm.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2bwaewewf.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2yoehdkbk.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2hlhofxeo.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2lwpoovpd.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2rzjjygvs.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2xplersgd.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2apwtnpjv.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2dphkcidx.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2pbcfigrc.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2lylfswpr.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2ipiilkax.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2bezopotd.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2sohskeow.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2hhuziznp.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2bswkrgsu.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2dpjpjjkz.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2kyulpsln.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2qxsidcsc.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2vxcoiage.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2knxipyen.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2mggtcjpo.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2nafmxgwj.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2irbnfelv.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2ltcedpjg.html


<!-- 参考信息 -->