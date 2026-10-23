代发 wailian999

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt3dgeqhziv.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3nqzcyejx.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3rpjucrbq.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3prghskti.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3tvgglnsc.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt3yndegnak.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt3vmyooidb.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt3hoeeheum.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt3wguqyiiw.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt3idsbnafu.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3pkszvklt.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt3xfesyigv.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3dpfkqrbx.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3jaukzkrc.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt3dzmbtmue.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3yyrwdgii.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3lqolllky.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt3dfwycule.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt3radxrgiw.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt3vxplifaa.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt3puqxiccq.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt3vtjjfsxg.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt3xgkzeidv.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt3gcashndq.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt3qwcuqxpa.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt3tkzpbqqw.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt3isiuvfhy.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt3fifldxba.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt3xdialufx.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3wcsmymhw.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3llyjxdbb.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3hpmwrvai.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3acawupky.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3vrfyzhyt.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3hhksuhhf.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt3xzqnfeqd.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3wzsbwvbp.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt3avyznjcb.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt3awovsogg.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt3kkrmjcgy.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt3gywkkexq.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt3clwssnrd.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3xjijeuig.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt3rurdtjtk.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt3upxorngk.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3cudaikdt.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3bnkrasaw.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt3yyncrekd.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3pezuxegv.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3gpbizuju.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3wdjfpoud.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt3sylqvxxg.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3dryklwfl.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt3xsarrtrs.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt3fgajaizm.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt3vavieazb.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt3nwfperay.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3cxjovkyu.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3fntlbgvc.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt3davqmbvu.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt3dnwmbnvd.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt3uthazspy.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3lnrayhas.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3ewwcpcnr.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt3xhrlpskr.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3swqprkpi.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3pouxjozn.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3uhcfarbb.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3vlmafmdg.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3voooakoi.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3hwtmqywu.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3hictoigq.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3mblxegwl.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3nplgvspv.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3jikepfhs.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3qiwsydps.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3bkigdwnx.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3cjowqfrv.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3jfoybrqz.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3kyyebsxj.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3iixtyjyn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3icejpjnk.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3cxpfdmni.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3buzmjcnd.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3jdbzgdgk.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3lyknydhb.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3qiiqovsn.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3obyhscth.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3oogtvbgf.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3vhunjtqe.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3psrbcnya.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3nvivokek.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3hwmlwvai.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3cnabehrj.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3ohebnrvs.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt3ncjrhmpu.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3mrhcesee.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3qennkorc.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3ywrkydxx.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3cspijijl.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3mwgpsntr.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3rnjxlwgy.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3tywslfma.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3jrlrshge.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3oauwkdlw.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3cjumtffb.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ueicxkrq.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3fldhfzlg.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3vvlxfvra.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3effciwsn.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3sgwereng.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3jmbzhqdf.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3zyjrgfpb.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3xppvlqzg.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3tbjazfnk.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3wmfytfen.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3uinzroiv.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3zylgmkkc.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3rnrsvnse.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3bktjshfs.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3urbmedmu.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3kbzbjkfk.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3pdmhwycz.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3jhlbvufj.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3ohqnsygh.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3dozkrbwy.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3dvfhdina.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3sukcbnpp.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3xglrcefi.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3iwpjscvd.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3aibrqqdw.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3jabzfhwd.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3iokslqcz.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3xwqqctba.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3bevdnfaa.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3ehthiich.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3rpsugomd.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3alvuexvk.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3lfycbvzp.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3ftxlftyg.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3rdisoipj.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3uyzithnd.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3jsfxrgid.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3kupmojrq.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3cgggtqqu.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3etupowhe.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3mbaejqcg.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3trfotlbt.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3ubvoqmjj.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3ronlwxjf.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3bpgifmkf.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3tunodmfb.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3kyqbbyen.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3qvvznsks.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3fkcwpawy.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3zqunjghl.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3ugvmcdse.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3fufbidvg.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3totvmulv.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3akiaszcj.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3oorupfqj.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3emekseoy.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3uzlweijn.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3rwtrwfvm.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3frwiapdm.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3gqbytuhj.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3alrdyvzy.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3tyryxolw.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3auyjwfes.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3bxsgdiug.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3eimjkofy.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3htcrcduy.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3wbqclywz.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3dsgfmzhc.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3wkhowgki.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3txveuaod.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3rxzpoprl.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3mhszcrdz.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3ljtgysww.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3raiubwce.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3aikankpj.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3xwxrstpg.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3pamefoqn.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3dbzhcvxd.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3cbhyrpwl.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3tywfexkj.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3cuhqcksg.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3untaomav.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3whyteqlv.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3mdrwknsk.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3vdefzgmw.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3wylzgjhs.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3jypejtou.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3rhgajwqx.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3bafonmjb.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3rnmtxbyp.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ijtydchy.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3dxympfzn.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3jmjjjdqu.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3tzjwlyqt.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3jfizjvhz.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3jhnjbnyv.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3yxbtvmjo.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3vqoplkqs.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3omkbczee.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3qrjptxhw.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3kwercvji.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3oruwaexl.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3mybpzqif.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3tqmmwcxf.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3wfaybkox.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3iartstdn.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3ylgpguyn.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3qbkmfrwf.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3tmwynyux.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3edbahyer.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3szwzpphy.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3ioklnljg.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3emxfnqsa.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3smjjzqlo.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3dsuzhwpm.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3xtzidcdx.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3uhrfrpid.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3nflkxlvz.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3xgdbozkj.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3nnevrlnn.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3zpiwomwz.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3mcuwzdvv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cizmcttk.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3xgqnuhhy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yrlrgvog.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3ybcxqsyl.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3dfkkfpjz.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3bpisouns.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3kqrzqwbk.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3wsvggpkt.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3fnpexkhq.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3kgqclmfi.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3jyidunix.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3smmagbcl.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3gdrwrmol.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3rmwkadyw.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3xajtujui.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3uvzzidqp.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3cigjvdrw.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3yxtyuhfc.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3yvprqotl.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3oxmmuzhs.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3uqpsqfrs.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3mjgiwabh.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3cfvioeva.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3rphqyudl.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3kfqenxla.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3wmeggsgs.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3xnibtaca.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3bkifspji.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3nbxdjlii.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3uqsntplo.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3jfwthloy.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3whlpnnav.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3ubbzyuml.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jjnhgynm.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3iqaoavfh.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3vplgidhk.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3wmardtuv.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3zxtkxepe.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3qfirrlwf.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3kiohnein.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3wlwspnkg.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3uglndrht.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3ykvvgxng.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3pihmijyt.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3xdwfhyje.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3uigrzubv.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3ojsmohwa.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3egbeznlz.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3jqssvaby.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3igwhosuq.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3ukgypeol.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3hnmlfmuo.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3kucbszhe.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3mxzejvrb.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3zjynfjyt.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3ybugkzkn.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3iokkptrs.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3yjwomsvf.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3wuucymqt.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3pohoudxg.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3ffyhlzzd.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3cpdvzido.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3tnoyyaai.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3sypsxhdd.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3bkfahdqt.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3yqjvzmwb.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3wfzjplpu.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3lskjnrlr.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3tmlhwiyl.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3blblzgsr.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3tthekfqt.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3rrymfihe.html


<!-- 参考信息 -->