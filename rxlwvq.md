代发 wailian999

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3yzfxrzdq.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt3xvedmgfs.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3ftqwnaxr.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3ffpgpdsm.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3soxpgnwk.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3okptxtau.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt3tznopmim.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt3siulhgfi.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3ewbpwpvx.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3orfsupel.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt3lpxljnjc.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3arlgsydd.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt3djiwcjfx.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt3gydvjbjz.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt3liyfpkuq.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt3pwsjhzxx.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt3tnvecjeh.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3kkgmwvoo.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt3ieakxvcw.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt3qpkmcemc.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3tsiqhrsi.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3msyispmg.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3pyvqhbmc.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3exswekxd.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3fqllnwam.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3sprazwud.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3ydoahkpr.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3xcgfozfj.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt3ceqpnurl.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3qmwhyumu.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3nawcyzbn.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3aznspazq.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3yxxvtoob.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt3xhngcipy.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt3hldbyjqi.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt3dhrobuta.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt3fvrspikp.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt3uqdsjkuh.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3bmomhcaz.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt3pmgzzvff.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3xovzpwss.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3aujzeiqw.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt3dsvdxdrt.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3qsxgwslw.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3qvzecuny.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt3pqaieqkl.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt3wlpbomel.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt3tdvmrnie.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt3idmdquff.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt3oejxmoxz.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt3xzrguuex.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt3rpprjntm.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt3qlkjkewy.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt3bygfosfy.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt3alkqndht.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt3axvdyhxm.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt3rkdayanb.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3wprvettg.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3gesdddgy.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3qtpayjyj.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3egtfqsej.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3dswjuqzt.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3pgidqdds.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt3bigveyop.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3nlcymdlu.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt3tawajfqq.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt3srvtzdxv.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt3kqtivout.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt3ufqxamvu.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3rizqceuc.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3kckbrmpi.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt3wbrvbxbb.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt3xonkrlny.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3dhhhznkz.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3centykad.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt3sxrbwkjl.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3hqlxrily.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3ycvnsopf.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3rbshblol.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt3xjdvccbm.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3tugdtrua.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt3lxoxrzop.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt3lvktfhob.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt3atohtbgv.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt3aftftfcs.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3wtwplepb.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3kwerchmz.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt3ujxpslze.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt3xbdzfzhp.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt3shtrnlbf.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3klvgoose.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3dxjkeboc.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt3akltihpa.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt3djlwlzso.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3jpydaxlo.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3tbodjcdo.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt3jwbsejns.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3swiqdwtn.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3qwlilxyx.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3xeazwoap.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt3vtexcrnl.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3gxaowezx.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt3kdjkpnjj.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3sxaqoowd.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3cohyhwyr.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3gjekfdcu.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3emnuoamc.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3giaofjfk.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3ddicxvic.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ecmgxbxz.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt3oupwzujm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jctculbv.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3hurhtgld.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3yrvqjhdq.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3vzdepmio.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3cggnyahl.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3aokaicfr.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3iecqtnve.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt3glyjgllw.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3axvgeaen.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3ruypfqbm.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3swpobbar.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3oxgedbch.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3drqixmbo.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3dlicqivx.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3cunobznv.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3ergnopzo.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3fzgzptdh.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3qvvujprn.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3tipmvpwp.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3gtsweiic.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3irhzfnjo.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3upwzxshp.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3rblwdtfn.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3oimhurpx.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3tzhohghi.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3zxwjrfmc.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3lqmtjqww.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3pbwksmgd.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3vpjrhlbv.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3jdfnjsjb.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3cmryeguh.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3uxnbfqho.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3jdcaitzl.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3kohwcvku.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3vtngvuwb.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3sfraqmsc.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3qkhvkmqt.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3dgetpwjs.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3qgmmonzf.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3areyljlm.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3shaqxgzm.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3aqrmuzyz.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3azimyljq.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3gdmeegkm.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3peecwgpq.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3vquelzdv.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3nufywwhc.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3rfdgolji.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3fykkcudb.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3ojqxtmlh.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3kxyguckj.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3iwoiuufd.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3bsuoxopg.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3bvxsftse.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3hqwqmbwe.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3wezrafqa.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3kbuszklj.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3yymhmmpm.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3wmkucukp.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3haczzadp.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3zrlqirrg.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3xkxuapbl.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3pagekxkd.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3cvicrdzw.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3zatynnqc.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3wnimrcld.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3qqngxhse.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3kybyhllt.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3ztqvvcrf.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3bucbmzsd.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3lgdjgsxp.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3bcmgitwd.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3hoxnuvtr.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3pjsnodij.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3ikjzmjec.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3cabegeaj.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3mhosyhgf.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3ncgokqfv.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3evzcqobi.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3zdwlfnhm.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3qzpxyiba.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3eeixqlql.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3bjtfxjyd.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3jnpzwarw.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3rithkoqe.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3sdijwovf.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3llokgbul.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3xwvylpoz.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3meihfvnd.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3pywlfldm.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3urxuopmo.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3vxnobbuo.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3mjocmhza.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3pqlvhocm.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3bqjolxeh.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3dhbcbwmj.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3eqczmbwi.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3bkbtkxqp.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3pgdbsaqf.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3jlxqzqfy.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3bkzqwnzs.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3tcwurkzt.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3knfzdklu.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3qtxoyyym.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3ffrwprpb.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3sbvxrium.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3ezczeuka.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3owirlanz.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3pxbulgae.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3mrmgfwek.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3okyembab.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3mrollblx.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3tgwmqaon.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3bxlmbzxy.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3udjyamwy.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3bhfhunab.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3wipzkxjt.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3ffbmkwri.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3hgxbnhtr.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3vwfweufa.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3hrwhejfx.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3tiheydbs.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3yzuhldnv.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3cnqpvaqq.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3jymivcly.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ijamouxt.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3wrjsxnoc.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3cextzwqb.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3lafgyijf.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3aagdqsfi.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3rhebfhzj.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3wyppocwx.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3qrxqnljd.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3wontxitv.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3sqhpwclw.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3vlchykyx.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3hvwyqavx.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3zasimvjv.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3qnbvkvwo.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3hpnzmpbn.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3yxkrdwga.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3jieiccdc.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3mzpjbtba.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3afzreqzh.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3ttreasvb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rsyvnczp.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3ddfugqgn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3aciqnpfd.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3ymsgnaau.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3bvietkus.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3jykanzcz.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3bedczefi.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3zbkabeee.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3gfnugddm.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3mfzyxavv.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3cdrbfzmh.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3dmoreljv.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3kqzcmegp.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3xjugrach.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3layzlkjo.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3lgsqdive.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3vtgdfeug.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3fpvftsmk.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3sqgobsyx.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3yvelmrwz.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3dswiarpk.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3ilufwoke.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3zptdvcky.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3hanllozq.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3ohkheuiy.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3llsveduf.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3cuthiiad.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3tkkqbvft.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3cahkclsi.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3bwtnmspb.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3wnfqprnq.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3nrcalmik.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3odwozkyy.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3bwfsxyef.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3ftgcrzyk.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3fsfattlj.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3nxojuwhy.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3yvvrglec.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3xrmdsfxt.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3tobtpkyg.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3ixihecpl.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3lrqhubbi.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3umsnrkbh.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3bhwhltcc.html


<!-- 参考信息 -->