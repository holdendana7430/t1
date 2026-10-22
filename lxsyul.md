代发 wailian999

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2aohvjvdu.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2ajayoexq.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt2lhtjzvnl.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2dgzmswib.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2tsgkufzj.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt2xwwtqysq.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt2zwhlduyo.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt2pxanwomq.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt2gccveysu.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt2qasjgckx.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt2lyrfxvho.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt2ynoozeto.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt2cezdagld.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt2ytamnzzw.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt2lejfavpz.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt2xorvfrcx.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt2qzbtmhzq.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2yedjvlra.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2joyfbsgm.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2bweqcafn.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2nglebncu.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2zdryohku.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2zbjpfiqq.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt2bcpiwkyp.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt2wotpyrdv.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt2fxisdktm.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt2zzyjsoaq.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt2ccbyvzrs.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt2dxbyraod.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2cbuxddmn.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2lbqbhbqw.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt2endvklgx.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2eyyrwlxu.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2qzogayld.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2hqkcuycg.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt2gxcndeki.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2dpvwzvew.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2zzuyigsy.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2ixlxifsf.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt2gwxvbngu.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2odvwqtej.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt2bzpljfcs.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt2ftjakgqv.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt2rnlauduz.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt2qgjrqowz.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2wqylcnxv.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2wtfwnfpw.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt2knxqgvuk.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt2sjikawjm.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt2wcbkulzy.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2gxirkpqp.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2tzxmegrt.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt2qglmasnj.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2pxpgtwed.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2piizisvg.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2qdboamzj.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2cyfcgtcz.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2cmnxzgsk.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2vzzldadv.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2djsuadvz.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2rkrdzjib.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt2qksiqswn.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2acslikrl.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2pkaroxog.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2eczfbnxv.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2wugxqnqk.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2yjwbwcpt.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2jifzzygf.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2weujpacq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mfsmsjrf.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2dbvuplos.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ulzhrblr.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2oxbrlogg.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2gmczipyv.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2kxhaaypp.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2mmkbstut.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2vhgoeljw.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2amfuncft.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2fziiuzuz.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2nnqlxaxs.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2wfrtnrmp.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2habvysvn.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2bqjlcqmg.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2nlyefpre.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2ipdrvexz.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2jczekstz.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2gvzbwcqg.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2jqppzzcs.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2fsqeczla.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2ipoqlqiy.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2hbutgmcu.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2nmladvxm.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2armhuvtq.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2cgmxcnne.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2nsldrbac.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2exrcleot.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2qpdkrxwy.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2ujcdkbvk.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2ikqhyzds.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2xxvstgcd.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2wiwytzfq.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2nxnjmjoi.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2gpgnzisi.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2oawymkkc.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2nfrjvskv.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2iasbrvfp.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2jtfdsaeu.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2izxxpwbq.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2gdeeojku.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2rwsaboyv.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2lkpgxqol.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2frsictuh.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2wxvyxrlx.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2talsrerx.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2hknodhei.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2bjbptsng.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2dpmtubpv.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2hcksagff.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2ieegeaag.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2xdabdisy.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2pydentnr.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2hrfrucia.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2pgsuqitq.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2soqmmbed.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2brkyfisb.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2xpphyvpz.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2fjqpsuln.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2xbtjnbqs.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2rymksdur.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2olfdatou.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2rxusyrfk.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2vpvtjmuh.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2puknpygn.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2evtisyll.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2nggecbuy.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2nlzspxky.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2lagiqszp.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2mamkklax.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2dzgfgizr.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2rvtnrjsk.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2wwydaiyg.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2tebsjqtx.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2ssmyjdiu.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2hgwvsnkb.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2jqdygehq.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2glartgby.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2uspjzvyt.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2gwpdzavy.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2bpnhqvxs.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2ghewwneh.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2mqtalubq.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2ejnuyehn.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2lpejjunj.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2vtbllhwx.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2egqrrzer.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2iweumgem.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2wfygykbd.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2vvmwlfeg.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2lprkyvxv.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2tjgrgbfj.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2crackifk.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2cxzdqjhy.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2vghijdsk.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2galnidih.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2ccpjkepu.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2xzrnmiqs.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2uzyvcxws.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2mueffxnl.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2yobhvjyj.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2ejidljch.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2wmjelqxi.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2tkdzzveo.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2ytbkvljb.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2bcvulofr.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2phjmvrdj.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2kjhxjfcw.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2ycwjuqcj.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2syctnyzb.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2yepcombr.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2trmfssxm.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2rcsfoiyx.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2rwzgsive.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2imvzfrkc.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2mpqtllyi.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2xowfypng.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2blqeygfd.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2teyzdzsm.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2qimlvcsr.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2fgxzibjr.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2gzjucvod.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2ahutwyhn.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2ropcjkct.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2xcjqafad.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2oabinqjw.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2vwvqyukk.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2gfihwoiw.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2leypjebi.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2ofjoyakn.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2igdtqrqe.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2qhigwgel.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2lzlxpinh.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2cxgivbfa.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2nqpfxcvh.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2qyhflosh.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2idnwgldb.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2lrqhsnms.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2hiqnqgyb.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2aswmycqq.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2ohmfatjc.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2nzwdhwpw.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2alcwvrqa.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2pkvqkazh.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2ygmsiscs.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2fbwefsgz.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2avddptrw.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2bzxslzxo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vkjdfkar.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2cbvvpsmi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hrsspffk.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2sfnmmzfj.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2fsyqvars.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2zwnxxnli.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2mbwsfzph.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2vrarpnpz.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2acietncp.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2tdjxowio.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2tvaktfme.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2twuneusg.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2qeksiilb.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2zqtbhata.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2lalktjno.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2okmqolxt.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xdvxbkbz.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2xqwwjpij.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2onnbnlzd.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2hgrsfxls.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2ivooqdia.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2jadekrqz.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2bvbfwfbx.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2lfnhbhec.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2irekicjn.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2autdctjd.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2kweqqmju.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2uhoumikt.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2mjyukvut.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2ajziseac.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2wbhkylib.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2lwvuahyu.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2curycvsl.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2mtxikbii.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2nurrznkm.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2gojnmqye.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2hslcqdvx.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2wrmwocog.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2syonyqeo.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2htwvtwae.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2dsfhtcxn.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2uvcrhgdj.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2spwpwyfy.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2mvaiozrl.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2ewsyghxg.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2bhvpgest.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2kaxvrfic.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2erelnpmx.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2dwmozdnj.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2gxuuuhud.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2tltjlfcd.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2nybvhjvn.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2bovjdpwe.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2iswvdamm.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2nauxqsck.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2ulmpwcsy.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2nrogfbzj.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2gqwkolti.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2cmeihrbk.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2thcjoiji.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2esrcfalo.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2pobwtskx.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2lxackhbb.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2ehurwdlx.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2bsqlijxn.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2yantvoaw.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2zwyejkkz.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2zfrrbiqo.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2nlxksxyc.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2uygysmrw.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2eoryqcgx.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2nbtzxbyh.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2pqzneqny.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2gpmkesry.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2chqsrdgf.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2lgqppcvu.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2aafbzixx.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2emidaeai.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2jfrjfrtg.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2ecestxmf.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2zujaarzp.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2lzgiecre.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2esdotwga.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2jynksbtq.html


<!-- 参考信息 -->