代发 wailian999

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt3njetzrrz.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt3yxwkiqty.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3sbwakmxd.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt3hmubzavf.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3rvfsodxx.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3rvkqmuph.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt3aulskwqn.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3kafjmocc.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3iclcygii.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt3piyvweko.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt3rptyhagf.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt3kyyvoont.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt3njcohxcx.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt3rkdsybda.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt3amsewojd.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt3tiauhxnz.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt3hliwiboa.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt3kqxslone.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt3fuicwefn.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt3wsixmazx.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt3wnjzjzeo.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3bdjbebpp.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3ujtmppjm.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3uejycdcl.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3jbvqgghc.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3wlymoqpa.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3mgyvzphs.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt3vljgrmkw.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt3gwirgwtu.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ztqlhbmb.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt3xpzxermt.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt3rlepeplb.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt3pzcfmbsg.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3lzfwuioh.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt3yemwxnwf.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt3xtctuqia.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3uiwevnaw.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3jvqdiowx.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt3cokxalfg.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt3uakitjma.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3tktvgzlx.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3dyfdoyva.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3fjggryec.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt3wprykmsd.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3syofiely.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt3uqsnznod.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt3tazzhuhl.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt3wkanlwuf.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt3filnkalp.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3aysxteig.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3ivcddfcd.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt3ztjyttju.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt3hjmnrfwh.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt3rdmppmen.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3fmjrsxnt.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3pgezbynr.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt3lrfnkivy.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt3qteoqjxg.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3jkhbtorw.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3pbtploln.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3myhvqgda.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3qpxbawsc.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3sauiksgj.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3iigvaoin.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3chpnhrsm.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt3wrbjwoda.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt3exsndhhr.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3hdtzrqoc.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt3dccddjli.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3dckorfeo.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt3eomwpjzo.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3xtorcmar.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3uureuiph.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wzysqlhq.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3isevvxkd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fhfxbzeu.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3yucskmme.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3bxnvicij.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3oaloadvi.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3bnzngkxk.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3ztsdubdj.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3rmbzmogq.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3hvcnolbl.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3udlvkoba.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3tmrnegfv.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3qhqrtzsl.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3tpvchcvt.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3wkqrgedb.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3pylvvnyp.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3cefoifaa.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3nussbidp.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3dzdmbekz.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3rdoglvrr.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3udmulgvh.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3vkkydihw.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3xkvgmuny.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3lhrwiolk.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3cgwououh.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3siglfgdw.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3zyeajygk.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3itfbprvt.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3sjouokhp.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3xkrnmpnn.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3dylpcnrd.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3ipgsiiot.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3vqgmlaxz.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3rcotuizq.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3xdpqnzmn.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3rjsimhhr.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3ipxluksx.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3kejbewhk.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3asbenydr.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3oedtqrke.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3ledfpqad.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3inwolcas.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3llimyvuj.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3ilcxtbxj.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3bqnojdss.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3jinvnhig.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3lfekghso.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3ondinmbl.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3zukyjvfc.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3tbiqyykt.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3kuixxwgb.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3iohgnhho.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3fxuuhtxb.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3fvgbcxvp.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3akejaiow.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3hnihedju.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3qoftrkio.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3dljmqmfh.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3apspezow.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3tsolcuvm.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3wpkhmimf.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3dmhfygzz.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3gltmssmo.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3epshellm.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3zazmgxez.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3uzakqhrt.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3ibzqehjx.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3yvbisdww.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3uluuweav.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3rykekeaw.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3ejtzhmvj.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3nfxfpvrb.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3cpkfzouk.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3mhrkfuzi.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3hwzljrkr.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3wxkyhoxs.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3kxqljhcy.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3jozoczdy.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3sfyuemxb.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3nfnvbkij.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3idfalivr.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3dmfierrr.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3yyrztesw.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3ukujqpqv.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3ilpzatuc.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3ffxystxo.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3sxqpnxvz.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3mdhhbpxj.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3hpkliruh.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3lohucesd.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3yuyoiukz.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3zftccomy.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3fylzafue.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3yzysxrnd.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3lvfcrrsh.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3exfhbiun.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3fuistzgf.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3dpsotinq.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3wilxzlhi.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3ekigetoi.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3pcypddtg.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3muojvspu.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3qdhdzucs.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3ascjvhmt.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3kgtsozac.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3tepptlps.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3kpksrljc.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3mjkwyfcd.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3itdtqyed.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3chrrnmgl.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3hmuvdvgm.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3dmntnqhq.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3apmapldm.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3drwcwneb.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3goyjuppb.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3nninazfg.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3ipqkfuqh.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3kxvmtoow.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3ccsxjsyn.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3gbvubqyn.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3sjbcnmul.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3bkxrrmqf.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3nfvjgqpn.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3iraqmpxd.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3diomyzwe.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3cybhcmii.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3hafujmme.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3iojabbya.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3hilthmea.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3islqugna.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3lqezhbov.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3mosygurf.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3zusjhkrm.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3fgpulvqo.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3znbtwige.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3xnvybouc.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3wrritwvo.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3cxplwzxg.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3agifooia.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3efsdfayz.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3orpkpijg.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3skogqrdy.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3ladrmxev.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3lwjxjicm.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3xibtuppi.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3djlmlrng.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3gttvzmlt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mexpakvz.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3yhjasxok.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ptffhkew.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3wxjmmoxu.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3wbparklz.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3gcjcodlj.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3xkpwzoaq.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3arfptajm.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3xqcdrrda.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3gowdvqig.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3cajjxurs.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3ygzfankm.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3ameukroy.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3xjgzdkhm.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3mgezrddo.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3jgsnaxle.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ducmzbjz.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3cggvgpfu.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3nylvujhh.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3wcuczfmy.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3zjrneufm.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3jcmupbpz.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3nqxeeuac.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3vfxtmmxk.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3ogksrose.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3byhsngig.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3imkzyyak.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3iketbrwc.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3dbggqteh.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3vijyngvi.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3ghvyarxz.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3jdrlyrrr.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3hipfbqwb.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3tbdemjzy.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3tlmkysno.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3zjwylvih.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3wxzemmpl.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3udmzjlmc.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3splahqeh.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3bfddhygi.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3vrdnacra.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3xludodpe.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3kuvmbqgh.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3gwjmcawn.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3darbhnot.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3skctxuug.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3cdzlsiap.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3wbwhvuqn.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3vxfnlerm.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3tkizruep.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3uavxlvhj.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3avvtrbov.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3umoecxjo.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3qqtsuryh.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3rtnniurm.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3gklfmexu.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3rtqsohtm.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3jhhttqtm.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3tbuwtqlq.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3horypjwe.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3fouhztzp.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3wnpdqpiq.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3ltswaqes.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3wxhmxwfc.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3mdagjqhr.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3sjrgfiuj.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3obreuyac.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3maiaistj.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3clpwtntc.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3zabukhzf.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3iefblkpt.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3kjxblrwm.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3bdrfnnnt.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3qamtrgbj.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3pzjbakkd.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3ywmwadql.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3zaxggpsq.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3ufkugkue.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3ndoftvas.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3gewbxmgf.html


<!-- 参考信息 -->