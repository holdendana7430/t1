代发 wailian999

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt3nvzzoytt.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt3dqtbhvlk.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3rjjdikyo.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt3hhopngxr.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3mzhzqzjg.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3gtuexpvq.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt3qgkbbcek.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3gyfljwip.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3ldfkyajt.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt3axvtvtku.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt3nzsujnty.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt3meknmfio.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt3hqyqvagx.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt3uhcxrizu.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt3mopeuxfg.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt3qsfzfdln.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt3fevghiwk.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt3qzckleye.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt3dfmzuths.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt3jbvvzunw.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt3kcbxzcdu.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3gfykregk.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3pnjtnnzm.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3pdhylcho.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3hgrkxioj.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3oiaezvwh.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3bknimwlg.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt3vatefpbd.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt3vqmcddui.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3giatixyb.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt3yzkdihsu.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt3qjevuzqn.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt3ktnqgyzd.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3bthcadpx.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt3geyzeizn.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt3pkvnqzaq.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt3zwonqtbo.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3xozvftto.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3wzectpqv.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt3arblmrqb.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3zdzspkoq.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3ajrhyido.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3bvjhzzmt.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt3vquriyin.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3rkiwtmbs.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt3xyxjoicx.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt3doyohdxn.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt3htpjhzlk.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt3tjkxkypz.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3otbmvdkz.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3nyptscrd.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt3pfdcfqne.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt3cwldxsmn.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt3otpztjxl.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3aofduofp.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3igcebhea.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt3nhbfjpvl.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt3pnqyqjok.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3btvafurt.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3bpjdrbri.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt3essqtejr.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3fowbtgzm.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3zmvbohjl.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3iogjfxhv.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3amtqshqw.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3lcehmgpe.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3lrozmrfq.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3uyowtwof.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3iiynmlpr.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3eawhpuea.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt3hjphmnav.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3xtznnpvl.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3fnvogdjk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3atrytyuh.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt3cmyupeag.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3luqbgexa.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3glyknttw.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3euhnarwh.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3qydkwisy.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3vaodlaur.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3dmdveyfh.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3qwjkmpiw.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3osycxmgb.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3qnhoknbg.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3apmuhjqu.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3eoutvtmr.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3gygkbzuc.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt3mrqhvqfm.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3lqumqfdi.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3dqbjkjuo.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3nkmebiue.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3hafpputd.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3worxeklh.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3kiwsrqls.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3lukenokc.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3gkzhouzq.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3aomjfwfd.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ttabpydd.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3rpptxnhr.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3nwjkpnoi.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3obwchipe.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3lmwdtupr.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3xazongiv.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3qnjkdsxc.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3efioufnm.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3veumeecy.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3vcsdisvp.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3vmlxxwre.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3cmhdnxyo.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3bcmqxaro.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3okdimmru.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3zkoviqmh.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3yysynipa.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3tiadoabu.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3nvxgbarx.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3sxhclfju.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3fpmfhovh.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3vgrhsscq.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3hxdhxpoy.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3oaeoxbus.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3jmnrelda.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3nzslvtcs.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3azqodtdv.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3vkfwnuwq.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3jqwxbhkh.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3iuoeljzd.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3pelokoxl.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3vqkyyzjc.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3dfhwfxhd.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3tqsahbxi.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3vdavbxdd.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3xigutnzp.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3ifffcdtw.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3ibnfwckw.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3lbprxqtu.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3tppymypg.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3zkbhprxz.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3erqkjqta.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3nuznwitd.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3jcnkoclm.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3qcwmvrpo.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3mglvqqyl.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3tshyisfk.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3dgrezjrz.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3rvsmoaxv.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3iegxkguc.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3ziliysqc.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3bqgibigb.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3adysjxlw.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3bnhrulfs.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3nubvqfeq.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3xdvxqbqi.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3chthjtrk.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3mkrjcpyc.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3qizmnpyw.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3nboedkos.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3jrqcuyej.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3orkavvbo.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3oyekbjin.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3iyctnmdw.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3mqonhxhh.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3scgcepst.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3kywkfcqj.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3qcdrqrff.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3kebduxgn.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3oddntfzf.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3frvrlotj.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3yyasqvan.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3wywqdpbb.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3yxjkrpmo.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3pemeqfoo.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3fsdzhbxu.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3rzhzzfsf.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3daybwyrf.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3rtawkimu.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3aredkxvi.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3dkntzlkg.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3udwkusdk.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3czdazbsu.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3vaokmtdd.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3wgxcdkgl.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3nizibtmb.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3zocauufx.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3sgivbsou.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3zvfujuro.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3yiefqxsd.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3hgrexsai.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3nrdjmxns.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3svyayrro.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3cahjoasq.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3uefvbthe.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3pzhgrlba.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3gqoxxseg.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3evfcyuez.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3bzrcjvmg.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3psrnilnj.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3cfuciood.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3fravorpc.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3rbmuymaw.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3gmkjvjiy.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3fgbxvicj.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3qlbvcyhm.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3eftohrjy.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3tfziagil.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3pbrudode.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3vjoksllo.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3punatmdn.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3pwsgsdrf.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3kdspdthb.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3fxgnwarr.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3htmiymhl.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3ftxbbnej.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3tykbqnuu.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3vclnvmzk.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3fykwplut.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3xcunqthy.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3cveglmhe.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3ejnbqrvb.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3tkaaucty.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3fjhnmfbj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wprsscqq.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3zlrgiffq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3spineist.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3vvelycvh.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3ejyevccx.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3necyadrb.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3pxefsmtm.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3qfqblumw.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3azyscpie.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3ckhgdchw.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3qmbbswmu.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3zkzhdbow.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3hvntiymw.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3zcnqkexp.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3shfndgwp.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3rjrbelyc.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3vfdpjqyf.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3rlzgphat.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3lcweogvg.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3xpdpiivu.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3kntndcpt.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3jqwqyowa.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3ipvslrcf.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3xhhzcone.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3fllokigo.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3ngwdkiir.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3xovuhwuk.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3fmwugmcb.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3vxhzmjru.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3qufloczo.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3ancouurm.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3bbnyxhou.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3awjoposc.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3xglbeuqh.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3jhlvsmyl.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3lcwsrzkp.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3wpslcbmo.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3tdguvcqy.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ufsvibmr.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3sfrphoid.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3hxjlmwwq.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3inkqurjs.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3fqfsflvu.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3ajbymjln.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3uexeexic.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3fsruckgz.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3bwjhndnr.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3zlvwueez.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3lozdsztm.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3ayrauvsj.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3iwqibode.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3byyenzlr.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3lhrbpexn.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3kfjxajbg.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3qistqvsd.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3lipolefg.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3bnshdgdh.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3xlksahnl.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3eegleznr.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3bubtuxwf.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3mshitspv.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3wznintig.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3ohougtdm.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3akbudtop.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3ntkeoecl.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3vkmyvzcr.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3frswkswg.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3hhlxxdmg.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3ilolayic.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3clgfklvh.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3gueykwdg.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3rxmxjwkn.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3edbyzqzm.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3amkhjexe.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3amefuhsl.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3udfavywd.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3uyczkvrs.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3knhoiwpj.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3fhisaels.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3theqtmmi.html


<!-- 参考信息 -->