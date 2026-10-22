代发 wailian999

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2pmbtgsyl.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt2ttaevdyr.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt2xkvamfia.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt2duuhwzbg.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt2jtfakgwc.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt2piwoksas.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt2rmdwyhxo.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt2xroxnllm.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt2uewwlvhj.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt2exhysjsz.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt2fwfxkmqx.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt2rbflhiro.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt2towlcuhn.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2feapnkje.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2lpoamxhc.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2tsqywzpl.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2jdgutfvn.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2qgfbpbnk.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2prmqnyvf.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt2uwriiwit.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt2bxlfspga.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt2fruxfnme.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt2xejydbtf.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt2ihqpsaig.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt2csoireda.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt2ppwwstpa.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt2aqfxcjrp.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt2wlcrqqig.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2qhhrjwbe.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2xlryrbvp.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2ycjrrhzq.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt2yjcwclpp.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2yrsbhple.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2zzsppqsd.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2sjcemhfb.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt2iyivfzfv.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2xnbmhyar.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt2rcnxxsow.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt2jkuaangn.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt2cnjxqxfm.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt2stqzorti.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2xuuahwtq.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2oousigec.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2hrvcaina.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt2crxptxga.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2opteedze.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2fislmrmw.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2wlwfkyyf.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt2mevanwdg.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2ccwdtmax.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2yfndhebl.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2leecpqkz.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt2skqrtblm.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2unwrnohl.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2qhfkhmnp.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2sdmxzmuq.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2zklqziyz.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2ckimdrdj.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2hrhltjbc.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2tqqplksx.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2mvipgqij.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2wsouehvt.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2dbidhbfd.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2ksiqfnev.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2zjkjxjpt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wuacvssi.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2fseaygar.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2aelhkdhz.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2loqyaxcx.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2vvnwyvdi.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2ujpckcna.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2mzvlexgu.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2vzdyoazx.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2xbzxugwo.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2apgzhlfq.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2yrzcokpq.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2gyvprrly.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2kdxtqojr.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2dcndtpvf.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2ocowfqrp.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2bmosyfoe.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2bmiebceh.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2avebuqad.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2sjymnfmn.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2jdioexvd.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2aqxqabat.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2hvyetipe.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2nniexvvi.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ilzcczmt.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2arsfczka.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2jarkvcdb.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2oqbfiywq.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2wbnjictz.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2slnlfful.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2swsjsnnq.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2nteaaory.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2qprggktj.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2wentkzww.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2wndrgbwl.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2wnsrloum.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2ohwvmgrr.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2slieunhz.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2shjlvbun.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2stayboma.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2tvacojxg.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2zupuqlrh.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2ygduyhtn.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2fvftjrao.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2hjohwetv.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2gwthfmle.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2ruyhhtig.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2biqchaox.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2jhpohzcd.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2vrmteawb.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2iepfyqrz.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2pjwivmer.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2yiphalgy.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2mqczmiju.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2ifirwnmt.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2zyowspsg.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2hwlvmjxu.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2jngwpzmv.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2tbdsivmb.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2ombzqmzm.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2yiamphqt.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2auejqzns.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2lncvvztn.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2nqnsnskd.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2duhutljf.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2myurguwa.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2xaqsmhje.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2gdnzbxaq.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2aqgfhbbp.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2mjqjlihu.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2ektnujpt.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2vgbftngm.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2dufsmsei.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2ttxskxqo.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2gnvvodaw.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2xgycirmc.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2lrbkkkdz.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2bzhplpau.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2dcrpxfgy.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2niqtxmnz.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2nboizyzv.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2pthxfque.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2syrgtfvq.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2bzeiouob.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2pswsfgfp.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2dbybpran.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2puegokar.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2mhixabxk.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2upfzeydq.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2buugwaqa.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2xudiflmo.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2njfrlwaw.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2ptmxdhrl.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2cbdawmno.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2ujcthcsu.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2cawmwrww.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2rpcimljb.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2gbnayqep.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2bzrlqgxd.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2kudlsqic.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2sruxdssw.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2gglrtlrl.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2lsetuuwu.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2dbiemsvv.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2oophdizz.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2jewpdnmi.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2eicogpml.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2yoiqpfpk.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2uenkfdpk.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2achtbvdu.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2rzuknctt.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2njnhiony.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2glxqtgju.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2ecpvqjuj.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2ymshooqz.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2docphorl.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2rfkzvzfx.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2ikjcaigy.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2sclgaunh.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2rrptoahn.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2tqvzvfxn.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2axgjjtoo.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2vblobjvk.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2kgdmnyho.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2hgrhwmii.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2junnkgqm.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2rbsxorqo.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2nsvgxruk.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2sbnyomop.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2slqbmmzx.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2rkiobmii.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2nyfxomso.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2llbuhyex.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2jlgballx.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2plarpuis.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2sxkwennz.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2bticdfbe.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2ptpcjheb.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2vrochuxd.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2wbsmxwpb.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2atcbkkcx.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2zezdwuda.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2pemfbkka.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2kbegaalm.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2fxnmvdha.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2wnbooird.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2upoczrfc.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2scfcqxfx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pjyjharb.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2hjoyoddr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vnevixal.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2zfkwrnjx.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2fuvwnzkk.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2fvnjmtyj.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2iqvgmirv.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2gxbfpmxp.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2urecrikb.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2uwqbrqxd.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2sflikuzt.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2bcoljeqg.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2lmgyfmyp.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2hpxlayft.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2cwcufigs.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2dshfixmu.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2rzdpobgr.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2rshjsdlw.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2affxtbxj.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2totwlhyj.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2xhxrdjxo.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2ndmczloi.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2qwvpjsac.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2atevbrbf.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2iclnvvlx.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2wydvsamg.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2jayzrqkh.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2rsnfekqg.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2vdvorhhh.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2lodgifha.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2zntftpbo.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2kzxezead.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2qehdmuty.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2sijdqlcv.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2fquvzjlf.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2zrkyzndt.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2dwpcigwt.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2smguamun.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2yviglcqj.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2goozidze.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2ovhxbogn.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2bumrfyri.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2hemtgftg.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2wrptmhtx.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2wdarkgzn.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2tndtaoxl.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2jdzbxwhq.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2ntzgevxo.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2kclmniiz.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2wxoroszc.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2sqfpacez.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2rpjywjdm.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2lvxqoupg.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2xminsstj.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2ptjpzhlo.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2lnqxggan.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2ftwgrfhy.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2fnhdzqnq.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2wodkrcyx.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2iazcwufu.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2qgddsnzu.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2mcoxptzq.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ogkswtgc.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2wljfztvi.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2kdndxwre.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2phrplxjw.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2sgeszstq.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2fnrqdcop.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2pocejovt.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2qdbmrkeo.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2benhmtqv.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2xsaicfxh.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2smvydzaz.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2zglhvgxm.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2mjfeuzkg.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2blnxcxhd.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2kqtmzcbc.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2vtjkdepv.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2thyjhbus.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2xupbkxng.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2iprylnpy.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2ylgklcuh.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2bjzazlyz.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2ipfeqoig.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2cxdvckfd.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2culwlvya.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2sqkrzqgt.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2zbberyay.html


<!-- 参考信息 -->