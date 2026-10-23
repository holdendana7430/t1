代发 wailian999

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3prwbihcp.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt3utfsdkdt.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt3wkqjodei.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3ndeyzwcg.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3gnohlrtj.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3lvoabfqd.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt3dezzbztj.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt3uzcyoqoq.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt3zndlssqp.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3rlmhadnb.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt3uzlzaaqx.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3cocbfdkk.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt3ghdijnel.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt3ytvkpwjm.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wqdncjbk.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt3bizwwkjx.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt3uagueune.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt3csgbdtxg.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt3ksptklae.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt3yllcpqbn.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3ehexhsrm.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt3nvpppqbz.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3ghbfvalj.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3nprfvysk.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3ohytmaml.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3elwphzaz.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3fkzdlcvk.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3pylmhahn.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt3avsuhnuw.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3rudvgwmn.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3lynholvn.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3dklpgdac.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3bqltvczn.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt3iugmqxij.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt3trbjlpyt.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt3gitobquw.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt3lqazqfpi.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt3miffbiyk.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3tcxleufn.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt3pricnzfd.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3qqjvdieg.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3trobbfvw.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt3outjkbel.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3kczwcqkj.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3gpopeehb.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt3skoftztn.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt3vauqdqqo.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt3hapsxpiy.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt3duwebsxt.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt3vmondibv.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt3ieoypzmx.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt3segosecn.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt3hqsjvcsz.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt3egadeqta.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt3oaqibocu.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt3uwfywnje.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt3mqzzrhkl.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3ryncnjat.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3eownjvid.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3gdspczpx.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3kedkgdwy.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3tzkvfrjn.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3lnrvnadz.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt3lpvxpbwh.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3qqkjvahp.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3hybsuplr.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt3uuqfvrlc.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt3dknolagk.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt3qyddkxwm.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt3mkkgflwk.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt3aefavobw.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt3bvuiwhxx.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3tosxchxc.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3kkucdioe.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3ugvibnzz.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt3ovrcheab.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3eaogucvp.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3lokngzya.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3pthbhzog.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt3lllxuswk.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3tjaqdbhi.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt3aihbkkny.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt3xqtrtzbr.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt3pycyxltl.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt3avtrdvaf.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3liaivbur.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3sybmosbj.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt3khlznhys.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt3aowhnvdc.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt3fjusnfao.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3ofnfqkrv.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3zykhlpre.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt3aumjqavf.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt3wshfvvjn.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3noofqugu.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3nwwgdanm.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt3vtbowojf.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3vvgpalzo.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3srkancjc.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3glzpxgvj.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3oneyzjvh.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3udhbbnkb.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3ogykdgif.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3elgtuazj.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt3cqzwvqqj.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3feyeeohf.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3xmmdhpqz.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt3hsdvuvhd.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3dlihkgvo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uttizhoa.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3oadvjnxw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jgmomvsw.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3nzodgnld.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3loodsxmi.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3fkmntulr.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3xymofwag.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3ebowlyzj.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3yqzmenqo.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3hllvxjto.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3pdwnnpuc.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3foqvzock.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3aidjsevt.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3idnfiooy.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt3nhidpasq.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3szxemrlk.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3croktbad.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3vcakcptp.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3rzdyafqs.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3seyrfaty.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3eizsgzwc.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3wbnjcfyr.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3szakiicg.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3txpeqiit.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3xykekiie.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3jracqozn.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3kqlncnuh.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3tfhzfrxz.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3lokmultl.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3bjlkyhbi.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3fpgmoufa.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3raigsjhz.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3fubngbay.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3ffjcjxzm.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3vxsapbaw.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3uahphocf.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3jtyqqgly.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3cijpdcou.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3vrfuybrp.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3muzfdkic.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3muuupilg.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3qayhyhpv.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3dunctllh.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3fdiwhptn.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3dwqcanzh.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3rcpgiceq.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3axyzunjy.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3smetvemh.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3wiozhwcf.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3ncxtmfto.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3siustkqz.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3fnnsfakl.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3svxkpkzm.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3olwzbtyz.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3juibvvsp.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3qjxfzncz.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3otjwlrly.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3qsvbuzqp.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3unhogwkb.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3wdbxkemq.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3pcxmjcjn.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3jxpnpkhe.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3tntuxdor.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3nodsmrem.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3kualplrm.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3ljfaqadz.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3mtqfuzqs.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3nwrclygg.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3trpbxpql.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3ysybsecr.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3eqtlinkh.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3esmricxs.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3cofxgmsj.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3ynfttmuq.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3ayvvbedg.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3pudzotug.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3skbhvtmu.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3gazoxfaq.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3ifzhqnet.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3quyjvfrj.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3rqyuwnip.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3seuswcub.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3zdvupigd.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3vtkhitsh.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3yjrcvknu.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3hxelauon.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3jhsrhmtw.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3rjuabbsk.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3xoncclms.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3iwzcchdo.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3mpfrrmho.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3ghufyfqs.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3timomzgo.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3hblfjali.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3ievogvbx.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3zgociafj.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3lvoerivl.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3kezvdxhg.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3xkejbrme.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3iclyevbb.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3jaijdgdg.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3tgbwxipr.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3nmsudmjo.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3smbdnccg.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3iecfkhmo.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3jdgaxowa.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3insyqmad.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3koaybgca.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3iwzrisnr.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3smzxpiho.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3eiqwczgw.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3kiyrptmf.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3xekqewqx.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3plofrmyz.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3fxocilaz.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3loliztbk.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3hvizmxjq.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3wamsygqn.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3tahyhgdg.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3cqrqwnar.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3wbmrivbh.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3xilugovn.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3zcyhlyej.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3sraqphbk.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3uozxvese.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3unhdddcz.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3hpayfczi.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3neqcorqi.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3qejsitlg.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3ndbcplkk.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3gvahiizc.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3atpmatxk.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3pvmrtngw.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3xwhnukzo.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3fsvlyxso.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3yzgbpzol.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3jsxqoocn.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3bxsfdigc.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3ypdzcarg.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3rbraaqmt.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3envvpbmj.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3gbdstjuj.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3jnnhtexu.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3vttbmydw.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3rvrguzzv.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3jzomswiu.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3qvspgnhc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qocqxopq.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3nhauwuac.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wziwcpax.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3nrmfsxtp.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3ntqexlxs.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3iyhazjln.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3bfgdvrha.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3oxxbuysx.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3laiytyjy.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3ssooubld.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3zytnrpoy.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3cdpbfohv.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3entrbqov.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3tekefqyh.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3szuwsuki.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3qzgovnpe.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3amddyevr.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3cxgjyaid.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3hwppuzjw.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3tpfhrkwu.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3curypmql.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3izckdlns.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3uakrvrtt.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3zxwezojm.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3kjzwkfyx.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3rlvslcxj.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3isajnkkw.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3zkdfcphp.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3pznitlzi.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3dtogmgff.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3otkdcaye.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3tshthiyo.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3bbfiiocm.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3spvmhjck.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3qpkhmuoo.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3fooebkdh.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3qdgkizan.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3dstxnrfc.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3xrsvkcfb.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3fhesafsj.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3fbyjwdqp.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3qwwogkph.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3votjmitl.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3cpwnqjan.html


<!-- 参考信息 -->