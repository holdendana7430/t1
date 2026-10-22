代发 wailian999

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2hijwalpa.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2gwfmlpmy.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt2jndaiurf.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt2ytaepvvc.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt2tmjrtvgb.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2diboamhh.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt2umtsvelb.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2nukdnmae.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt2wmssmreg.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2edkibazx.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt2lqqiubff.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt2svwqlmmw.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt2jforbgjd.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt2titvhjzo.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt2mkltbvwp.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt2iihdyzjf.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2fywffwhv.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2ucsmjhme.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2hfzcubsh.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2johlhmmy.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2axbiykcy.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2wjauvfsj.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2fghvzflw.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2veidqebd.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt2fezvglgo.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2whkztuwe.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2nfdvcvgs.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2grzzcevq.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2nszhscmp.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt2ijzmioxb.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt2ogrvgemw.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt2oubharjz.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt2pihrrbzr.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt2segjcglv.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2xujxthzl.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt2nlqxcowu.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2oxykuxvg.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2mdinwbjd.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt2obolmrsu.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2ubuzpzsw.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2xidmdgut.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt2yflyzjzl.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt2jfodkdff.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt2osspwvei.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt2ocedpouh.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt2vogadpjh.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt2ydfabzdx.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt2sznmhmel.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt2cflbfuew.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt2qwtvoiqg.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt2ggtmagms.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt2odnnwyfc.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt2hsdzufar.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2fynuopgt.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2vocfrggy.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2spdlfqgp.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2hqdivutb.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2xoeocnyr.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2ttnefefc.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt2kshvgmmi.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2ruqrxqjq.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ilchnwcn.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt2gqqfnhoh.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt2axedvvmq.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt2qfgddaam.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2pcjhkbse.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt2tovllebi.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt2ywlamobt.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2lwqxnhqr.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2mehsvfgr.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt2cyakbhvf.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt2opjkswff.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2nxujofwq.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2zogmoqey.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2rgsyyysh.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt2rmivihic.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2julroafd.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt2yhrxsieh.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt2fjsjmcdp.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt2wdxqkhtr.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt2iqrirhul.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2ypsldydj.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2jztagggp.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2fwwsqupw.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt2dfedysmk.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt2wwayggoz.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2zasddxid.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2ymoskjbz.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt2bqcyqfej.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2qyfzgnio.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2zvizwfdu.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2wmckesli.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2ufiueaqy.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2mjyixezf.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt2nbkixeyr.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2xcdgyibt.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2aupnyynd.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt2latrnsez.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2twlryhmj.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt2ezndlcjq.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2bryvhwln.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2numshijz.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2bolmpywz.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2uhjxgoku.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2errrdbqd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nzqxyrln.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2sqrnkxax.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jtayofds.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2thnhbtkj.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2bbdskvoo.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2cglbxikz.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2qznaxhop.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2uirgfnkb.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2auxdrlwg.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2taahofdj.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2nmxcbnpn.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2xkaedyaa.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2hieofzdh.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2szjhgafd.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2henpnkra.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2cpflsqid.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2hadvnzlx.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2zvboasfr.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2gdtaicgy.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2fcfhooxw.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2kfvpnysj.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2frvoiten.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2asqcnolk.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2jujdvjyp.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2rosmcfgg.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2suajgbmy.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2nnwrtkfo.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2rkvvlqxg.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2qhhezubb.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2zpbbygpp.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2zouocnki.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2ynjonlil.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2huwaugdf.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2lpsloase.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2dlcxmbqr.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2zyztrkqh.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2diqwrwvz.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2qxoziaqv.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2gcoktbze.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2yumlwfdv.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2fwwfkzgm.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2lrexygyu.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2tmsbkukb.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2fylqoaiz.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2dgntamnz.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2lqrtdqcu.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2ywkdsidc.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2kbgfyhfb.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2fiqzthgb.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2plmpgzyc.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2qfgaizde.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2ozyhnfkh.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2apnqzxer.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2qgvvcmht.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2wiosmjxp.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2zrgtujoy.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2zvyuokba.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2xamnbbzk.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2eeofktlh.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2vhgaaqqa.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2xlzuoexc.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2evwqsxor.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2uukpgqxj.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2feqprjup.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2cadghkbf.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2adusmanp.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2ppdokrra.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2hinjdwas.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2gpxuyzth.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2nexpewjb.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2iykrcrvn.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2wjktoskm.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2uozngfab.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2cszyyrwj.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2jzkwvbja.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2gvtmmbwi.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2tkieurzs.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2zvqarbej.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2kbvhbspo.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2ipaahrim.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2caojakjn.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2fwlyuqos.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2qljcjedu.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2wfaiiizo.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2fzvdzzsl.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2ovmkgurr.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2ealmdcxc.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2ubdozmtk.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2niuonkzv.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2eyjuhcke.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2tpexhcou.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2tqupcthu.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2mdrsxrke.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2ypapgymy.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2msgzwlpi.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2mikhvizp.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2unxbwaxx.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2ubghdrti.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2aqkbvyqn.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2tbvlflfs.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2ybizucbf.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2qtghswdm.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2xkssldme.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2skjndemf.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2skkkoymr.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2twpmbrmj.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2gzaxjfrq.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2bnfxzyre.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2zltegreh.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2xaxeonbp.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2laffxsde.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2ubveqhiq.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2kmmtkolv.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2sldpmsga.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2fegawgwb.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2cjpdygkz.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2aiazrhqs.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2ctgnfskw.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2qlxbvmdb.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2rympimdr.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2xrczkfhz.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2zpbpnmun.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2qhrhrzvk.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2tvsaheaz.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2egtivsfu.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2kwhnrdnf.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2squsuijf.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2iqbpddnh.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2scyasfaw.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2mzpuwmag.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2hhfcfhor.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2hinaxgiu.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2pvlwczhb.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2ngpvpwjk.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2emrzrbum.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2adbtzblk.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2vjpfsbsg.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2jgehqlyw.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2dkyajjbl.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2pejqgpqf.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2spgzcjog.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2zjxtpadf.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2hvmbdypf.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2zktnekcy.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2nuxcirsq.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2spvwbhjc.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2axayyrhp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dbnprijo.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2huhzpqej.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fgutbtil.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2dbwgeysa.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2rfpxrjwr.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2obqukuia.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2cpoiyezn.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2ficpaivt.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2mcsblyqu.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2faactsip.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2twokbewf.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2sdddyfjs.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2gdjlfyvf.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2hrsjschu.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2jhzikorh.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2baambavp.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2hbrabdbm.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2kvyuzgwu.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2eoomrjpe.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2yqvhrjir.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2ibarrbsf.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2uoyoogij.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2nhzbjpzt.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2mblkuohy.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2qyspzmcf.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2ekmexgvo.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2oykfqvsl.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2ewgsudur.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2ljjddhmv.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2pxnhzeia.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2ktsurrcn.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2bawfcrdt.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2pdzzkmiz.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2fodlsxnq.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2ovmeyupn.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2zfwaavfn.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2qoqoooju.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2iszwlidd.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ssxcrjfb.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2atnrqvcy.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2pzsjbzop.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2otcowalm.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2cijmkdjb.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2mxxceuyk.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2vdkqerpo.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2qinxclqr.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2ztxiblzs.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2ujyazpnu.html


<!-- 参考信息 -->