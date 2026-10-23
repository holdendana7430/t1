代发 wailian999

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt3wmrgelyq.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt3hzqydcux.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt3utrhgldc.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt3piimjqjs.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt3chlecqfw.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt3urlucrin.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt3xceccsvn.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt3avaoiwwa.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt3omcgrscm.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3iudxhxph.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3hkvigcwd.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3ncsojfum.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3rwbwlgxi.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3hyhxiiwj.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3qvjoieys.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt3xabvjhyt.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3intizqhb.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3hvbsmuig.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt3lwhtmniw.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt3xkgpeprj.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt3ksmtlugt.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt3ylohuagx.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3lhvgfqup.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt3rdqbipfk.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3pfjjfrkk.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3ardtlfhq.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3uqxvqbdj.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt3cnkjlmft.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3mltehptc.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3ynvsntuk.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3kwqykmom.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt3vschxmwx.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3tcxamfob.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt3bnmfkrvu.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt3ejghzvjf.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt3wskcoyqg.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt3qmrvmugb.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3rcnymekf.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3mithkqql.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt3ktdhrdjp.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt3zjyutyrd.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt3jowhebbe.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3utpytlip.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3sscawqoe.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt3zsymnfdp.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3oddcdcli.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3spwkkwzz.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3nqdtmfwv.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt3dzujqzmy.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3lbrbqxmz.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3hibuhpns.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3hjlunfkn.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3mqexzrvu.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt3ohihsqgw.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt3aoetzyrn.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt3tgovmlvr.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3ohqwvbvc.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3ugmphbgu.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt3zcxjdhql.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3dibidtyb.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3gqfpethe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tpkirmvm.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3xuwnrjdy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wukitamz.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3ookguwai.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3lfcsyabl.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3mkbjzawm.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3kujccosh.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3wuyaskim.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3lyajjksx.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3djigcpou.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3cbqhphng.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3zeucpnzf.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3fuaokhqk.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3uqqydumu.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3azovckfr.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3kfogjgqm.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3jziiakil.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3erwudple.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3rhohiggd.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3dbxrjdfg.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3bvvxnjap.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3kqsywvvl.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3stjiebfy.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3dbhpaalq.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3otntiogs.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3xelrdhwt.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3ygmijdpn.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3hsxpwqka.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3wpiykeno.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3jvtzpwpf.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3vrnllwyx.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3kyiyistu.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3wutejmkq.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3ybxjmled.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3vzfuatap.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3otkhwstx.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3tltnkmmh.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3mbsosbum.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3eexojfkt.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3rhmdoaes.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3mpejirhl.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3cevqzwho.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3hnxdqdpi.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3svafgkzp.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3gkcchkuw.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3exxvstlg.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3jaoljvmi.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3aoafovpi.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3qggwqxqw.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3lghaxjhf.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3gkpntpxq.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3xnsrnqiy.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3mwsqkmbh.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3fanprfed.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3hyndtsne.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3zazuqmqz.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3nadmzklt.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3nhwxezrb.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3tcekzcga.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3lwznsgsg.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3zaavomcy.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3uufrmusk.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3adfbisgf.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3dglhsbak.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3bzctlvgm.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3phmibsgz.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3kdrwqfra.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3qknavwgu.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3rfpqjvna.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3vvferqko.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3vdhssxly.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3fqiwbmqu.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3tzqwkjvy.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3xfyhcwff.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3hbcqazkz.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3rfyocplu.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3zkenpuop.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3ytshrmrt.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3juvmygdb.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3jmqwjnlu.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3ysovujmf.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3wrtguepn.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3cvymncpr.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3bkkhjbvo.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3gsgnwiux.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3thmaarze.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3jirfojdj.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3jqhrrrcb.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3eyrxwbzi.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3nhqsyqvq.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3euxommvp.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3jvmhziwm.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3kymopxwx.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3fohrhhso.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3qepffcai.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3bltedrsm.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3kizoohpj.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3addxjowd.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3aucgeryi.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3ytswkuvd.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3vnluocxc.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3wettxeds.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3ovcugkfq.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3llddvbxb.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3kawejplb.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3nfbuxlgf.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3sbpheqxn.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3iwbarpml.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3krktqfnd.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3rjrmmgvn.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3ewfjstpb.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3bpjsaldb.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3mdcywxgt.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3dgwfogcr.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3unlhkejt.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3bkhehwpf.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3hovpykym.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3szzamsnt.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3nrlukfvb.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3rohpdldi.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3kboohdvb.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3vsauaiyu.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3umdsglcl.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3htfyrmgk.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3oqouuqmz.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3uggtkeeb.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3qpypyymo.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3xnooscdc.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3khxquomj.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3yungdtkx.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3cgmsbgfn.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3neqesxsg.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3tgumswsh.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3rseylros.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3afsljltz.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3ysljlkgy.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3yzoxsxah.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3hhwlfeqg.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3lmxsuqnv.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3oxzrpclv.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3hmpknnef.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3atbbissg.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3abwykkjq.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3wfxgqaeo.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3awbrnhzr.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3ksvwctab.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3yzhzdnnt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3atocbdjv.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3lsxloqdy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qxqcyacs.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3rxitovmf.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3fqeadwxh.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3etmhceud.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3qktufoci.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3lzufzdtc.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3yrfpopio.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3khiwucox.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3qtikrxxv.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3ojdwuctr.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3qxvolnuu.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3fxurbxlc.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3fojiblzm.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3canpxjlk.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3ysvfcvwz.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3xtpviktq.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3oqhfygkn.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3gvjhwxaz.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3ahoufllc.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3mssiaknw.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3wqndckqp.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3pickbfek.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3lrqhgwbl.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3djmntofy.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3cuyxbzvg.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3zsvsngcs.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3nwsbbzss.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3fctnjfre.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3wikajwih.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3rozxmjtk.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3feksvpaa.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3gavdlbgl.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3hqgfobcv.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3hsxvdouj.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3xawxmgbi.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3miimohpe.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3eswnubom.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3wpvxaeql.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3ovkiiiyz.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3qspczjjl.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3egwanjyh.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3llwzwzys.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3cfwucmig.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3wlcllmdk.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3iwxnjsth.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3udjiyrhd.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3kawdnpuv.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3wwtcgzog.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3klbmnrkh.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3latpvkjw.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3qnagsosi.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3xezwvzva.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3hcldaopg.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3vvfjdwvh.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3pdnqgavf.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3sdtqlxnf.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3tiohcvst.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3xifejvpy.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3zfbbkbrj.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3vutgjler.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3kfbjjbcv.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3kfeorlvp.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3meodrsmh.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3wxhejmkz.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3xzobokpd.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3ibxcgfne.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3jqftgkws.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3ephepwkf.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3thgnlemr.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3jhbibxfp.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3kxjmqhnb.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3xxocbgop.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3qoiaklec.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3wmjgtzto.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3zarsuwdt.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3bwoiwfcs.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3gmnmuodf.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3fcskxiou.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3idypncog.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3ctbeuqko.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3jvuoukms.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3wixyovej.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3yikcqeue.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3ltghmjql.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3ggietdbf.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3marttqew.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3qmwlqqaj.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3bbzkxrbv.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3ibfjxvhq.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3hsuqauri.html


<!-- 参考信息 -->