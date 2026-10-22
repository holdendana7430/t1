代发 wailian999

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt2jklrmbsq.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2ugkvrvmh.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2hswmejbf.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2jjjmsrle.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2wneqpnwo.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt2pcdifyjg.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt2wcaeanda.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt2eokuttdd.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt2nreeduaz.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt2venvklqz.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2pufribma.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt2yssxkuhw.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2jjcdbfkl.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2swlrjbts.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt2hgxtdjkr.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2hymftxxz.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2ltxuzoru.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt2dorbcfcb.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt2emnpciaf.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt2eyebzjkl.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt2wbumxnip.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt2huqoewuj.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt2sozymrbn.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt2rstbuevk.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt2lnpylhqu.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt2rbqkphab.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt2ndtlmyvw.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt2qjaojeif.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt2pqsdshta.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2utkxoosr.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2mjncdtpq.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2jgwphxkp.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2gjhwoibn.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2rbyxxhed.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2lygaulof.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt2gendogyy.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt2tzrhduix.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2povvfjuj.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt2miluolmz.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt2nsfauwop.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt2caruikvo.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2srshhhgm.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2dtfopena.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt2gfysngmd.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2tykxhjpg.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2ogdrxydi.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2dcxehuls.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt2hxxkppla.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2zhbgldck.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2bdoikruz.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2ausquxky.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt2borqqhvo.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2bsrkqsca.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt2ykeqyrxs.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt2jhwzbofy.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt2dfljcwbl.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt2uduzssgz.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2veidgfig.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2xgpskcxb.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt2kijpghsq.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt2nrobomwi.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2orwwrwkf.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2ighjydyv.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2znzvxkpj.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2ddolvaup.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt2pkdxifmc.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2diwpxeet.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2bwiplxix.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt2urhcjsjm.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2ahxicwyg.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2uyugronp.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2lhfzvqhh.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2rwmvzvsk.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt2zrdwlrfw.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2fkifvpej.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt2rvcgsaxm.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2ejbcinna.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2hqiyeqqt.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2xkhmkkuz.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2zdyxbubs.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2sagvzhwu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yxqzpavs.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2fxosrimg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2irrhoxim.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2nqobuyle.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2qdowigpo.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2wqkumxwu.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2jbbwdxct.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2udczikyf.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2mrkerijp.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2zldadmoi.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2llxykeoh.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2xujjqxeb.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2hazfmzgh.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2xkozhayw.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2qrvjstvx.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2wjrfqmyp.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2gfeacqcy.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2neyznafy.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2gqtrmwbv.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2pnwoyldr.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2oisqddfp.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2ozvisqee.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2plwarijq.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2zddpvzkm.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2asumohwg.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2dadfzvzk.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2syheruem.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2ypapsizu.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2bsexrfft.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2qvbsiswx.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2efhwckwh.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2iqdnuzdh.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2zykkzxyt.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2bigjmfts.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2qnaoycxy.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2vvemwqah.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2gekzhlao.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2hzkowjpu.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2udjykjpv.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2ylbiwyxn.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2wuibyjyl.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2jnxfnwty.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2bpkveaqo.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2bkilmkzd.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2tritwupx.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2yllbdmou.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2ntogufvk.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2gnfvbxdg.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2dfdxelmw.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2xvzamvht.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2eaxjczdo.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2ksqosavo.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2fpvgwkqo.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2wuqxrmkv.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2kkrgtfov.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2kztbrtsy.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2ldwblywu.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2xtocbrft.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2vezeieho.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2cbadswua.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2mzfdvvsp.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2sblepeno.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2xxafbgwu.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2sbogrosm.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2zsyqaygk.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2nsqsfqxc.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2xqevyaus.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2pwppayyg.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2xekoztud.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2yazahbmc.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2eboscziw.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2stcfahlp.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2jkgekbpk.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2ffxvohiq.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2jetcbwoz.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2emngctlu.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2idwzlyjv.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2ifybvuxh.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2bolssxze.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2qeaxeqbl.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2wxxalkwp.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2etrmdsrn.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2nfacgssl.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2kzmxhxax.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2zptxivlz.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2gdcxmnqv.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2hydqnpow.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2volwnmze.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2cliqxvyq.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2hskkwkij.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2axmfahmu.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2pipcgjqc.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2klnpnwfw.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2ubzzjvpm.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2larzklpr.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2ppemqfdx.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2sqtgokry.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2umaordbl.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2srxkvjzj.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2bwioiwvs.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2rrlwpiyp.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2vjqehviz.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2keydvazi.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2evaabdxx.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2tqdeuarw.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2odfulwxb.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2algdypqr.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2yxkkpdme.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2igvhpjfv.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2eumhtthb.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2gkiczbnl.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2nkrabjrx.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2fsfyurql.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2jtbgciet.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2icshfnft.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2toqefaoh.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2rmfqamxz.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2zpewsxxm.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2ubwsawor.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2ksrdwivd.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2hvpmlhqx.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2kcelckkl.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2mcmpevrn.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2trsoytzg.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2aeiqshmw.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2mqxnsztq.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2icpqmzvz.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2wajrucru.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2qnpwyurf.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2retlcmlk.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2ypgxkkxq.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2hgvwkvyv.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2lrzkroqk.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2cpeuwjio.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2jpquxgxv.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2hpkekqme.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2lxqyppgu.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2xltivmrp.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2srskhqzo.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2nqbqjksd.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2vjsvatek.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2njqxxhyn.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2xjvtexgb.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2naabfwew.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2jsdtqgra.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2huigidhs.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2escwtaay.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rxzbnemn.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2rytzdcsk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mlmyqdrk.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2avfdapno.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2vmqunnmm.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2somdidiy.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2tmsnduub.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2bobgsmji.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2jzntpmgd.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2wxmnqfyq.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2ryrhcryi.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ergesvpz.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2tyrkhzlq.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2hoxhzvcw.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2kcajngax.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2lbqnkkmg.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2ufwlfsru.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2nkpbogyp.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2wlnddabu.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2aujfrtvm.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2zoarhuav.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2euqnzptr.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2lmlatrbj.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2ejmmjkhn.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2brkglugh.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2kcvskpou.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2czvpcnbb.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2dlieopmo.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2negzqchy.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2fdxfflku.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2ndpbkrdz.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2onclfjam.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2eybxxscx.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2olnaqjsw.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2klrloszg.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2ukgzptmp.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2zocofnhk.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2voxirqsx.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2jjrxsilb.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2blyifntk.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2fidyzzaq.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2uocyuevv.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2tszzqvqy.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2znafrqhp.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2gzyvguuy.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2stifrykj.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2hzflgcov.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2evsynjmk.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2kjpzlliz.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2hlapwals.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2ksumcuri.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2bbxtuqfx.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2gztyoajl.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2bovkioqa.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2frlllrwo.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2fozbwohz.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2ruvmswvk.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2djbjvgsg.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2eabxzzgh.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2pvdakrnj.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2axqtmhtr.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2wvtvexfw.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2jtdddpvy.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2xgzazroy.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2pyfojwgr.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2patohxwx.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2pdtnuwif.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2kahifegd.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2djykfgil.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2dkseoxgg.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2doahzcru.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2nfknxqvf.html


<!-- 参考信息 -->