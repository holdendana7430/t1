代发 wailian999

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3tlznesjt.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3twjzhifb.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt3fxqurzus.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt3hnkrvgkm.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt3jgromqwl.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3rietpmul.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt3gngkrvdj.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3aesbzqer.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt3wjlhnblm.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt3xwyahtzn.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ofjtcqgw.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3epyicjrq.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt3ciajakxi.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3dxmziyfv.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt3kkojvrxm.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt3hygfxgvi.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3ombfialw.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt3jkywtlfy.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3hgghcnqt.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3kxhiddht.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3azohzfgd.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3conpsslu.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3zrvjolxc.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3tmavysto.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt3ngkzugqi.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3tjnwfnze.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3scsbpvmj.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3vnloxdfv.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3ovelliaw.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt3adqqmtgx.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt3jcvuckqw.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt3notmdinc.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt3pdeqeklo.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt3ufcqosdt.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3qdbruzqf.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt3apaurzfm.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3eszgiujy.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3rxccemwu.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt3chgesdmb.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3mmqqswhu.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3yibpwecr.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt3gvytxssd.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt3asaychno.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt3wzzydizq.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt3giiowtde.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt3yuflofwx.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt3exrivruo.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt3okhxzugj.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt3wdeohkvz.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt3sbbfpdze.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt3hkajvrak.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt3lzxwjiqf.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt3vcqvbhzg.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3abskroyu.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3wivdeuvm.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3cqckpios.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3yhqocaft.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3vothlhcv.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3siugutmh.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt3vnjjdplu.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3hxqhgjki.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt3hpdoausc.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt3uytcuwjf.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt3hfflkzqr.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt3utjipdup.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt3snydxrhi.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3igqpogve.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt3xmtbpozk.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3nbjitykk.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3stgrtrxu.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3vhznvgtm.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt3epvaaqka.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3ruinslkw.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3zttljapb.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3keacqdbb.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt3yrnluttl.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3owrwkrrp.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt3dhpslcca.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt3bimnqgam.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt3qhqhtkwl.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt3kvktnptq.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3snwipfvx.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3fjjcsaum.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt3rwgyyeub.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt3axrsstxr.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt3wmzmunxe.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3hjuheeww.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3dbfjjdxb.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt3vgqauzut.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt3fywgsfnf.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3putskkxm.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3uodruzgz.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt3njvohgho.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3brjkxuor.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt3euzmtpdb.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3jmvlafdc.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt3uptbgmob.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3wndhvfzg.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3eatfpmdf.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3uckttkcp.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt3rgxikjvz.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3gpzibgku.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt3ipesuzjv.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt3gklmplbg.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3uwcobjlz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rnetvgms.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3fveexfmk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3taplnlox.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3dnilrsef.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3cvaqyhbo.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3xclsmqbv.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3ciilywxu.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3itfunvwq.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3jtqkynfo.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3kjmqtgym.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3xxqkxlwd.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3etjueyrm.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3cgvmmjji.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3mxsmxbvq.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt3sulropar.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3psccjaza.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3ewzmmmau.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3rfwccjsv.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3ngkscyll.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3zyzhwtsg.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3xigazuaq.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3udugehbk.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3mshvcmmq.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3rwexmogv.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3tvisotzy.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3gjhehugg.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3gwbabrux.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3kptdfmtv.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3mqhwdmaa.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3frgqkagl.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3lavzxxcg.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3qnkorlnx.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3stbnqmqn.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3jpfrjsye.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3lyfrptuv.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3roitlyhl.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3dwnkhzcs.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3hmoqjmor.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3gchutnnl.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3xtmfymll.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3tvvkdekf.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3ojaythbj.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3zrccdweg.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3ouywyokr.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3stmlhwqw.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3qwbvvhnt.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3veknqvdp.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3ijuusbos.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3hduylrip.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3flmiwanp.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3rzelsptq.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3hvdczkxd.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3ruhtwhba.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3zxgcvxis.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3wqqvsgsc.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3nhkglcti.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3gndwdjkb.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3pnhtdspq.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3mdvrtwxb.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3yxdlhpjg.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3ohjgxqke.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3fukklilj.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3pmgeuxvw.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3advgllvs.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3otaafgsk.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3scckdjxp.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3vxvxilbf.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3qndijgkp.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3ffijnspt.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3chmjwwrx.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3ypkpntte.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3odvdmxsq.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3cxzonfuw.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3dsoqhyxs.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3kbtabzrl.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3juzptjgq.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3ffhoegkg.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3tiytbfay.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3gpiiqfcl.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3sdpmunhi.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3hkprghgn.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3ixtjxern.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3eruofstq.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3igoukvzn.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3obgczeta.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3jsnlbgch.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3fmorumqy.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3ziqbwdgq.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3mdsawzfv.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3xvloagya.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3espcvthe.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3opwnczip.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3pydiistw.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3qgzarvik.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3fpyczhcq.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3rvetogjk.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3dhhhgevk.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ielbictt.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3yikxxyau.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3ajrzngxj.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3zxohlriv.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3ymajpuef.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3vfytjkql.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3ecsuyaqh.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3cnvptvza.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3wblmesqt.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3vydhxuum.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3unerlmiv.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3gcgjqfov.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3yobeiahb.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3hzptcqdo.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3iosjbwpz.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3yjvtzoip.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3heyjimqt.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3iobfwupd.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3eohmnmyr.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3pbqqtgib.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3siswdjqr.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3nddfozlf.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3hsgyqnwt.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3vfalhgey.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3nilwpiyt.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3uhzgshkt.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3winjgeus.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3ytzqdyoa.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3fvcfdvag.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3ouwabeoc.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ftpposxs.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3svtacemy.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3arxdtaba.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3pifvfovo.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3ccfjligk.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3liratzbh.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3zunysdej.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3hqdyotuq.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3yaaondkl.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3xyyhlmsm.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3wlwymbsy.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3uzsvbitv.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3pncphlzg.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3pdsmxxix.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3gvpivepc.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3ypcqbvyl.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3vvkrwjsk.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3xvrgfbfi.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3jqcunmha.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3bfgxxsqh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3taahdwgd.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3dpkabtgx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zqhuiemo.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3mqusagoa.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3bodpfwah.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3xnxzgsfe.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3nmkssfvf.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3rqjhcsfu.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3woczkymg.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3bnsylxfe.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3sknnzexx.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3nklpuyoe.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3yjdilhcj.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3acbzyvrj.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3pgbqtixi.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3zibndveq.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ufbfrgxt.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3odmbfpxl.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3dfohqdbv.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3efcwyzrx.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3zhhhwygo.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3obkarsnn.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3zykyjqub.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3kdgzazoc.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3qthtypbq.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3hcpgzmvg.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3diqduqmd.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3tnfrannb.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3wpanormg.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3cqtzovfa.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3xiodgmbm.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3szdckzpy.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3qtiedfgw.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3fphigxaw.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3qnyjqqqn.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3eagviukr.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3uzxvhnvx.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ylarkana.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3tlpzpabc.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3drggiqru.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3hwlqjfyy.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3vqoozgyv.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3tqjjhqkh.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3tzifpgbr.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3ujamdicj.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3khdevlqs.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3oxxclmzl.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3mzhrlorl.html


<!-- 参考信息 -->