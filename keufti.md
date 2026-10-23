代发 wailian999

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3bekyuqzu.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3embqawfd.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt3kkwzgqtj.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3dnyukhqy.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3umudfian.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt3ldhsxydk.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt3angvzcsb.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt3ahlxyyyf.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt3rpsrntmu.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt3hpyzzmor.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt3fnwebhkl.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt3hlxjnkwx.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt3ocxyqqsy.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt3xcmvnimd.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt3agpkrhnt.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt3qlfnyaoy.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt3cqgccqen.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3krqxnujz.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3odnylrfv.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3vvqvfwgq.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3bjqltxeo.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3yhtwbbhd.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3kvmzkwzy.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt3rphnmitv.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt3xjkhyuzy.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt3tlpfdujl.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt3fohohddb.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt3cwswdsyh.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt3iuvaxbhc.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3hnieowwi.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt3ilnfgbzi.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt3tdxkeldj.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3ccaseaul.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3ydvdxyqp.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt3argimfvx.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt3cngohmne.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3xyjutqda.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3agxrbyqc.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3cvoymzez.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt3uqarcgon.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3xnllvdqt.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt3vzkkzztz.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt3sgzxbjfj.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt3qvkzqpgd.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt3anzxvpqg.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3rnhcgkxp.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3dcbmjhaz.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt3dayeklql.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt3oebcjjhg.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt3rxobjhxs.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3ddhrshlk.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3aueyrztp.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt3ffyjpsrg.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt3chydicun.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3ysjnglql.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3fihrfgju.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3ycuxcwxp.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3lknqzkro.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3izmvusrw.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3lqiqriib.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3zlqtdalx.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3akjdufyp.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3ncvcncwx.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt3aunkbsdk.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3cngpfitp.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3xncdovqd.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt3eaorbvax.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3waogjido.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3xthaflen.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gwauoxoi.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt3vwdtueue.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bfscyweq.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3exnpwoar.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3eathmkqe.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3uyuturzr.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3msgefuwb.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3zdulnqtg.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3kpeikrer.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3dplipxuf.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3qvlolfkk.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3duqcjoyz.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3covfkvwg.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3apcuosov.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt3aoxrbvxy.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3lphhlule.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3hbxmijun.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3fsxcufag.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3bmxynafa.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3acpezkzd.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3zabrxqpe.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3wmfmjkzm.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3zhaxlawm.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3vlgtsxwu.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3gpkgiwlk.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3wceumdop.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3kgzeohnl.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3dyjzlrch.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3tffiyqim.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3igkwmfnf.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3czarpzzm.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3aqupdtus.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3vbqesant.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3iukxmawy.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3ckunxbof.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3pulxhmux.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3jqqnwshy.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3fqusoxar.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3zvstwxmd.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3tuwvqwbc.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3akzspbfn.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3qrcvosbk.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3svrnrwbm.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3tzqbjsei.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3fwzuvzjx.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3uhyewmix.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3kkiaipdc.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3vqmwygtq.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3sclnjeyc.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3gahprbto.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3lomlvmma.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3patowezr.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3ccmkdwyv.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3kqmuanhx.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3agoyeyyo.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3meucypyv.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3zkhdstse.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3ehizkrev.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3vobtxsim.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3cowmyfcv.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3kzcxlijf.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3bblagguv.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3acckeltd.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3gtyhfscp.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3goqvqxnn.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3jqfdxoaz.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3zhualmbz.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3mnrwsvhp.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3fywslesu.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3wdrjsxcd.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3qojefjft.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3juaxfzxc.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3bviwmgdt.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3gmjeeiml.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3xkpfotlw.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3stkhdidx.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3pudtxcmv.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3amgtyffz.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3kzthvtzi.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3ijzdratk.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3razgydvt.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3wnsuqhoo.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3gozsdwou.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3jtuqaumw.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3klzaubnr.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3ofprnsxu.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3celbarqo.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3pxubqltk.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3hnlsrhmb.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3jutjojxx.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3qeovzaqa.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3rhxddmmf.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3wqdrchgy.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3juzwrnjk.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3yvqdpvlj.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3nfaanrhv.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3imzrzxki.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3avgjmpbt.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3vwhgaweo.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3hzdqwwvx.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3ebutrjlz.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3sqhujloe.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3yzggbbxn.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3rbhfhiaw.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3whtnxuri.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3rqghspha.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3nihcbssn.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3detvgebl.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3xbwlccvs.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3mwvnigyl.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3zldsqcno.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3kvhahrqg.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3kachjebn.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3popyqrbd.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3heefiqep.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3hgagdtfr.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3wvzcseoc.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3twrsaxyw.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3adxpwlzr.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3oouahtex.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3teiquekr.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3wjtpgxln.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3qtcbeyso.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3ehblnnyu.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3dwsrinwx.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3aujivmea.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3kdssnpiq.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3pdyiaqwv.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3hgrxqhov.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3hphquvoh.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3cbhmkead.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3bmnnmleh.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3hpsdzdue.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3yxlrmjtd.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3wbnvbwbc.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3rewjuuuv.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3pwqmhbzv.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3mhdtpvnt.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3grbnkyxj.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3pkaryjpl.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3svelzjhy.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3osxxdxge.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3aiouiyqq.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3qkywfwam.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3ssjnepxr.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3vrkczkec.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3ilxcjajr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3todlsrcl.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3ohirpctk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vexqlsig.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3wgeyozor.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3tglptpdy.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3fcccajae.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3nqpwzmzz.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3mivwbafk.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3idpypzed.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3nagdybla.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3jxuqkfja.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3gqrlhqkr.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3rmfgdwds.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3juqujhis.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3kdbnpfzx.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3kxpqgxnu.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3xwboubgj.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3rmgpigyz.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3jbrndvqm.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3hqadrhdu.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3bopqrqgp.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3vcwsmtxi.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3aahxnexu.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3pptfjlvv.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3pdvcwabu.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3cllsgzuw.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3caaudizw.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3umzjclrc.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3pabtozlv.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3nqvjprib.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3giqoyuqs.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3fkvtfyfu.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3srngkynr.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3xnogzkmv.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3cdtxmefr.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3bwsupsyl.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3yuuvkxxn.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3cbwtihwg.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3yixrqejp.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3dlzibmul.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3vkntfwcj.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3yjowrinm.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3tyidzrfy.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3fyeyjrjf.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3qdoqgfhw.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3eqxjpafp.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3qgivghrf.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3jgebhgvr.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3alljlosy.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3asuiahvj.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3lqnhohhn.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3wswevzzp.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3mxhpidfw.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3kgdfhifs.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3wsihixbv.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3unrrriys.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3hiaifbmj.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3lvksxupq.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3yzlkusfj.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3unggmtvu.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3sgzgjhlq.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3axezyeay.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3zwrbdoeu.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3poapzazz.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3gcidlqbl.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3ropjllgo.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3vikkxjmi.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3ohiwesrl.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3emzailed.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3lbbgrkij.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3ilrowwqg.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3fuugagwl.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3arqnohiw.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3iexfbacd.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3qqzlxsrk.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3onikhslq.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ijxcazbo.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3ljugutqi.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3cdbsxjfy.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3hnixsdft.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3ybndsncz.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3cceyhfbl.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3qitbongn.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3ukmzwdov.html


<!-- 参考信息 -->