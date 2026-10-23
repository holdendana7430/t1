代发 wailian999

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt3zicrehsb.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt3ejukvchr.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fyeaelhc.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt3mweatdlu.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3xtiasvws.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3ookrpguj.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3hfqysirh.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3owggyvho.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3sywiwzms.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3ucikzuue.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3bzezliat.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3pwvjdswm.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt3ecfhpctx.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3eqmryjua.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3qdkzdhqf.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3efgsmvwx.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3qrwgtdwk.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt3devrugdj.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt3orhmimyk.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt3lilpviip.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt3cacuoopq.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt3jhmfqpyy.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3nldsqqio.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt3jqxwrpxa.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3suzrhauz.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3uybwjghn.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt3flwecttl.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3dsosycqu.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3nmxuzyvo.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt3arsitfrc.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt3dneaooyj.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt3xwqjyplq.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt3gydnqfar.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt3ibfrlyst.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt3ucdhhpuq.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt3skhcpahf.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt3znokootq.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt3lrvbjjos.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt3ifcapdww.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt3ozvonaye.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt3izpppaks.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3aozncchw.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3zssepusu.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3tfdwgbxm.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3msapnhui.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3iuvbzxpt.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3vauuzanw.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt3throsxbx.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3ixefoijb.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3fagttbkn.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt3ipmlstfb.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt3jdwtrnow.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt3qpcrmxne.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3lbscgkga.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3wfvvoihe.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt3doyashnw.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt3apzvlutt.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3xcuilrbe.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt3hcqoefeg.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt3aygvnbgz.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3mdjbtzwc.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3drqsmkod.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3vvgswdny.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt3cxphwzom.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3ffzhglif.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt3aiarxpgi.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt3ybpwiceh.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt3gvnxudxr.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt3cxsbbtdi.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3vwjwfcru.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3utglcerr.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt3umxjilwm.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt3rbmjbkfd.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt3lnjcjkmt.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3ctryehex.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3tmadbqol.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt3atvhpaac.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3letkclol.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3rghnytwv.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3bathndwd.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3pitiilhm.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3qwcnmtbi.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt3jykxkljs.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3fbjkbhum.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt3ocqrtvws.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt3maouhqhg.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3ylggxmwl.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt3mdfefyhl.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt3hugpuhom.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3ijrjbnfr.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3qfnihtjo.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3cluiukra.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3ntdzyzlw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3durasxtc.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3sjhceeeo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gwrmyvxn.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3kubohdai.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3jxezovzw.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3vtrsfqtu.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3asczsnny.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3yiapmjij.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3qkrwxbqb.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3adsetaji.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3pjuagnql.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3whgolrpg.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3xhzxpgjq.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3bflupjbn.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt3vzgbqctx.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3hrrduuak.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3goomatij.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3xlabtkrs.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3imnaxmyg.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3knktovib.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3qbrjiwsj.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3wgqdgoay.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3zyxyledt.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ymzjnisp.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3tjamslfe.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ujfqyasq.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3vkqeexyn.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3uzpbuqgp.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3qywyjaqv.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3xhfexlmj.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3ghpvwwva.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3ihbatnzv.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3qycqrxdf.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3jdmebzuw.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3sphedklo.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3lzdtqnvk.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3dhjrvhcg.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3yuxaemez.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3ibkglpai.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3qenkboal.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3jzpbdngk.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3erorbild.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3qfrkdtrh.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3poxoauou.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3twiikiau.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3xqlfnzbo.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3hkqqwlnm.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3snoexeaw.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3kfqafdsq.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3nqvnqipz.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3dobzscjl.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3xeinvzct.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3yfdlebiv.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3yysskfzr.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3wfdbjdlu.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3ayufxqnp.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3gsmrqlke.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3sxotvxzj.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3mbclmnnz.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3igjsutil.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3pzumwkkp.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3ezdfhyid.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3gresukim.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3numcduru.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3pefutfji.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3zwuhlgaj.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3oyyclavs.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3oxhulasg.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3weyrfjeb.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3fawsfepl.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3rdxdpzai.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3dcpubwof.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3nsfjtnxz.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3uwpltkfe.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3hyjgrvay.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3tdbeynds.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3ughctovm.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3pkfpkalq.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3nsdwucom.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3yfshstom.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3lsaifbjn.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3mppglnkl.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3cqtyehcf.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3mtxnmkpe.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3imtokwbo.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3uxmtowuz.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3ynelzxkd.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3scvwiubb.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3kppcivcf.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3rdrqcfrk.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3wpbsnnga.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3ksrfjiol.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3kldpctqx.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3ekehddcz.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3ljgmjrjk.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3zbhoeddc.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ymlpzgef.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3yfpqdwvw.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3ntjsfskf.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3iceqoelz.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3smtnplbk.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3waqbtsxr.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3xsozimft.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3tqqzncix.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3pkqqwbyh.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3dfrurarp.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3wsnyvmxo.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3qslpuxif.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3mywthbuy.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3rqwnvrkz.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3jjfsrqug.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3snawnnku.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3wafjejfs.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3cshozeyv.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3jdholraq.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3sywpsmah.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3rehzklho.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3hbslinhb.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3rfytrkze.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3phzkytwx.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3lbjwqrrh.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3fhfaursr.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3abdvnkaa.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ltxhskni.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3metefxpw.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3juulzmkz.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3tgtzbzto.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3svtqexzl.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3drtoppke.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3yqdepeqs.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3hqsoticx.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3nsefbjdm.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3gnbuojog.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3mggecpcd.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3wrniygpr.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3xfezoudv.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3tlsgnfbb.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3rbadusvz.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3oburmgtt.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3lorbzfjx.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3hpspxnbu.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3rguetrow.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3ooasqlir.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3awccdync.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3bgxpmzdj.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3ziumsplu.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3ejlopzot.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nxxmybnf.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3fibysyas.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vohcuers.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3jchetebj.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3dstxlqgq.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3giqrgjby.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3xpsfwewp.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3xosvfpmz.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3qffafmrr.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3cnzpufqa.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3wvmkxdoc.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3qcjalfdf.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3ngvndauo.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3llzwqdle.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3vzpxzjwo.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3oodevayw.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3ouvrarry.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3fdqrenmc.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3cevftcpr.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3wuzconmt.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3pjjwzjlk.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3rxbdtsaf.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3jdjlipmh.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3wagavpxz.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3xqymrbza.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3dqjyytoc.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3rrfglemq.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3mdowhwrh.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3jyztbotd.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3aqwiyeka.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3gpjoyfel.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3jwejynfc.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3ojrqbjll.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jmfagdtf.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3cldkqduv.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3uibnqajs.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3ukrpcipd.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3kycpoqpb.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3quqnygyo.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3hofshiyq.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3gkimpevn.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3gwaokiax.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3wlleuzzy.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3rrykamre.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3iyfizplf.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3cjqjxjxy.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3rjiuvcuw.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3soewynoz.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3pqvlykwv.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3twhconis.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3mkhmegcf.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3iylmzxfb.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3wmxehbzg.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3izfavdkc.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3ybrcrbli.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3xdqqwqon.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3hhvihikm.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3cbzlhkjr.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3ptvvkfba.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3pgtpduyn.html


<!-- 参考信息 -->