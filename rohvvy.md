代发 wailian999

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2foexrhiv.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt2wxqcpxjh.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt2blrekyny.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt2lvucrmae.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt2mzcpcnfo.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt2fsncnmry.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt2bwpnvlrg.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt2wlotasfy.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt2ivicrilf.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt2nzmwxhpi.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt2gqcermeg.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt2kchistjk.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt2wuxlngpe.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2knzjkoyf.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2unfiwmgc.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2wymusyln.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2dlbuhhna.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2zjqxhktn.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2lmczkimm.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt2ftbnbant.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt2qqwumtjj.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ehkooxsk.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt2dmaawipx.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt2lrcrjdtb.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt2benaijbf.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt2ubimetvg.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt2wpepvsgo.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt2ftsjexap.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2zvcpbjfi.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2cmeernnv.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2oeyycgrb.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt2ejzbkezg.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2aictqfke.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2yixyzksc.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2irbodbth.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt2iciaybfo.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2zhabytxc.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt2nyiyrwqg.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt2lysafkdg.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt2kfjeyowe.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt2dxtsxjar.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2ggocvymj.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2vpbxfbui.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt2zfvqmmkz.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt2gifqwiks.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2hqpxeanm.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2yujnvadv.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2nevvzkph.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt2jxnejoqb.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt2mtxtiqsr.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2eafinqgj.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2ytlaeqdw.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2slvsavis.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2moxokaog.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2arxzuodl.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2zgdoxmzd.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2gvnzsywo.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2kwczueos.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2fhavitfz.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt2rqcceqor.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2cdybmsbf.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2jytxjjvb.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2rqxzxqrw.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2dddnjqzo.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2ttchcflf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2oiiqumav.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2qyehfqwj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2khhvbvte.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2epolzdvk.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2wqxykwst.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2rikzwggf.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2kfuyemok.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2gaudiecw.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2jcmzfsqm.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2kajbiwjc.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2asxoeczd.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2sinxkphs.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2vfcabvdk.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2uroohmlj.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2uypsmbyx.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2cqsoxstt.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2zfjyzxvf.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2necnlfsi.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2ifyohblh.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2xisxnfar.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2pefsktwd.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2vanotodh.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2dfcyjcth.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2xiizelkw.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2emdtwclb.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2ztihhrfh.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2xugzfbzc.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2bzeevzhj.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2popepqyc.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2suffcpio.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2nzbswwbo.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2xcsqexxn.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2tcipqzbw.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2yybepuid.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2qkdwynty.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2fnkvoifb.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2fbydzxvk.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2korvzkww.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2lsrvviqz.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2qybikrnp.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2kiwjjrgu.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2vjjcelle.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2aejwyokx.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2jsclwjuv.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2sxfyzgmr.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2zmhddgpw.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2ywvndrcd.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2iahgrhrr.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2lmzauqta.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2zikvruab.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2rfgojmys.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2esitbeak.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2zfnpzrnk.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2urjgnvzw.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2gdavuhim.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2uxtzdbtb.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2ijjlvucx.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2dsbzauwe.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2fttgsgjp.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2iqdvavyv.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2nibbfhdm.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2bhoaklaw.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2bomcwcne.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2kszvbohi.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2xtynmwns.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2ttkaytzl.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2itgtwimm.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2jtixhcno.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2ontdfmxi.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2wwvmrruj.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2svvcukmk.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2fsdwultu.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2ajrkiwpm.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2wonksmjp.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2ecgstrqe.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2mlywbleg.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2ykugsnzd.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2gmydhqtz.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2vqepovre.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2gpxarbsw.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2wfonqouj.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2uiprjfja.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2inhvtgxt.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2vtmtgpyu.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2hrzqldum.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2rhuszfql.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2jikkoyfj.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2kqaufsmm.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2wcmuyqkn.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2tnodszsd.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2julfhlbk.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2gwedcpwx.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2vevsotnf.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2rpoiixik.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2zagoemsc.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2lziofdii.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2rmdgdbea.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2yjwepeyq.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2navhaiek.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2gdftvzcs.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2vxtndaqj.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2cuyyerkg.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2dbnzvaaz.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2zegezona.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2vjcunegm.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2ahwaqnfg.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2oiesndmx.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2mwjwasft.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2zqnsuogg.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2egxrdtov.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2kgyjygtc.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2hqclmskx.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2pihbqujw.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2gvpxkndg.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2cbktqgsw.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2xwetulgv.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2tayupnll.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2wlktqbzw.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2npgmyecl.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2pwcrglvc.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2xujceyqk.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2jucudumv.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2gfyfhtzc.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2vnpvidac.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2qsafsupi.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2mvrgngzt.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2reuucafl.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2utsdvhyf.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2lrldpivh.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2bkxbyrid.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2oxrpkrst.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2zhtfbadc.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2prebqbpf.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2vsmknsaq.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2ksxdwvnb.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2toxgvtgf.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2pntqqzwx.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2ffoxjdgv.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2uwommlsg.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2erfehvwo.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2vxehzwre.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2ppatpnij.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2dxxktvjm.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2lfmlmczn.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2yhkrqflc.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2dtzkksdp.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2hjfibsev.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2oyzrzqvq.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2ghsqrjtj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cybrntqc.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2gwrjunnu.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2fbycoafa.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2jyzhvstn.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2dyfhiqwn.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2dmxvkbjs.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2qycngbnx.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2xpumztgq.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2eaossphf.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2axxyqhie.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2oxcjlrfl.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2ihswcnej.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2rfivcrhl.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2thvnogkm.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2ktqapbrc.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2hupgjbul.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2nswckhjo.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2kdgxexao.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2nkxqutqo.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2wayikuqj.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2owvsfegp.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2ydtryapj.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2rivwdrbj.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2stxpwsra.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2hceejlxu.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2erpsfguc.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2pcnpterj.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2pmuhpzfy.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2glkorhkw.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2wlxnzyta.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2csvxdomv.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2hoqkkbqu.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2lodrszko.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2fxjqpxqt.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2sehbusku.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2rrckfgmc.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2obtndelm.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2voeqovqh.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2yldpsdim.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2lvtxlyiu.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2hsghgxeu.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2vdtqzmyl.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2lvhnhlxc.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2bhtikiwx.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2xfevmntk.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2taxlpcfu.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2savnoboz.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2amdarsny.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2osnlmasg.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2bbevyjzj.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2asvkflqx.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2qyhsgceq.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2nqahqxwv.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2bzrrerjp.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2yzodfggs.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2ezpcgrxn.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2gorhhgqy.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2gpwynczd.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2lqlqhdsz.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2hvxgpbsv.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2nmtbrank.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2qerjwxsk.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2keavsnjc.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2weywfaca.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2zsrgvntk.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2lztyksbr.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2jsobxaqb.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2nshvrrcw.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2xvsxoyki.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2wxzroysr.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2yrdgqybr.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2kvqzukwg.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2bpptspbk.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2dgjsyonf.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2vviupskz.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2rrbbrdrw.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2vsavruoi.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2nyfwnszt.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2tzyroltt.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2koaachbg.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2xkywlgxq.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2mzsdqgcf.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2sxfzeqht.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2gwyjtanb.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2tajbttvk.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2nlsxnffs.html


<!-- 参考信息 -->