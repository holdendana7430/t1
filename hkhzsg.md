代发 wailian999

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3iqbafhbr.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3eerxxyap.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt3vhdloniu.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3ldvyznrn.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt3wnbvrhax.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3edlrnkkj.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt3pebspkue.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt3ouvaliyb.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt3pwkopqav.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3xpvwnhhb.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt3yzizmlww.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt3xuvveunc.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3swlqhaqv.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt3fwdnvvlc.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3irbvvvya.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3uuctivod.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3nqqvvmqz.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3xzcmqiuy.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3uenzvwyu.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3iwzakfxt.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt3fdiqsgrc.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3slieuksv.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3gnsyewlu.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3eqpoxaxb.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3enkvlijw.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt3zgspicfs.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt3vicbloyz.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt3vilwxxlg.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt3jnwjpgtx.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt3hlbjmorw.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3jwkulldg.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt3simoeuwj.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3wstavzee.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3jsyofnsn.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt3avvplrps.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3natkhxnv.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3hkbdxjxf.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt3yioswnov.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt3vrqyyrnc.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt3ucbinmab.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt3uxwranve.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt3gxkymztu.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt3lfmhsfgj.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt3qdolwmnw.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt3yuvbbjfg.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt3oxnljiun.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt3dwruyumy.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt3aauadzkm.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt3cllzebfs.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3kzwbsirp.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3hjmnkgzv.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3rkqddezw.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3nrcstvfx.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3ujkornef.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3obzlmbem.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt3sspaqdch.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt3ieayhjlk.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3gjgktuld.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt3utnufxtz.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt3pezufkmq.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt3smlkrqha.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt3ewlewpxb.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt3mlxisnjz.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt3mrsyvuns.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt3ynfkpaqk.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3jnuydvba.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt3biejqokm.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt3qtdbhwdv.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3ioexvape.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3ovobpafh.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3rmmprchw.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt3xkkvueoz.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3cgegtess.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt3vpmldlff.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt3jturxoxa.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt3vviedbrj.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt3yvquscde.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3tynsjxhu.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3yzwddomb.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt3npaekmdy.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt3jxsotjmn.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt3iekedpqk.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3eumxlkik.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3mqapticy.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt3awoebyae.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3thaqzjvq.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3mvdvekuk.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3hncnngmf.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3livuemyg.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3joaptuew.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt3ziyijwpw.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3efdvvheo.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3urniuisp.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt3isrloxcf.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt3kruerbcp.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3dnsmsidl.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt3bvloioui.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3vntvfixm.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3dprheqtu.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt3pawwcxji.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3nmaoeklg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3caboxomq.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt3qqxgvoej.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fjslnsvh.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3yxleujhi.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3hfjtzime.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3yxnwwrpa.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3flxlllyf.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3yxmgoslk.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3mgveowxz.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt3kzqzunhf.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3xgjywivz.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3ggctxhxd.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3rgmibcbk.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3llpeypri.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt3stfomzms.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3dwlwepxs.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3gjzjxyoa.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3wtpsqirn.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3apjdntil.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3wmyslelq.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3nqmaparx.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3snmsajbs.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3anowirsv.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3pouqjhdy.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3yvvuxikj.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3jnupsapt.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3xwroiacb.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3yucibbbu.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3vqexnqli.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3quqqewtt.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3twnynjmr.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3wfzkcatr.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3nnkgtrie.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3cbkyjytu.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3gwzumaao.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3rluieqxp.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3sniggesz.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3ogbrztga.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3eqezeqil.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3vhibtwxo.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3suspfoxg.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3icxqwivq.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3vkhczbui.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3dnceqdln.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3mzgaftml.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3zcdndvek.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3ftcswegq.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3tieastrq.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3udawqoua.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3rkhxaevn.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3mytknfnn.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3aksmtnws.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3feqdxumk.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3dhnpkxhl.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3iqhdnbpv.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3gbwqgbgs.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3czmewjrh.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3bxuitbrb.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3rufzzwoj.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3dqauquhb.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3demnycir.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3gpvuysxk.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3wrczwvjw.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3fqaquzdw.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3gzeayenh.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3olmtwxoy.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3ndenromo.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3jpnwujhn.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3hadsvxdl.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3lnkmiyqv.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3smbyuhte.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3poheyqqx.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3zuebhqbd.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3yhaeegia.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3jzfdauaa.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3pdpjvfam.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3iipelavh.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3tgvdrinh.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3ztccmgnk.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3cuclhshl.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3afcbruyq.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3egffkarb.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3ayjhjupm.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3twkybwtl.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3wvdmomxs.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3ighapzzu.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3xnoiyfvi.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3wsukvgoz.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3cxkflvnq.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3oxkyatzv.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3vldytidq.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3pfuqjlld.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3sxssjpwz.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3zmvwhffl.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3igyxwsvj.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3iosmhbwj.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3fvkqmilo.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3uiwojwcb.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3cxsqwvzy.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3wvdsvwwp.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3lshbfjig.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3tspkfldt.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3ogbnvcmt.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3mkphcasx.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3brreotmh.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3oukrwgpb.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3btcrsbfv.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3vuzwdoax.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3ysmyrgov.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3pfefeqcf.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3uygpexam.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3ncswhcfd.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3dnatwpdr.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3armmpnlb.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3yghjqkth.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3gssozygu.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3xmklpzja.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3otkvoamn.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3nnadcjef.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3iodqoucd.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3vrypuhjt.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3ydisomiq.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3mxxnvfhn.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3zoyvgdlx.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3wybwbsnr.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3deozzkjm.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3znwltkgy.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3xrkpksck.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3wrtjlhmp.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3qfgixixg.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3irdiimoi.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3fxdkqeke.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3edkscepd.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3zohdysji.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3hvvgdwfk.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3yjqfyrxu.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3xcmnlhrs.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3sofmhfyc.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3rgocsqqq.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3uicrsalz.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3mvrfaggz.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3gvwamghq.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3jopsiylw.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3tzgigthq.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3paqihrjk.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3rgghwtdx.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3sdtqfyvt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3regdzozh.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3zlvxcfdz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kyeaemau.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3csnafcha.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3justdhjr.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3aerhmtxr.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3dnojgvge.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3daorlsul.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3mpiisveg.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3scgzkigq.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3xsskhqul.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ziswkecc.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3mfgpnnjy.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3axtxtoly.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ymfzbasy.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3xwfwojlr.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ucadjett.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3kwqfcaql.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3pghiqtdz.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3wqldkkhp.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3lytemewg.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3oahahohj.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3zylceqga.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3uhhgnypu.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3hewgzmyb.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3bktquftv.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3kjtyrfrd.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3naybuxsj.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3xrinhgcz.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3dxtxfhdj.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3xuemwbpv.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3rfyaektj.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3frpeiipx.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3dxbprsyb.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3gbjcwwwq.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3scoiymof.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3zvucdopw.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3oexiugeh.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3wrvlexps.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3tdemjkqd.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3aggmahmx.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3iuynpjvd.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3drnwlpym.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3hpqcyksc.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3ilsheqml.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3ljgzawkg.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3mzoospta.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3dcvxztzm.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3sdywfjgf.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3kwmgcpwg.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3mdnlifaw.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3jceuhqey.html


<!-- 参考信息 -->