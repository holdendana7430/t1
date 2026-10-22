代发 wailian999

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2xzdlafii.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2cbxdmdbh.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt2fuufrvns.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt2rnaxmgbs.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt2cqdmhzlb.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2xklqgozg.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt2efgjpnwd.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2omeyzlfx.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt2lkcctqsi.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt2gurifcur.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt2skwnydbp.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2doabeeox.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt2blvrsmla.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2zbzasvgt.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2baomlmei.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt2jieepjad.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2rlomxxga.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2zxqcqngt.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2cvnliobs.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2fpoqnsxc.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2tssvxpef.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2ifnsmcnc.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2jqnzwkid.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2hvuksbmw.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt2uagqpxia.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2mdplmssd.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2zbwhxmzm.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2gccdshyi.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2ubmelont.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt2uxvuinjh.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt2oxxkabvf.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt2nyyxcxzz.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt2gqommatb.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt2bbajitpm.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2fzntixnq.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt2vltjwque.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2rnstmmku.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2ubxetcax.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt2lhoypmun.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2chjsetit.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2qpedmzzx.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt2dssfnxte.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt2ezosmjoi.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt2tuotpdto.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt2hcqvsfyr.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt2pdvfwuoh.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt2vsnidchf.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt2zmepddex.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt2oumlmjzv.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt2hsqumfxb.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt2xcxwniol.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt2jbqxfhib.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt2kdaodnfy.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2strwvxhh.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2nqjdbixg.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2dxgwztzk.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2agtxsrrl.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2mqiigecs.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2ielrsfgm.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt2pwouuikq.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2zlzlofeu.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2axzgbngz.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt2bkvswqqw.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt2xjwecqpy.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt2oleznmtm.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt2cutqndpw.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt2conznwua.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt2etvxoriz.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2umjjylvl.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2bticiljd.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt2wmustyvf.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt2dslrlrzg.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2periszzl.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2jhxmzszr.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2uqajlkxu.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt2ytgcecog.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2ljghntia.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt2xevvipnp.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt2enwtqpvr.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt2xnkzxbrg.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt2cbwjyypz.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2wgvrivjy.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2vyuzcdcj.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2xbvctjwn.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt2pyrpnjfd.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt2urmdecul.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2vsoiloxb.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2brughzwz.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt2byzwxgpr.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt2zvqejcvv.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2oetjmcez.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2gxiuvsef.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2wusaxosd.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2ffnsvvzr.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2ivepczzo.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2eprhowce.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2tsfiakwb.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2hanbdctq.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2cafftxmt.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2xefeltdb.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2fmgxuczy.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2tvyesrvb.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2elfkggze.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2nlknokyx.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2bimsyyem.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fzrithpv.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2brufpghn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zyffhlsd.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2ydokmscr.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2aaoefvll.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2ktbcowiq.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2nrpbualz.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2tozeebsl.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2nmialuim.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2nmngcbge.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2hfjrqaer.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2ywgvsqoj.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2gbuyipkk.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2tcampnoc.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2lfvblosd.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2plzxflmx.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2foduqebz.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2qnisegae.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2xrwhhawu.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2slbbrovl.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2qoijehbt.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2tqpcmiwh.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2cqhrpupx.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2qviknnze.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2spdwuhyn.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2adesbppf.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2dmotuvym.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2xjlpgzdc.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2fscwxiwe.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2nqiydhpc.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2xfzakvyo.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2ehdizzkt.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2qnawgnnr.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2jtifqxjc.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2dcwxwkap.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2rgnayobs.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2xdfrxzsb.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2wdemrqrs.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2npnyxtea.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2kgyuzdut.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2mitoswcc.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2vmxdigkk.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2dwgiylqw.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2tvzgsjsc.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2zmwibnxp.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2okfofqjh.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2qitrdleu.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2biiccvuq.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2zbmmdrxg.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2xpewssuq.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2noetzjjq.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2vydbpydn.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2osduorcd.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2gjcqbyzu.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2szursowl.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2ihdhklhw.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2llpvkjgj.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2nbodfuvl.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2ikdnktye.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2vtcyqibf.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2gofhcyll.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2nealiffs.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2idivjjzq.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2rjmloqac.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2nkfmzqwx.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2cijkwxju.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2upudjshj.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2wywnncxc.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2blmmhfcr.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2quvitlnq.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2suuieqlq.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2lijdjcur.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2plmwzprv.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2cjaggdla.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2nvxvuibi.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2tmbshumh.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2naymvykz.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2rbanfmrc.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2xibnzvrj.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2ozdgfmkv.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2tpdletic.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2lnqxvkqv.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2ocskvnxc.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2calfftah.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2pqbrhoku.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2weirkjof.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2jbvrbzsp.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2dmqpyuhw.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2kngocjkl.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2mllcpiyu.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2qytomack.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2prkrtvif.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2cjwtptuw.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2zjdtzxqf.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2kvtapsgc.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2nkpadbtj.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ctefoskr.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ihpixmjb.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2xjtpjmwg.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2fateujiu.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2dkzwmdjq.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2cbsrfovo.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2qyuhmrhd.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2tnobkhia.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2ypndvflx.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2slizrwdc.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2lrtdotpr.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2tibpkqfu.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2gcpnauqg.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2mhpevylw.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2skubnmri.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2jguehqdt.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2geqjybcr.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2fgxvljle.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2ojqiniis.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2wwovdkdc.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2fcdaebxd.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2fqqyqvvm.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2ghdapzns.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2qxhtgtae.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2wwhbunrw.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2qaxrdoos.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2cgpbvapl.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2siiekgrq.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2dzjrclle.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2irumzvtf.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2jlmwrthy.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2vzoiqazx.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ptkfpbpq.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2gsrppjhf.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2zuwjhmmd.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2wcgbrhee.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2hwiedxnf.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2ohhpruos.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2ggebtikx.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2jlkopqia.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2chpujxxc.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2gtbwxbnk.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2ooxxojgi.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2mfwudnai.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2yqbmljdr.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2yeufnfqb.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2fausmyhw.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2wzwoohym.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2xjtalsap.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2feozifhi.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2gwncgbrr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2imdmenxs.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2hhbtcfjj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jwhenhee.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2khwlxfgo.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2xsurjihz.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2yqgbzsol.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2xdyjuqel.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2onaytfjy.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2qyapzkka.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2fbmzjevq.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2utudovkx.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2veorlmko.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2xiwscess.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2tpamisep.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2hglediyj.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2lpxxpuxp.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2oinjqhtj.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2kbozsbci.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2viislqbh.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2fmkkhgfx.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2ouqvqkvm.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2jvfjwsst.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2ldodkhqf.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2sdqadiuc.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2gkpmizat.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2lazkzlut.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ujcjgcsq.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2wgscobgp.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2fdweqknl.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2cyxtnlxg.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2lajiolzj.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2calorqzq.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2jnqddjfq.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wetqpxcj.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2ijulgnlt.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2ylilvkcf.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2hnwjxmyb.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2tneonqeu.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2tlgybohb.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2ehmyefzy.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2bzncldgv.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2fkavckwd.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2hwwllhlv.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2uupkxega.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2tpumfsxl.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2kvzpmhbb.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2cvcqzlgo.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2bchxxiii.html


<!-- 参考信息 -->