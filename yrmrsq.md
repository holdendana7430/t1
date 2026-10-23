代发 wailian999

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3ndhjnuup.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt3cjrkgvul.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt3fcoglsbo.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt3npvrlhtg.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt3cyfvkdpe.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt3lkbzdccg.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3gpowecmq.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt3kyxjdxqi.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3zsokyvmv.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3kiwgwqwy.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt3vvrhoomj.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3tyzovcks.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3rlohulgw.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt3fsjchnnk.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt3sblqdmcx.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt3kwfpepla.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt3kyoizntv.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt3lenmpkvp.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt3dvivpfzl.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt3hymrkzaa.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt3rrsrzncq.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt3nmpyhoyb.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt3ftljuhgw.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt3msldjwdw.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt3tqvxowgr.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3znadhlnu.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3soumkgaq.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3vwqhsmyp.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3gnebspfu.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3bdoegkrf.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3boevfubv.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt3lnmmqdwi.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt3zrscgurq.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3teimacrs.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt3qvqjzgcg.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt3ekyjjomi.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt3qafmohxx.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt3piwhrcoe.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt3tpyvgwuv.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt3cylvqsfk.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt3rjajesfd.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3ficigpkr.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt3amzuvxth.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt3hguyorgu.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3fedrfqbr.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3pceakccw.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3sbeqioso.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt3emdnwqcc.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3temrssbu.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt3jihvotjh.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt3zrxqxarg.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt3gfiqmscd.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt3onjjgvnj.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3ohyvexee.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3litcdzpl.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt3txlpuzgr.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ybjtprdr.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt3uiscuxws.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3biegqhej.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3mfyjwjaf.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt3frqrmplx.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3yfgajyqg.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3gxzbahyk.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3sgaphecy.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt3omoconjr.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3rgjlumxe.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt3natnbeom.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3ndupaosl.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3pygtvhkw.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3qsfyvhkz.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3ihjurrmo.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt3tlnkwrdx.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3gmycizxi.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3wylztjjf.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt3erohksot.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt3ojynkfsq.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3ulsixmky.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cewihukv.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt3ybwtdzcz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3chufhemq.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3capvlvbp.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3bhnoskyc.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3fucdyekn.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3lhevzxzp.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3kqnqycwa.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3zebihxyc.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3wcijgoxu.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3oqgctvql.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3gajahnmw.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3swssggaq.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3sbihpsbr.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt3ylsnbizv.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3qcieaeoj.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3jjtkgdxm.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3hotfekgj.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3hjnmvuxx.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3attlpuvk.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3ppanctqs.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3tjvnefla.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3zqtiaosd.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3hazsecyc.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3jxxmtchi.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3vqimzoln.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3elqojwye.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3qhgbumtm.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3ishypngk.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3befdxaix.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3hmkiglbj.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3kxmwneuc.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3nlribhde.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3uoxpteia.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3gacfdana.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3gtujtlmy.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3phhixuij.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3vwyterjw.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3xvciyhnb.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3fwwklggg.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3buglaicg.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3zryfomct.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3xfppsnpr.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3mauujfmx.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3wvckppzv.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3jfuiippt.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3vydilphj.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3nygbwfoa.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3bbsqytrc.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3jenhrlfu.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3rrxxnwtl.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3hxottawy.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3ifvbcxgv.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3pxnpbedf.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3djqucxtv.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3oxazumgb.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3gtigwawg.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3thtzkjwz.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3vcexfkeg.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3tzkblznc.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3cygstrss.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3zsugvudd.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3wbalnuuj.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3ducioyud.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3gmoigijp.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3cjkwevtt.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3vxsdvale.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3vnbaokvd.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3rqshhzme.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3lltytjca.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3jawidznf.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3fnuzoxkz.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3geaecbao.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3vljgxjwv.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3phjulwfo.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3wgpuqfay.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3phltxyod.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3caohwzea.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3adyftqkw.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3zabiphhl.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3fdvkccoa.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3vdhfghyz.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3ewhmryqp.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3ohwzlibn.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3bvloxzrr.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3mfcgwwut.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3gyabourk.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3wymkbgpd.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3hdjwmlsv.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3wqiemkzi.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3nhvhunsn.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3tllbafmj.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3auklryfd.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3lkkckrrq.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3iwatdmyj.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3hipacrta.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3nrehpirp.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3rgcdgyby.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3niamqupj.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3bujcpvro.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3xmiikdim.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3kddohxti.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3kipxjfzi.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3rathlqfo.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3btkivanb.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3sjzhylmc.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3kowoegue.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3curroskg.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3mibemoyb.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3nctpexlh.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3nmqhfyex.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3gsxkrtkb.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3jkhxllxt.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3daeargrf.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3bfqxnxlc.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3pfgcfoek.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3ppxtzjzo.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3jrnuyuvk.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3lcvxppie.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3vbpsryga.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3yjctkwmv.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3whzaibpi.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3jvrwzfcv.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3fdkctesu.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3vydempdt.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3jytjzujv.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3keywigkf.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3mgoheani.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3ldqarnkz.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3lcrqwqyh.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3cjdogttr.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3uyylvimy.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3sikcvxok.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3rkmpzrsn.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3gufvrwzr.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3trjfhydb.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3cseetvbf.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3mfcbwzxv.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3dpqizlvz.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3hkfikqqj.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3jwhsgsuk.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3diruycip.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3nzsqjaxg.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3ozqntzxa.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3hmlkylkn.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3upchhreg.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3qmiarcrf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pgieuhej.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3zbmcaecr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ppfuxqce.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3ibwnvrqt.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3jhyteoso.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3mmnkjgls.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3hbgtrise.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3uutwxejf.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3dgmjymfg.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3amlgpuft.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3dpkekwtg.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3lcuyojne.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3fawtqxxb.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3iseaoscs.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3gsvptvrq.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3scoirezh.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3oqkhzygd.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3fczcislm.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3rjnwyvvo.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3bzsyhsfe.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3abnkgbow.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3obeirpgw.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3jvewzkmp.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3trkdaxrn.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3whnejsom.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3ydaukwkl.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3adeeyhks.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3igxehrzm.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3mxukmomk.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3jtpjclkg.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3eswrdxja.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3ydhyqzug.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3suqpqzst.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3dbgmfyfa.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3vdiyfcpq.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3vgnurmfw.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3qhvtzssb.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3wbkqrhvn.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3hysxqpur.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3rexllhnv.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3nwylvesr.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3fdczjnby.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3yfnyppnd.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3qpzguzck.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3wajitdch.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3zjazdulk.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3nzovxbxz.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3ffqwicjg.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3izkubaqe.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3bkotbnkj.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3sxrvromj.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3gakvzyik.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3fvxfrshg.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3fdwdwisz.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3ggzzcmax.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3anaryujq.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3peuemtnb.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3bjdrrvqg.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3djyjsngz.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3yvghyzpn.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3rdonwyox.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3rmlbkdwa.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3hxvrecmt.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3spomhbut.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3cpzdfzql.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3jieaugzz.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3xjacxfkq.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3gecxcmzc.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3bcjqrnko.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3xdfpzlzb.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3rpuydbqx.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3pwedashi.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3waglcgwo.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3yjlcrrdh.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3bttsapjn.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3lqnbrchd.html


<!-- 参考信息 -->