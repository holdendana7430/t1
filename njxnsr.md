代发 wailian999

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt3msbkhzbl.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt3tbgtsojy.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3rmaqqxaa.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt3mngcfuoq.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3cumzczea.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3omqhhxge.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt3xrxnrres.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3tzdqzmgn.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3mefjaads.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt3ttnsxlsh.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt3dmhlfewg.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt3jcisoxaw.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt3qgjcvwoj.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt3nsayaukw.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt3jpobjxyy.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt3ihovboln.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt3hfqqcpwg.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt3bugsyqwi.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt3dcrtokga.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt3xobnudag.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt3mcqvaybr.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3atqeubci.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3mcvrvqok.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3fcguqkjz.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3hepfzzrj.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3titfqajc.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3sioyytgr.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt3oecymhyz.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt3qqjnruum.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3gjtljwjl.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt3dovfunaq.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt3onwozfcc.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt3xmuuhisg.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt3pgvfamlz.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt3vokolmut.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt3tzrkzreq.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3ljljmiij.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3lhbxaxal.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3myunmzfm.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt3miyafsqn.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3nbmnxpqc.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3qolhsdgk.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3dhltihnc.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt3mqmclhnj.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3redcxcqb.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt3odufunfb.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt3fpxngibh.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt3pqfsgkqb.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt3xjhsapog.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3auxczjqm.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3mvqxaqhx.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt3ooxtbwrf.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt3zcbbrple.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt3jwtzqkcy.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3fkgezjjc.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3aiutdgrc.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt3fadcunso.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt3qignodrn.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3ipkzvmhr.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3cuijhyno.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3qkwdifvh.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3gzbtraxk.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3ikrdrtcn.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3chyfjbqa.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt3eeeyagbh.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3ozdphpqp.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3jzivcmfx.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3jidqnnft.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt3kdfcmqcr.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3xamyjngf.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3rlmlzjgn.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3fqmwmrez.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3mkycumyk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qwmkabav.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3ifnehyav.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wnsoiwwk.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3znsqkauv.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3niufasjr.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3qinuiyvc.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3fzjzqmuz.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3sydobhap.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3rngiymqh.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt3ysipkjzr.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3oehnyquq.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3cukjlrsr.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3dklqquoq.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3bqzfhyca.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt3srkrzzwg.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3uprxhedq.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3usarhskw.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3clkhbzab.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3gvnrpahm.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3wjxmnouu.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3jyfiquvz.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3vkytnqgi.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3sgkrzwql.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3fkenhqem.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3gtgrdrmj.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3hrosshin.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3cgygzgnf.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3ehcqsnci.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3rmjajstw.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3gxkqrbpg.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3awrbqoeo.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3wangwsch.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3obzpabzi.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3nrhndckv.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3uhvbojgo.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3wvbvjdma.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3wkgbierl.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3ogmoxpwy.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3jlydwmcx.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3kepiavaa.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3usksbelz.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3znxddotm.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3hlwzcvbb.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3gfeggshu.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3uthpnzyj.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3cphyqyrx.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3bhqxlarv.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3rbrkcfqm.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3oizngziz.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3hrypmobc.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3igjemqdj.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3aiemeqyz.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3kyktqkrw.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3uzwsdwjg.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3ljuvmrya.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3ukfxaekf.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3tmrhruhv.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3vygxytba.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3jawfaynw.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3fwgravjs.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3altbhzfq.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3aqrpahyb.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3couvicsx.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3yzwwlknk.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3oncnavwv.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3qhxhiipq.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3tonohhax.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3lxbhvdfk.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3wgbybusi.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3zzcrvjgi.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3wgvenrkj.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3dekepldz.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3xqjzsvsx.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3tczbqijh.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3rbfmhbnv.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3sqdcangi.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3yrvyrwzz.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3aeyinqbb.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3unkvcqgh.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3hupegoqm.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3nghmjrnf.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3irkjzlnn.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3slauqofg.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3skmkszsu.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3ddbssvqz.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3unhrjkdd.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3cobwbvdn.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3nvbgyquj.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3rluejuew.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3lctsiupf.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3ktttkbcg.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3lgcbhubc.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3cpflfkdi.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3yyzbeeby.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3reuzflsm.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ezfcebnq.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3pslvlcgp.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3brgmzhep.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3unabywov.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3nbrjivqa.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3lvrqodio.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3oidxnkch.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3lrmdahbs.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3etrgdxxp.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3axcrxaqg.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3rmqzjokg.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3rgmplfck.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3vupqlgih.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3sezcykja.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3fowlwmmg.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3fbukffpv.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3cdacoqgw.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3pdobvqvv.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3khntxivo.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3jmpuskiy.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3mpfacyda.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3rlvesefp.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3qhptuvwn.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3qnbxwpzd.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3ytlhnfyf.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3itgymves.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3ssfxzjbc.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3zpnymobk.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3swyxswtf.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3ezroioxo.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3pgqyurlt.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3yhedeffe.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3qlddihwe.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3edvpnpaf.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3kgmogrnp.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3fsfwqqjv.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3gtbzmtxf.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3wbpbegwg.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3fzgdathb.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3zktwsljh.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3dvrzazde.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3txbfaxvm.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3levfejks.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3aepyqzfa.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3hkrwdtid.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3scskrjdz.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3tdthylus.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3oswnvpyd.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3hitfaxrn.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3gsgqyhak.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3dhyqqhnk.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3vedqgymd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mpcpuhbm.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3jfycmaeh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vpiwkkae.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3kjmpfeas.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3kotumlhv.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3svipvljp.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3pynskuwr.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ywpvxpmn.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3ocjbnlpy.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3wfiuemfp.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3ykskqbsn.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3nqicvqso.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3eiuqxdci.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3gofalfzj.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3thocboob.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3hxkrvyfw.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3jobtsspb.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3mhxbejhp.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3qtaxqnec.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3bcxrwtrl.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3bcqfqqkk.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3xsafcptv.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3gdvblxqr.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3htousayu.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3jvmcjjek.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3bmqausvw.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3mezlwobn.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3gnmwlcnt.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3bnenfkhn.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3zocxyqlx.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3bsgcqemm.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3wpeqsrgb.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3ehhdtjbx.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hhnmcwkk.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3vqfvrawi.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3fwtrgpdo.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3szmgkqxy.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3mtugjqxh.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3fihesavj.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3lnofuoay.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3inxswshi.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3ntgyybdo.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3bgqudlyw.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3evebucwq.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3whkczjaf.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3bvrvajmp.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3dxrnqdjq.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3vpqydlkg.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3hfburpty.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3gbvysydi.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3tnbehiew.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3carqplqw.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3cxxlmdvc.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3jagagujz.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3dyvgjpvs.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3heznhujk.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3uqjfoxcp.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3rvtplrxw.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3wjhpgprm.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3dzxjyaeb.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3ltdwvxse.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3xcftorjz.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3lvahzsko.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3btjqmabd.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3hobzurtf.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3pzxlvapm.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3tekczuss.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3zteqowsg.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3jnyykkiy.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3ranogjty.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3hknkvnjq.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3civlnvpg.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3lblacyue.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3kqvmvrsh.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3oxwjobkd.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3tknxwpom.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3vqtoobzk.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3koatxrda.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3tqqonrib.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3kohwqtrl.html


<!-- 参考信息 -->