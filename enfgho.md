代发 wailian999

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2obmowrgg.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt2uumcjymq.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2hqdyazkd.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt2stumvswc.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2pgbrlfrz.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt2duzxnlwa.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt2pdchlxhq.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2pekqwcyj.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2jdjhhgxk.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2vucsmhgv.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt2rvrqvmpi.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt2hmyrivvi.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2oiphfydl.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2ziqcwlad.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt2eqcfybfm.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt2vwyypbmf.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt2pxgshccn.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2rhjsiqya.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hqppicei.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt2topsoqpq.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt2icxzjzdn.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2bfuwvntb.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2umztburh.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt2vvhfnake.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2sjexjvsj.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt2foprqwia.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2psrvmuue.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2snomglls.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2kryvbkic.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2bfzbzpbu.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2mbvpjlyk.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2wscpchwk.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt2jbxgzwir.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2uudmmdcc.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2xxwtbmad.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2iemgrjie.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2dfkjmuta.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt2qxhgzdtm.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt2vswbmnrl.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt2jhkbmryb.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt2eikfnhvu.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt2mysnzykz.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2qpldvbfr.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt2dywtkiyo.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2hnagcoqw.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2himzewlb.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt2ymfhjdnr.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2lwwwpfgw.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2yameghgg.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt2yhfeqbku.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt2uojntoks.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt2tqsbzjei.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt2yevptkau.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt2zhvotggm.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt2kkvxghih.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt2vlfqgzrl.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt2zvfhsaol.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt2baxhrvuu.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt2kyibbrms.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt2rgipakvk.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt2dleylyga.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2gqzkmihu.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2sazzqihk.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2cltthrvo.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2zxmrqmhk.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2vmzsxucd.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2djstnjae.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt2duhxafct.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt2xolmhtqh.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2neorwuyi.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt2fzeadhxi.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt2edaqcpyl.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt2nmzrvgqv.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2bcceqotm.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2qmgcyfrt.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt2xbfbbzhg.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2tzidifuc.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2ehiqocbu.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt2dtzszuun.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt2tzwrkwdl.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2voqnscsz.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2etkfmqvi.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2eyiszire.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt2qxschkxg.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2zjilapdt.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt2ticojcnk.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt2hasoogcc.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt2ibbseaqc.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt2vzulrtww.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2nfkfjlfh.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2krnznfwc.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2drpxpvbe.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt2kohcarie.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt2deatwtlw.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2jtqenboc.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2yyjtywhn.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2livcstka.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt2clisyyyg.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2blzfnjdj.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2zmefctgv.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt2ksdpgqsm.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2qxanfurm.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2miaqwjen.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2qedcytzz.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2apejfzlx.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt2oizvelam.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2gosycfov.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2jjlkkyvv.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2gfjdwsuk.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2jnypnvdp.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2jnkgotpc.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2cfhlydbv.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2xaaooovz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ujdzvjtg.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2yddbzqsx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wcqapmcr.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2dtaoijel.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2hnfqfeoc.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2wnqnvivu.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2lndlgbrr.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2izssypbr.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2agnkmezm.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2oxuiwkmf.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2dcujkyvv.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2spdffdnt.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2ebuebbtr.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2dtccwlpe.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2ggfxgydw.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2crnyyzno.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2sitqzyjn.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2vomiorrx.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2vcviiees.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2lhrgissp.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2ydhmurke.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2zjmcvgzy.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2jhhswcrk.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2jqavvzoe.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2jsufctey.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2tqtimpcf.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2giqmeflt.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2kuwqbekt.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2pyrbkyed.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2dttnruqu.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2mewrntqt.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2lduanzzd.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2obhwkokc.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2mgblultu.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2yjynllvk.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2eoelsgvl.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2gcgaqsdc.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2ujcgxkou.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2wvutdjax.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2xzoegyct.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2cggxultv.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2torrpiyr.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2bnvavjpv.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2jbejmkkh.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2fjgpfish.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2yiifajux.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2mqfkcxll.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2rxjamqzd.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2ljfnmlne.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2jbiqpegj.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2qgqudzfk.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2pqoomrsg.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2vyzdlwjf.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2ttlqnslr.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2wcpknior.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2ckadgdvv.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2mbajbsvn.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2yrtbzjmi.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2llkbxasu.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2yqymlnzu.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2rjfhnljj.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2hpmnxbqw.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2fyasaieu.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2ixiimsbz.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2wcckcmzq.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2rzmlynqr.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2bcrijcaz.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2tcuhlctc.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2tzzzrzyg.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2sepaujxm.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2ckoqzjni.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2wejsenyz.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2hiqezzew.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2qfcoampg.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2pgdeiput.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2mtnjxlsz.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2mbpiotaa.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2notvqtwr.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2gskrydpw.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2igjytycd.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2dxrinsij.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2vjrlsyiv.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2ylwtrrqw.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2lidolnwt.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2wzlfmckt.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2dyrpisvs.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2hyqxklky.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2hbljfghc.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2nmxwnpsi.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2mgomcmih.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2gqjcexre.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2rhhkjlwk.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2jtlydydb.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2ckwexbry.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2blchcekl.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2hoxxtnvs.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2kskmjwry.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2fcggczzi.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2wyzjkpsb.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2gmxfapzn.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2bqohefse.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2ufmxajkj.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2qoynkpif.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2aaiqhqzb.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2znevhxmm.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2indwsufz.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2ilspwyfj.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2ohddnskk.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2oqtegwun.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2cqlgrdyk.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2dqzvgtce.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2esxpopno.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2pzpnkjra.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2yvcnhkca.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2nlyrwbxv.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2ocbgzhwx.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2xsbecyow.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2mjibpqax.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2ttzmcvuu.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2saqorvjy.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2mfmvapdm.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2zurotuvc.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2rycxcknk.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2yejwsrsk.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2jocejvax.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2teghdxzb.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2guwwijgm.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2rbyodmpv.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2fsyduiqf.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2ykadnjyh.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2bfyherbe.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2aolmuuli.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2kebwlxeb.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2xydjwgyl.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2ocbzjicc.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2siyzmjqe.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2ybgnkaor.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2mtgehlgl.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2tpercbnn.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2wdgwkhnu.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2setbatpg.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2cbndiuhb.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2rkzrguez.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2tgysxarc.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2yrresjfp.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2hbtzztsy.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2sowbeybt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2imtmanxq.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2mzuflxkl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yxdvfjnf.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2lbsaeaew.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2tbhpqbqb.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2uzdjfwfv.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2qxjwqozg.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2fsrwejfh.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2lzvobqwa.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2ohxpenzk.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2wpwuaujz.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2qqqavlhq.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2afhysmix.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2ifnqxkxu.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2qzbzsosr.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2hfmqiwyf.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2vpuohbrv.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2bdigknsy.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2gjfoaolc.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2dgwfgzlz.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2axphtzce.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2svjfnbaw.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2udluqkhi.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2eialkefc.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2jxkosior.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2lhshgart.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2nipcfiiv.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2bijzkiex.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2yooonpsa.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2llrnbxph.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2sucajyzj.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2bywypamy.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2bvqxrcbg.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xmzccjph.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2yvqsmgka.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2praogbwe.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2ozxxmhcg.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ksaofsfk.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2knbkieys.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2pvsmjaed.html


<!-- 参考信息 -->