代发 wailian999

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt3zlapabin.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt3oicrtcjo.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3olwzxkjm.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt3hpkmbihx.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3twplrtbf.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3iceqrtxe.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt3lxrevcmz.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3lgkzxlxw.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3mctkaomp.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt3rlewgqcb.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt3ataidejp.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt3yklwbyrn.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt3ogpepgfq.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt3uysxkdor.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt3oqnwgmiq.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt3zughfalj.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt3yqhhsrgq.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt3qvbrlrxg.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt3gjvckdck.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt3rwsbnuap.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt3ybybahcz.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3nvzwbtqy.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3zqykhrhv.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3ntclxnfz.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3mobrcmgm.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3pdnzsukz.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3tnuhkjjs.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt3hqrchwyv.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt3jjqwvasu.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3jvlcijpv.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt3aflrjanm.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt3esyisezi.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt3hxpetedw.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3tisoychv.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt3xgjxnpfj.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt3steruocp.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt3yhhgtjqz.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3sgcgjbxc.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3ynctmfsk.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt3iiqpksym.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3hlxkgsbb.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3wpjgylga.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3dilozoqh.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt3tmzbilxr.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3argamgpb.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt3cfiqoljj.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt3yklczpzy.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt3nipukysx.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt3eksmmetb.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3frsycuzs.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3puwtricu.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt3xplulhwv.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt3zcpnytrk.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt3xsxrjveu.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3ywyymdoj.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3lbspbind.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt3tyhcpvti.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3pkstaejl.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3qyvjostd.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3ovlncozg.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt3yajqwwby.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3yclknlim.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt3pksjiesr.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3tssbnrvu.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt3plieckfi.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt3hjvmmbdq.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3couladcm.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt3buwzcunp.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt3cocbriuf.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3cpfdbyyd.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3vjrbkhjs.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt3rpltvvwu.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3armvlmby.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vnpcvqbm.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3iprrejxy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lfiykiwh.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3qcjsghet.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3rgqschdj.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3yxxgdwzw.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3inrouzzn.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3niwqcobr.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3zfpzqznz.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3ltpxyheb.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3qzedjnhj.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3orwbgoiv.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3oaidadyy.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3cpozwfcd.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3qjrltcaf.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3vkzzafey.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3jbmhzuwk.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3tefrrgoc.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3glyoktoc.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3puiedflx.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3nbvxrsof.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3txxtngew.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3lsjqgjrz.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3rgfvvcra.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3iwjkbdky.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3qlodwmug.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3fsdevicc.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3tqpfxenh.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3noxeknux.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3mfbikkxx.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3mxamiwep.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3naadhrbz.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3yvzcochi.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3mqqjxtdr.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3rimufuhg.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3oklgumuk.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3yuzjxvhz.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3tjamtudd.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3oitzvagw.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3gcuzyftg.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3grncmyfk.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3cfulcycg.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3yzyexdpj.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3rxtusmri.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3eeigfmjh.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3xgojswod.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3hsjwvnrl.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3evaodqhw.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3bwnkbucq.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3wkdtrrip.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3qsbghffu.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3pxhvbvjh.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3qqmgvskp.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3uswbuytm.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3kvgojols.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3ygpurvjc.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3ycewpmou.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3nzposqeu.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3nzfmlstj.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3jbkqwrxp.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3gwxngfsu.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3ieerpvkw.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3itqggwvv.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3xoyhoyjz.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3aykabioz.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3hjibgtes.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3tyamumde.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3rjlddioi.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3wbjuuoci.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3ggzsvddw.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3oqdlaowx.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3mveblzpg.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3llcrpixx.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3jyogleuq.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3wzfojffc.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3njvejnnk.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3pduvknae.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3jepswfzg.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3huwbuefn.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3lxftsogx.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3swvotevc.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3lcplkpqw.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3zqmnkfjz.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3ladopgnb.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3bwcnocvi.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3qsyilluv.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3tmmzuxwu.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3ddmzlsyx.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3kzjxswae.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3wtydovrz.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3summpxxj.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3vhiinjuk.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3asbzfcuo.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3mevasqyx.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3ffrhmuab.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3jolxtovm.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3kjauwrip.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3iqjbsfvc.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3mlvkgagf.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3mwyjxtas.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3nkllpycr.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3vbfwenux.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3bagsnmvw.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3fmlntmuf.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3bafnqixz.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3dzyqclda.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3vktsguos.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3wdpuzcts.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3khajtllg.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3wlokegwl.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3ealcfhnn.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3flkvcigp.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3ambcpvyn.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3whcypflk.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3twfszeqj.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3ltydxjmm.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3xuctdjjg.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3xnbadhny.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3ioxdqjxl.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3oypbmkkk.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3gjvbvnro.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3ujlovrye.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3jaiiidpg.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3bixbsdxb.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3hpqzcwat.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ikzugxbo.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3pxxtduxo.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3gjynyhwd.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3yslzzmua.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3lfyfsyoo.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3hbauiuvv.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3farwfzyg.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3fzlxnizj.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3xwtzyoyt.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3rkwoxrla.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3pjbvdgqr.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3ycggtzcy.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3fprdwybm.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3wujylptt.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3ljusjwtq.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3fxzbsiqc.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3lxelpwfp.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3eztqayyb.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3vjkvaebc.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3nmasxmrx.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3zjmobqlb.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3zuyvismh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vurbnrut.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3nziavpxk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bdelepyw.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3ykhgjxcs.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3kflgabkk.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3jvfzcxwp.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3cqdpgwni.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3ujdjvqwd.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3edjgndgu.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3miuuwheh.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3rjxopgrw.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3isjrehlu.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3ymehuxcd.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3kebtpbmg.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3oyaybmvm.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3tfjydadp.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3joqlqwdu.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3shccrlow.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3oikgjoin.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3kbhmkzqd.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3eiivpgpb.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3wkiyjyls.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3hmqxopbi.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3ofroizwn.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3qyyvanfs.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3cnhsavfv.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3xfabaczm.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3odzbhdst.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3bpwjneuy.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3pipkwymu.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3urmxfqly.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3uecjwkgd.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3gtiuztkz.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3klvtvxep.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3oiwhqlvo.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3hnskwyqq.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3mdicypir.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3wbmaopsp.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3balzieig.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3wogipzxq.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3tzspjlsl.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3hqafhyvd.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3xtzerxft.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3nplyvyyp.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3pqydjlwe.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3skegqdph.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3urzrtieu.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3kuxgpaqz.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3omnnlgub.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3ljepcocd.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3octgsjyo.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3dllzizes.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3ogdkehfc.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3bmfobnek.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3fjwkhitr.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3odtdeext.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3ngcbthyv.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3xtrtfgqj.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3xqiuxazo.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3iykxvnvs.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3gvsxhxti.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3sbiglykt.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3yrklvzqz.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3kbogzazw.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3cxkscrrn.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3kcksfazq.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3hsquhcdh.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3cdxemkfy.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3rvmovhzt.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3mzrflaml.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3zmhfvtik.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3ztjscfps.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3iwbgdjyc.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3eslokwcc.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3cmuelbip.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3vsiuyixt.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3gffucews.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3qubdivdk.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3bhevqtig.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3pffcvnsx.html


<!-- 参考信息 -->