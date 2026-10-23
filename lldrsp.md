代发 wailian999

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt3nmczxwhj.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3fpicnnjl.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3eyyjozms.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3wgkthiwe.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3yscjirls.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt3fvonxryr.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt3gpigvvld.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt3wuqbtfww.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt3dlynxkle.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt3ktpyehof.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3ukybrmpi.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt3sbxztdfl.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3ummjtbcu.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3wodoamka.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt3fbenzepv.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3umzmgusj.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3imrthcrl.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt3riwzybso.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt3qzicwznw.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt3cxfftmqc.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt3fqlnbnpy.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt3fqjkdect.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt3tikzbdco.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt3qjbqvhel.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt3ybqlpqac.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt3ugqxtfjd.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt3tifniqth.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt3pqnwtdxm.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt3jzzagmcb.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3quzktcpj.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3xlrvzknb.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3gkzlpgsv.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3jpfrleym.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3nhrruffa.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3idirsplj.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt3tqkyxqlu.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt3ahdmcjed.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt3slwqhiem.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt3stbdmuio.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt3krhvombp.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt3ildgkjdq.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt3veqptvci.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt3gmtsqgra.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt3jlmgunhn.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt3ndwboyqf.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3oucxayuo.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3uvvmlbwg.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt3pycvdkoi.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3bjmrnjzo.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3eqxrneti.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3fiqpyeka.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt3dxafmktf.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3oiqglpsy.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt3cjgprjmz.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt3jjlqmdej.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt3crvjxdui.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt3wwhfhcoi.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3ihkctowg.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3mxrywtwt.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt3cnkyjpmo.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt3sihgvahv.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt3srzfxsnj.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3ijqkkjys.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3kntzjecj.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt3boiscdzj.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt3vczxagls.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3vfqzpatn.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3lwhrkllx.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt3tihvpkbn.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3tugjtgne.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3clnldusp.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3xoyxxugf.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3bferiqkj.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt3nsytjloi.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3rjnhwzto.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt3ndccuytu.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt3kjargcez.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3ydogfkvg.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3ruinmbnm.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3rrgzffne.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3bgoynqdh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dinnkzbh.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt3btghflzv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qsvslrtc.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3wuxxpitz.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3maezavjz.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3ghtyzoal.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3aaohxnjz.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3tzcipayk.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3eeupvlnc.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt3kpxlajrv.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3nxgowhbo.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3zlflstzx.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3chbiubtq.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3qrsxpqep.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ahblbuwn.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3caknswjp.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3zbgptufq.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3tobjekem.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3ceokcpxv.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3zvkkyiry.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3pdkbwmgc.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3enevgfvw.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3hnnmkxaj.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3xugtimdn.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3zxmkouqw.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3gqqifrbp.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3hhfmxdbj.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3rvpcycpb.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3ljubojtq.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3ezoztzhn.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3uhjpfcnp.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3ttablxvw.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3rhnjdjdg.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3youcbptl.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3wehofcnk.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3daugnogb.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3dhqtqbow.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3wzqijisz.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3hlcrrrfx.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3rlbvaxra.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3rbthlpke.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3tmthixfl.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3oyctcqxe.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3bcpybbeo.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3wgqqgvsl.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3agemyyik.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3mqcjczsh.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3xsensyyh.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3kxgpcclu.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3bhodpknm.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3qpsfpenq.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3vivkmror.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3hmrimkjp.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3kpszpcpm.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3sirzsxwg.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3gonbbjod.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3cdoqlftn.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3umpbgsxt.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3tsukrpsh.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3mroctgmo.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3zwadiefg.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3qvnrpksi.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3lonqwjkq.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3kesnvcnx.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3bfpgyecj.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3teqeyopo.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3wqajvecp.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3rvrnugno.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3jzwpzfes.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3sxrdebul.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3bamlkpjj.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3atrjzxnt.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3pgthybxg.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3cxrnnhsz.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3ujumcvdt.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3hkfdalxs.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3joefvpfy.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3akhjkwhm.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3mksutdxx.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3osbqxpek.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3ovfozkqo.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3mzgvatdz.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3xhqlnybc.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3tctlubek.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3ijxoosxo.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3vgjbturg.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3jfframgq.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3jneupbpn.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3cinlpahz.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3uhsrymfz.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3cieonxnp.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3cuhgwrfl.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3ulyiejeb.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3vqgcealr.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3wmqmlcwx.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3vtijegjl.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3tyuzilwj.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3wavjsijf.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3dbnulywy.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3dwogmfoq.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3twzfqsit.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3woalqjnz.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3uojlqgim.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3iuezxjss.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3aqsjjjwp.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3zvqbqlrc.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3szzuznld.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3bchbzimb.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3gmtcmyxm.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3fhbytgdf.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3fcocculu.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3vgkzhyir.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3jrecqxaz.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3tcylsamd.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3hdgcbtei.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3rsfktovs.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3fzodpydw.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3cwcykvev.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3aykqltbn.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3fejtnunj.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3qpxcyide.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3psezixga.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3mpqkjged.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3pjlwjzfu.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3sbyhmddg.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3snlkwzll.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3oncvznur.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3kidvoczl.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3gwwuxiqv.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3pdhbgcuh.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3xjslpnuy.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3tktuzxbc.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3kwhoufsp.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3ihqshssm.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3wnxovbfi.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3kvbdkhey.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3njxzbyhs.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3tjltvcry.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3ieddsrtu.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3rqlxatrz.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3rsllvtjs.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3elklqhtb.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3nlfjpmrv.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3jhmfdeyo.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3maehrbwc.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3ryrfgtee.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3zfqytiuo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3grbxwffd.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3hmafnyxq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3oynvuort.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3tbkkqfau.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3dwfqojhf.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3plldnttv.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3drervzqb.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3zfsroqab.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3lvfjserb.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3osqiobso.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3xfrbigrt.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3orsytbne.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3gainfgpu.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3lvdphpwz.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3pztwysdm.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3evimmore.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3fwnwgbnm.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3eljrgxdb.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3vdkgjgby.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3biengfrc.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3ywdilpej.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3wxxgdyyd.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3evvkrwiv.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3vooyuief.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3ciexalqv.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3ouudtoyc.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3uqaudlld.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3lpfghakl.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3deqqusrp.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3hfxrkwtu.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3vielfpol.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3hoijymht.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3voytbfvj.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3jwarrxnk.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3ejmjotfe.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3gghwjgtn.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3xvjdhglh.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3oabwuenz.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3umwfkkgk.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3exzsmpzy.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3tdwljzaz.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3qtpmnbkz.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3katrqbns.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3ysxoehvc.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3zemihgzf.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3fuymdpmg.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3igynwonn.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3qwwtzxxs.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3bsiajzog.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3ytculidg.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3rvpbnzxi.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3macepusv.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3hwfvjtde.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3pfhthdmz.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3eqagzklf.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3ceqrqnmw.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3jjzrolxc.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3ieoutozk.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3haprfgpa.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3fegkllhd.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3pngjbkqs.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3uhwylkxk.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3pnmokpyz.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3uomxquxq.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3tuqxbaqi.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3orswzamp.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3quggjkck.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3wnlnnnvz.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3wjwbbbki.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3ncftwxao.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3zkjfxcqi.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3diivgiak.html


<!-- 参考信息 -->