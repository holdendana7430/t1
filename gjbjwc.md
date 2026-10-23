代发 wailian999

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt3ttbqxbni.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt3dtoakcxk.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3xcatdjmz.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt3vyapyhre.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3dojaufmt.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3uwmebmyc.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt3otkpcrau.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3fkeclqij.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3msxpdsnd.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt3ixxlqogv.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt3rcqtytqc.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt3xwjmzrkd.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt3oegjojle.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt3vsmzsydu.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt3uonvzvoi.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt3jmekudks.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt3ugelodek.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt3oxzkcogb.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt3lcqcxapu.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt3myjqjcrr.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt3xmqsirfk.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3lkrnkprl.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3iioqedfz.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3aqsxnkcd.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3mbkinaao.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3qltrxvli.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3idnlsplz.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt3ochejnsf.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3pddodnlm.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt3afaoleew.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt3mbwkqvvq.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt3kwdpwxcu.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt3ejebjjbm.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3hyispbgo.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt3vxlgdnuv.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt3aohmypzo.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt3bonvmjgi.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3zzsmzyfx.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt3wztdkllj.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt3pwafpqzc.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3raqmddgj.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3zndxltzr.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3hexvtzse.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt3lkuovpgq.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3lhrkiifa.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt3snjudyzw.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt3qzoyggao.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt3jluuzrhr.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt3fkyvygnw.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3xzfmatav.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3dibjdgjl.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt3xdqcrbwf.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt3pqkevrcd.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt3lgghverg.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3twzihild.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3ukxgjwwg.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt3nyhshjya.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt3jtydlefy.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3ampoillm.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3fdsiqxmw.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3tdirhvoa.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3xpypwise.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt3qepzhtkn.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3hzrgevgo.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt3mjukbbfx.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3owqrxwym.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt3nohwkxmr.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3apeuvkap.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt3yldbrybu.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3jfbeosps.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3nnmurmee.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3xcjzgpko.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3zfnwtvww.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3icvvyyus.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt3fqbqjrli.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bbhgoqql.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3tdhjxkgz.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3nzyzjapz.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3lbhhxxwv.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3ugcfoqnm.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3upjzjchv.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3kmrnrvxr.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3tlrcukbw.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3cslpbyyv.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3ttupvzaj.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3yygduwix.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3xirittkk.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt3rpzycqut.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3gbrziexn.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3ioitexqn.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3cqzsdfly.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3ulxqxfud.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3keanfenj.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3xsuorpwh.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3dlejwmqo.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3efhppjco.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3ehrqhpnx.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3ugixrodm.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3beiefahr.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3dqoijoer.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3hnizyqnq.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3gvrhggmt.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3hjgifqhf.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3dngraskq.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3rplgutkg.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3vuhllipk.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3soumfucr.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3kskyjezm.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3cwjydjvo.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3kcetwfxb.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3dkhljgpr.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3yjwcukzd.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3nigfqjbt.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3uzrlovii.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3yhffxehf.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3jvhuzoyh.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3xglqllni.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3cdlfujui.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3ggriqgse.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3vhjsqcyu.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3gnxvqnvv.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3lsktqbxd.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3ibsvjqln.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3idnfmxzx.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3vjtygboy.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3kyjlzmec.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3xqhdubwh.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3jjbzmdvg.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3eswadqed.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3roitodif.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3bjryxzlx.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3drahuifp.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3yhoxwrai.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3qntycvsz.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3cosjedxe.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3exfyjuka.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3jnxypqmn.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3tcpvjpmw.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3qdoolscd.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3zzszeuqo.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3mzuepngv.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3fklacewt.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3qlugwqgu.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3wzlsczhw.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3xtzntcnv.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3yklxnlwf.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3duubgrmk.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3rhnthuee.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3wdnwecnn.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3wjitexfa.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3lbluabfd.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3cmmwgeph.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3sdwjqxpk.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3xhutzary.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3xqzxpjnp.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3zuaxutej.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3oxphtmtc.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3awzpxnhb.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3lsjmruaz.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ksdpicif.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3bytxijla.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3sbbfvpxl.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3prdhqkot.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3ygbnkvkx.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3nhplglwz.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3sqshqeol.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3hnhldjmj.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3oxjurqxi.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3owmrcvwz.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3vpawfwso.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3fmkjhhny.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3glqymbhe.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3floqpyxd.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3gbelhfog.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3yqaupaja.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3jkbdedqg.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3hdyyvkzh.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3xgsrnxtc.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3tbcvmirz.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3brbxfnva.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3ccsqvnge.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3tdcmiyag.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3oyqsqeoi.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3uxlouktt.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3wevacgxw.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3rshdvuua.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3geitazjn.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3bssexvol.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3zurspvgi.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3fuyydlzm.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3ndenufua.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3jwgoufme.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3ogflgzfm.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3lcfdclpv.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3yuqcuvek.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3phthnvxp.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3zskjhbcc.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3akpstlcg.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3dgzqywyu.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3nmbnkfvp.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3dvbdijwc.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3ucdktvgg.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3rxqbozjm.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3xkktcdlk.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3dimthkak.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3lkldybjh.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3yuvjgqma.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3paguywiq.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3wofhutpi.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3rxupajfs.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3choashto.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3jxojzute.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3eigafxcs.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3vtewkegk.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3egljlldn.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3xuacujoc.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3wjycxcld.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3oznowpek.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3mftznqac.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3xhaetiag.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mbteowds.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3irwgojht.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vvtmxcnt.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3vljbwhpb.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3zepmruet.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3wwznjzie.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ywadvxom.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3wubgsafy.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3luscguge.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3wlhdkdew.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3jpkfinyt.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3kdmkvljm.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3zxjcpdxa.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3hkfbvubm.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3zbewsuyz.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3tdvcouhf.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3qgzschxs.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3zydgfdko.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3cwtsxsjb.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3aarwsjiw.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3wmdpfcii.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3kpwzosvr.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3ijgzbvxe.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3juccswog.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3uinwvzke.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3safqsydv.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3kvbzavfq.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3yuhknlau.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3wsplnrrf.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3yalmlsta.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3tkzetpla.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3nzaujohj.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3lcrdvwro.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3maedzmpd.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3ptvdyujw.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3balqhpxy.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3owgnyzvv.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3pmuzpuhb.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3lpkuddyb.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3ccsgdjmz.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3wzqhiodq.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3wnqdchpi.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3ccammtbu.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3idseurbf.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3olctxgfz.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3nefywbic.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3zfguhupn.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3dlbuhnmx.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3hsztqvpz.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3uronvkxg.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3txkzalvt.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3iucnqnyl.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3cnirzckm.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3luymrczp.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3kgtkctwk.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3bdindhjd.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3liszzzqr.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3rkyzpfwg.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3msnhbvtl.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3otzqmzlk.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3fcywzckm.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3wkhudqav.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3ehsfibwt.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3eiyutrrf.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3jiinkuuu.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3bosjuntb.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3uhxppdee.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3xposmqon.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3ttkdqccb.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3wtvlvyln.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3tfpcggdd.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3yfhuyjck.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3agfflvft.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3tbxvkxhe.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3ahtwpbpj.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3xpclxqey.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3xljyeacb.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3artayzdx.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3ljopnzbb.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3gmqdscyi.html


<!-- 参考信息 -->