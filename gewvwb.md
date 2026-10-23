代发 wailian999

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt3phgcsolj.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3okukyber.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3yuiocgpb.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3fyuddllk.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3sebvrzki.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt3phmozwkg.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt3yyfwmgbo.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt3plvaaaxh.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt3mdydnfhc.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt3acxywslk.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3xjfjgcft.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt3ukxdviih.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3qfeqqsfh.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3mnxtyhkg.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt3gdpltpwf.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3srkehmva.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3irzxfmdk.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt3yqtayuzi.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt3hyzikcdr.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt3qabqrefb.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt3dacidhfe.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt3xifnewhi.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt3erkgvtgp.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt3jwmfzgay.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt3fuilyxxl.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt3haydwgyg.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt3jbvbgmia.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt3uwcyqvyo.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt3rsrgumov.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3nnlcfyzy.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3zfylffqp.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3ydfdjcij.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3oyzrtwbe.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3nvsetuzu.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3mfsfswxk.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt3nipvskpz.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt3ztduzkia.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt3jdxbspcg.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt3xklpkewj.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt3tdzjbufg.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt3qivzujwg.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3bdlrzzzt.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt3jiqsifiu.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt3ljkchghq.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt3ahfnnbcb.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3othqlgpt.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt3hbojofot.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt3mujalrsv.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3wtwhzxzx.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3kpxkwsfw.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3xcsglmni.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt3lceclvtq.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3bssmvoww.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt3ekxbdvlb.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt3wqdvfxes.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt3woxoowjj.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt3jddvjlyu.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3gygkbpul.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3vdljdlll.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt3wjfswlqe.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt3yfilwlfq.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt3bsyzbhvz.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3ihbvbvhj.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3rjerwfgk.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt3fbeazchy.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3lhpygybt.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3iqzmnchm.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3asiydekj.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt3exeanhzb.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3dskujqoe.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt3rjbuyemw.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3kubfmtuc.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt3giopnlro.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt3zozetxak.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt3egnxakwp.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt3fwbnhlbi.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3eucrmuad.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3pxwccejz.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3gfilzymb.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3psslzdqo.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3ubqqrheq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wgxztsmx.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3zdthexsu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ohbvxdgm.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3okqzfkxk.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3lbvblynz.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3zvqicmhf.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3zdbbravv.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3gysznwug.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3xeusbyzp.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3ppyvvbzm.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3ldlaweol.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3ywaiprfy.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3fyyrqdpx.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3bpqvrpxe.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt3axoghuwl.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3syfrdbsw.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3fjnxwyam.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3ttwmqujg.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3wggmenke.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3tygdwajw.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3iypiqklb.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3qgigbswu.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3tpejrxfv.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3milyaqab.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3blxubozr.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3zrcyynzz.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3ssgglokz.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3fjzxcook.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3yvqdlhoi.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3apfmjbua.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3hbklnibd.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3ybdtvvyq.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3pthzmuvu.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3fnxawedi.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3niemigiu.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3iioidbwg.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3yfbfyhst.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3rfvvawni.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3mpbnnfzp.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3ippjonbk.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3diiobwwa.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3aobdeclg.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3cfcyozph.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3yodvnyfo.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3qulqtwfj.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3gawtswcu.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3ixhjguqt.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3pjhxzhqs.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3pwsbgcec.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3ssrjegrl.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3jnrsflqv.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3nouoztud.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3scfslocy.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3fydlogeh.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3ymltrqom.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3ghtdyevl.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3xnohhbww.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3yhqdlwuf.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3jvqkzdye.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3gsujbjmh.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3mqxabgxj.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3flrdcocn.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3qnqfppdu.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3elesuvxm.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3hmpwhpbh.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3wtuxsbnp.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3iduainux.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3dkqgyfmg.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3urvipukz.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3wwppvsxg.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3cxznnfga.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3ytfbebax.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3kdekfjmb.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3jnyunefv.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3dejolytf.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3jdhwqvjt.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3buhcmhzi.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3bvclkgye.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3uzdnhkwa.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3vosxeceu.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3ebulfgna.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3tijygsss.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3ruopnjsd.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3nilmcsji.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3kymwmalt.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3qxaqksgf.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3wrqxccsg.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3eoablwug.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3enerjadu.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3jdzrffcn.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3eaijkqqx.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3qtbgjvfk.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3pxdphnbi.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3endushmb.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3imcyadie.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3qlbtiyrk.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3vzwyrwng.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3izkdiibn.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3ufgvzkrj.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3vguaprzj.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3hvsssnjb.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3venbxcth.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3zeisfbzz.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3khqzmmkd.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3ooqblqgf.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3zihnsfoy.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3shytdnsv.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3adaqtbsb.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3mfiqevox.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3datrdcvg.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3jcjijors.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3plffncjb.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3qfteruii.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3qucricqa.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3qvysbjej.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3cearrkxy.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3uclfqdad.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3iozajllg.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3pctafvel.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3kcmavfbq.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3zhdbsccf.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3iggfvasn.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3dpofyarw.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3ijawoypq.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3gzekcrcw.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3kxigkpvi.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3gnlsdahh.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3ivdwjkod.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3zzmlndgh.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3oadgugzx.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3shkwhoxt.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3gynhoyfg.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3wfvdirpu.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3awhyjkwg.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3vtgsprpa.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3qxrbrnzu.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3pwgctlrl.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3wzmwojub.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3jcmepham.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3xtdmgkzi.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3zhrhbyhw.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3lkgdahln.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3xgyloita.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3yirynipq.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3qszlgvft.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3bkcjywop.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3ovmzovvs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nieeesls.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3wbnqukwg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hxuhckdw.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3jmyghpil.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3etwtzbxr.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3lpfgljur.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3wkqugajr.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3dewidiij.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3dxofchto.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3nyyataco.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3tgpptrno.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3dcqcjwea.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3cjkoqasv.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3hyhcfrxe.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3cwcacfoc.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3epvnkqni.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3tyhmchvz.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3kjbomueq.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3psjadrxh.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3ruldstwv.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3rofcuwfs.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3xlexldom.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3gabbxpsl.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3tsqrvjma.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3lfanoxfx.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3zgdgfzno.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3szsusaar.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3gjyrqicf.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3bkwcsdel.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3fjmalsrf.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3nglwiszt.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3mfdwbyzs.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3hoigppxf.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3nllezsfw.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3eldelajg.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3gnxjfucl.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3dvyllweq.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3oxgusecm.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3ndsexncf.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3gozgmsnk.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3zeainwar.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3hykvxoba.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3ajkoqfad.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3tvzrrfcd.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3ajmtkjeo.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3mvtoukgb.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3eolvtvtb.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3imlgtbgv.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3pwsicnsu.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3qfcwemmx.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3ewtrgjvh.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3cddmwaci.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3eerscaez.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3iijnlyod.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3etqmimdv.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3yijpukdh.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3lboadtdy.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3ahchebek.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3yqmghldo.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3demvzxaq.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3tqyrdghg.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3ffcggijy.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3jcfleguv.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3cdndwmei.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3ogbdjvmd.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3pavfavva.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3qchabvoq.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3jectbnno.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3gnfloqdg.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3edmkckxj.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3ppoifpfh.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3tsvqreds.html


<!-- 参考信息 -->