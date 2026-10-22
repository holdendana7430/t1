代发 wailian999

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2prgsxfik.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2aabsvokx.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2tlfevfll.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2khactpig.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2tywdcynz.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2yuvworxv.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2yqfrscxm.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2eyxeyzzj.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt2znymnhgq.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt2wtaufnme.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2aiiwembq.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2lxsnxxjg.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2dnsavrld.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt2dobgwhuc.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2iaqtutfy.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt2gutvzypp.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2emxuvpsj.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt2ldvdwzlj.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2ivrnjrxo.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2zqxqyikz.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2hygreefq.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2potgnvmj.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt2fjefsgxt.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt2mqvudtwe.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2xjxnzydx.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2rxbgrbzr.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt2gzzkeuek.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2wjjnsxrn.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt2ltlavcqp.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2avkzbodq.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lswzmzkn.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qtrdqajz.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt2alixxfoo.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt2hegldwrg.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2sahvfwit.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt2pcdyjamn.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2hycuzcvv.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt2bnrxywip.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2ubnvelwx.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2cogbodto.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2dbetbjrv.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2wvfouahl.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2osalyzfe.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2ugftdkxe.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt2igccyufc.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2jlmttkad.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2xkfbsvoy.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2iuwrkiqc.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2xazybxmg.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt2dojrjdbw.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt2xxuaqyeb.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt2stlumgbv.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt2gwaotjcf.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt2gpvmmxdy.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2diskhqcv.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt2hgmickgy.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2anwtlrak.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2fwtgiyfu.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt2bwsmypxw.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2qoefaddz.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2cbvgocim.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt2qudrburz.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt2ulhvqlis.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt2aplltfgb.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt2gjpmvsyk.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt2wusuapff.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt2zpygolnp.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt2ygqpopjp.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt2spmrrred.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt2wiraqcps.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt2pgicwojz.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt2zzqjubnl.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt2fstgymje.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2raojjhya.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2uhmhsudt.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2ettcvtem.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2udaxvqgk.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2whkllmta.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2vkttzetk.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt2ulftzcna.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt2bkasvsqr.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt2obmeyqml.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt2iluikvbw.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt2atkjkcqf.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt2xfhvedsz.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt2mjvatvnm.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt2yigxaxed.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt2cycvmqdm.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2eyljycti.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2boaetozw.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt2whutobze.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt2vepidisk.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2esitickc.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2mvfczrdm.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2utxmgaaj.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt2oliyzazn.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2mbhiqtka.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt2fexrcjqg.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt2wxgwyuwz.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt2ajlbosgo.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt2nitrnczl.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2vdydaaqv.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2qzqkzlmf.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt2xoqjysga.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt2lctvdbfb.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2dfxoizxm.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2dgisccdj.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2sryveyyg.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt2mguuybgj.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt2dwizxsqb.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2gejztjsb.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2jrenzpbn.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt2wufgbrpd.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2enhxftcl.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2nbujhimp.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2miyctavx.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2igdzwgfk.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2kfucesov.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2zjmjjcuy.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt2lpxnzudz.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2xtynjgzz.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2pdvmehff.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2tkoysqyi.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2otgychfk.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2iueufbpr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ugjzcohl.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2ketayarx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2alzavhpf.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2dnvsjxxc.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2ycrjcorj.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2vaqrjuik.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2jrbpuesm.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2tvflxxjg.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2hqujybtp.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2kdrptwpr.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2fiejazyb.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2zvrdjcaj.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2laavptky.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2wvtaatwf.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2umjgvvrc.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2ncwyddra.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2pmjpqezw.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2luzyxtpu.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2ihqkrcwc.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2bnbttbvj.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2axtwwrvp.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2jxwjqqbj.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2hlxrdnus.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2vwyohams.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2yjpralsb.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2uqedknqk.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2fkpplsrm.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2qmgvusoe.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2utjygpvs.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2doujstqi.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2hnmlknaw.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2vhrdvruk.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2zznbiwue.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2fxnnfosb.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2jqlhebcg.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2mfcndyul.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2jcuxfgas.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2wmvldkib.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2quaflgta.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2hjvldacz.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2quldzgxr.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2lxtjmdmw.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2vkhyhhuu.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2ccrqtbdw.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2olztrsdz.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2omacximp.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2lshrjenr.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2zhvixrue.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2eumjfbks.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2fivelmlj.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ppnmubex.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2tknnwusq.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2blyjlflz.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2xtxmqyrw.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2qlnlrcmk.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2kfugcblq.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2dkkafgtc.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2lnjmrnpt.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2mtetuzrq.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2zzooeyzy.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2bcwzwore.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2izxqkwpe.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2dlgwkrzz.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2febhivqk.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2kkykyzdg.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2jvaryrim.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2dysjtdoy.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2vxpebvps.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2hgcemjsp.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2eztwivpl.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2fpjtbrxn.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2pbaijdak.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2qngtwrkk.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2dhbwkwde.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2kbodmnki.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2vqhpfvbg.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2euzufudr.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2iczyhymc.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2drtxszpr.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2rakzigbj.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2scjukxhb.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2ddjhmpzu.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2dkwqjiny.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2ppfechma.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2yyvoasuk.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2gauwyzds.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2vjypweie.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2ixpydstv.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2flbbmqso.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2kgvawtkd.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2evnuwlei.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2nmxyfrev.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2hwxykzoj.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2lpksmhob.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2powyvknn.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2ouzhjmkt.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2burimcia.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2taqxwlxy.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2kjyyeovd.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2cknnwont.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2zcgtxlfc.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2xxcamjyi.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2cktqoczi.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2hsjaafdp.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2lhrnxygd.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2xgtawaiw.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2diiyxjsi.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2hvygvfrj.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2jmorwjps.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2ookozjsv.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2vgubybpr.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2dfclbaap.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2eptgatpc.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2jbejxslz.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2qewnzfhq.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2nkbhcbeg.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2vnikduvq.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2ylcdhkzw.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2ottorvkk.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2oldrtsgi.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2slvnpmoa.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2ehmnfpug.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2yxjczvwe.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2qkwzxdwy.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2rxbizyrt.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2xwtenepu.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2uvkhflue.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2vkazpvfo.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ipbpbctn.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2cdyfczdq.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2zutusufj.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2bnujemor.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2nfsqsssh.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2mlsikojd.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2aeagtowi.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2nkrmqqer.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2mpnutfyy.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2huwcyxsx.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2imklndhe.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2ixgifqrr.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2bmwzsyhu.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2ypoakgzr.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2bojqkkix.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2petflnjj.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2riryjfdh.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2urduehgp.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2tyvaopaf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lfqmwlwa.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2mnrmtmor.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dudgkedi.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2impdrkit.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2nvjxjisy.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2semvmibp.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2oaalxliz.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2ctyyjiua.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2fualyefi.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2gupdrqpz.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2wdytzppn.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2btjspxmb.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2ahsblzdb.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2nzyyglyg.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2oozzdnpb.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2skkwyxzj.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2saqkmtcc.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2bduuybft.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2slbwyfsy.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2xcuobckg.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2fvirgasb.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2mqqxffej.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2sqssfxsn.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2ywadetwq.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2drtzjnjs.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2htdpkygn.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2wyuogopf.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2ffvugaoh.html


<!-- 参考信息 -->