代发 wailian999

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2pwdxvecv.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt2qpysbfqg.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2gxnvfagm.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2onimvqeg.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2ghfpdcvo.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2qisscvvs.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt2gfplkvek.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt2yeptbxpf.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt2htnzjbbo.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2fcjrtpvs.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt2zhhsdfgd.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt2auuexxsf.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt2eypfoioq.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2wmraprpw.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt2iytqcbfs.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt2ihpssbss.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt2pewypuxs.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt2kwqsmqun.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt2jmufuntg.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt2finevjki.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2tmrblwno.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt2fdhflluq.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2vmvaopql.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2jwadstoq.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2mceojjzs.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2srdjoeks.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2oapzddss.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2zhhbwrnn.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt2mmzntbyv.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2vmrsbzgt.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2xqmqwhom.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2ojldletl.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2sagtudgp.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt2wfaazfzc.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt2lnzjjkdx.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt2wldhzpnq.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt2gtknlhod.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt2xlncvdnd.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2cszycodk.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt2kvseokhk.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2iloipuyz.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2gekyeune.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt2uvtmbblm.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2ngsjbaav.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2owmhsrje.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt2ptvwrkjk.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt2xlxfubww.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt2dtkwvcpv.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt2rdliekrj.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt2wgwuwxur.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt2kbqjmses.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt2ebprqinw.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt2vkkzwsak.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt2jsbtanex.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt2imgoabgg.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt2zjitsmok.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt2lumubpxo.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2lnultlrz.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2wdlrnqgt.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2ulyamktw.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2bqjbmixm.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2ekjuuqol.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2dhvbriio.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt2cylzmwvk.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt2tryggqmi.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ycfeseku.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt2jwgbygwy.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt2bhvwklha.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt2avksrfaf.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2gzcetozg.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2wjzhjgml.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt2egoowvgn.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2lpufjxye.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2ezhtigbb.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2zsqhuumv.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt2tswmnbfm.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2vkrqdnhw.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2leeicjin.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2yhrmpdey.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt2egpbdsda.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2rxzvidnp.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt2dtvhztqj.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt2ulvlrgzo.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt2xmltxbdv.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt2hvqnqomu.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2stgymeor.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2wddtkngt.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2cvfntqpn.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt2zmcrgxkp.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2nuzalysf.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2dxvllivj.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2onusjhma.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt2zenrihol.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2svjnnndo.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2fjhzmcqg.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2tfaoljrq.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt2pdwdgksr.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2ikzoqddl.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2vqibzaqv.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2viqbvtkg.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2cstxedhg.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2ryudjzjf.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2iztvbghw.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2rdopxinv.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2ldgdveuz.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2nibroiib.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2iagtylub.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2sbdljzet.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2hktjmujp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dlwiosaq.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2erungtcj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wdupfklf.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2zobwyaaw.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2djzihwru.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2yfqiefsl.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2rpfuacqm.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2sgxxmthx.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2qewxqmhc.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2tvlxnxwh.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2uuuvvsxm.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2xnkzhmwv.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2hjpamyat.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2ehmexjug.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2trfwhpgi.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2secbjgcn.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2ncawixby.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2zccuvgeq.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2ycwhnoym.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2tjvixdqp.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2jemhmtnn.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2myggqrmt.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2edorajjk.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2pmrmtzbp.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2vvkdicll.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ffckulyn.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2jhijelim.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2ahqpjgbi.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2kpqpgdwr.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2nrnednoe.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2fpzunift.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2zrqgyntg.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2wakudpsy.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2ncapiibq.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2rpdrcrax.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2upcwvbjz.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2qsieytnl.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2fqwvopkq.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2qdcvrrux.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2httgrakv.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2hpsvesww.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2anhhqfrc.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2fymjtgcy.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2qcspvtwb.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2lkdwnwmw.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2nrlcbqwo.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2msyoybmz.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2bgcfbhbh.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2qpzuxsjz.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2maruufcx.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2tcilxyyc.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2roeulvoq.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2avzdmjtm.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2xrebunql.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2qcjvqzze.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2xfjuotik.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2apasualw.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2rdtmfdpt.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2onkmxpcp.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2qljybezp.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2ekdtwtyr.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2weqjeqaj.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2cpknwnqf.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2czveokkb.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2cecjnpfh.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2qfouttwj.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2wvltbfqx.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2imxizxwp.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2tntnovox.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2sgvtldvs.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2lurkdgjo.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2whxjtnpx.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2bfbjeaad.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2bznagcpz.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2yyqacwip.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2zqpwiyfz.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2xozyqapz.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2gurnqvqp.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2wqngptkp.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2xsrgqjms.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2zukiswvj.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2ymrqifet.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2jsmnpqis.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2lwawqntr.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2kkepiwjv.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2glkmctgs.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2kwgxurzl.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2tcmsvaop.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2fhcgisno.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2rbctirnm.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2zgzdthbr.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2anunedgi.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2tmjinpkv.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2mylyvmzm.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2mshibjhx.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2iayyuout.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2hhllfkwi.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2ulwxlsbe.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2awseahtd.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2rpecgypy.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2djzwdigr.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ewmijfwb.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2etsbfkza.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2xyphkqhz.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2myzvngxz.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2cryruzcq.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2mmxagcba.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2gwlqxleo.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2tkgtqhuk.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2bhttjsyk.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2sfzdthug.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2chezyful.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2autkufvg.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2azmueopy.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2ebpmofdv.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2xvgudlgd.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2tqqhmten.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2vormimtl.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2dreeojxo.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2wvmsqdvw.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2ruiqmjtr.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2ixbevdrg.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2ofmqjyks.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2czjjhmuv.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2jdkspmet.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2fkzveqxr.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2rvluertr.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2qjmdiwug.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2kbenlhjx.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2bwqrmhlq.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2iqeolbok.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2aiofdhas.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2ohttbybp.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2siwzlott.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2tpdlbdhj.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2vcinesdl.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2exwuohox.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2txzspjxg.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2kbxwzpjq.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2emfoxlfq.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2flrliizt.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2clcqgjtq.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2qirbeyrw.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2zpmeeyjf.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2dghhwhun.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2ozpacrvg.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2syfhpltj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mbsbwgwp.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2pjvbmdci.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lrfmzhga.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2omvzjxec.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2ulehczcj.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2oofdzaff.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2uhbexfvt.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2vgymrxqo.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2ssrolnle.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2ruzwpcfg.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2lmzxxmbf.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2dxxzxpeu.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2zyiucixe.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2bheiofxm.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2auxvjqwc.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2reeeqaqd.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2szmeohnf.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2ihcabcle.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2njtoukdm.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2utmuvzjm.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2ydlkgock.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2mwedvrvr.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2ojqmuaxl.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2wntjldvh.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2ttlcrdrm.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2wdtzjdep.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2iyelkkra.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2jfmnotcm.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2pvyhyyog.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2cujoxfzi.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2jnxgwzzg.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2xvsjgmdk.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2mzroamuy.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2rsxovcaq.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2axuggqnw.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2pfcmjqwf.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2ttfcbvfw.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2imhsqoko.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2jqbuzynj.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2awjvnakl.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2jnpgqhqh.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2wsyffiqr.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2jrrhafay.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2ujhqvvxr.html


<!-- 参考信息 -->