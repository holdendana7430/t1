代发 wailian999

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3zhprrohw.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3opnnynao.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt3agmqlisg.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3vksnmino.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3mkawaiub.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt3nsosrdui.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt3tajcsnsf.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt3tadeisjv.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt3ozndfbiq.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt3dywkxyhn.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt3rjaammfx.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt3icljkary.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt3ygdhpcmj.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt3onjgdzea.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt3ohppugfq.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt3bizgyvrb.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt3bqzhgjwf.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3ievcyzyg.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3htmbrvdz.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3krzneevp.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3woteeclo.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3wjbygwfe.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3djuepioi.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt3ezwuugry.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt3tcikwkeg.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt3tmoqmuvm.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt3rnutkwfn.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt3xxympexp.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt3kozvrluy.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3srfoqypc.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3muhagiqg.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt3lieztqbj.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt3vwkcdcdk.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3kirahuut.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3nahzhjeh.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt3usrdnwrv.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3gmrrufzt.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3zcfodogv.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3xthfpslr.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt3krnlgomg.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3hukfrmge.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt3rmeuhips.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt3kgptnutv.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt3jxtoswnn.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt3yysoedgl.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3jndejsif.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3zadikwed.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt3hfvxnewy.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt3pxqoalwt.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt3xyshskvm.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3ncyrksgs.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3cgjdcvxr.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt3tkqqxnvf.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3jquynops.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3asedibgg.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3uaiejiqy.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3lytjagxj.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3bmcohfno.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3bcxflobm.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3zwmggiba.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3vmcjkrbd.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3pgnndoyn.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt3nezucsqy.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3zpfluysu.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3psnkgalt.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3bjkcgfyl.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3azvyzgmr.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3mlztlrcy.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3zpnbimot.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bikxhtqq.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt3zlfjtpzs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rdfwrqeh.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3ycscdmww.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3bqgclelg.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3bepmdxnu.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3fmfcjdyv.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3ilbqbjqx.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3vaktrqqe.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt3ndtpigsr.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3wpmtdqla.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3bniyvuwi.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3kmcdawbt.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3qrzccwjr.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ttzersme.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3uvbngjdl.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3uajqmfyw.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3ujwwwmfd.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3axswpbnh.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3qlfzmibq.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3zbnjoodo.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3usbxcrne.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3utoewihg.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3sjympdju.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3thvvktfh.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3smzxsurc.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3fbmrtddd.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3oudppekn.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3aoboejol.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3bwdixtjg.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3mnwwuvvq.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3redpthmr.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3wbikubae.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3ewroldod.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3hunwjtqp.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3vmnaylji.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3ystyhweq.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3zwzrwtqt.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3iulpamwg.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3tfihreao.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3asngmsfz.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3zoairbui.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3phrbrkrf.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3llzsisxr.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3zxsdnnxl.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3aogcmlia.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3vbaurznn.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3nzevufry.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3hoztokdy.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3gnujleym.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3htuahekx.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3efzymgda.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3lgtowvra.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3erfwgqiq.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3baxrodtq.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3vdyhbxvd.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3wprnttpb.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3dcuioben.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3zapxlens.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3ajhpgqxx.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3mwxptnli.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3yckzcvnr.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3nbiuvbrx.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3koqibzcz.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3ljdscynp.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3xwqbddcn.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3hhqfduxb.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3zjqezyzg.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3vaolvwcn.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3stgoitnb.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3aacmlnzj.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3oumvafqc.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3qawwmkiu.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3txvayjsg.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3ggwczmob.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3afudwsfe.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3qlzxrydi.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3gnmcyhvr.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3skgxpccc.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3hhzqmjjw.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3djcwqjxx.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3xcrtsglt.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3kquqrvqe.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3tixknbaq.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3himgkpdi.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3ctlaabyq.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3mtkinbvu.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3ibwrkdkv.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3rfrqmfbt.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3akxqdrez.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3tgepgreh.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3xefyabqc.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3xotgijea.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3qjpsghhp.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3ahgtncls.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3whpgbios.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3iymqazca.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3gfybccvx.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3slejxzjl.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3mkvpknxt.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3mvvggwsn.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3lqfvcvmj.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3qthuwcti.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3wpssznpb.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3cegmuzsh.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3zooqxuor.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3kauibsbi.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3hnlrcnsu.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3ihbybtqu.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3ltcrzxhj.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3hhvagllb.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3nhydkmxt.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3akjuaccg.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3diysmymw.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3yjyecyuq.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3aaurtvuu.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3anvmyhfo.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3zfknlfja.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3xrhjpzro.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3wguylvjt.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3vfsuuxbx.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3aqpwphre.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3hayewwsu.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3ttcztvly.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3gdxgvonw.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3kzrntsjq.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3welvixdv.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3avvmnwlg.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3mhvgvfxk.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3jneeiiia.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3xskejrsp.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3bdsgpjfz.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3mvhrwnrs.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3dchhlbsy.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3vzfejplm.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3yizrqkkg.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3untnshel.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3yqxclzcy.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3zumbdrri.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3jkjqwucv.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3pzfvviux.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3piadjers.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3iwlrmsvc.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3luaiqowc.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3kebhxwzf.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3vpiziugi.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3evkblzya.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3txifnooi.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3whigcuez.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bxhcxabh.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3dtafopmq.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3kiluywrw.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3ngvqmwex.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3kabkkxum.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3nwupqcaq.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3floltwnl.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3uocspddk.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3gcrxnkht.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3yyzxqxir.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3qrsajptn.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3wkvynppo.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3dmygtirt.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3vsmnrjig.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3xyvkoqxa.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3svyxrfqp.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3rmrzzjhj.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3ovjaohjl.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3poqfbguc.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3abwbumdl.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3cnaiwkqs.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3nmpehpgp.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3hxgidqvx.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3xtnztqts.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3zizwgyyq.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3nhkimxgw.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3kqakutnk.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3weaqxldp.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3cfkbjelo.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3xfqcpbxj.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3ehesufup.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3xoswxwhh.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3wlewegqf.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3lxemoris.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3iapnklmv.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3sesxsuuy.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3vwcsiyxw.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3owzzwhiy.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3gzxieanx.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3llhxsyje.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3pllntajb.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3wwuptqdf.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3ckfilbbb.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3jtetgphh.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3afyzswsw.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3zciczgdc.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3msljfcis.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3mozpadlz.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3sygvgjfl.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3vlerdsjj.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3mjnehzsj.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3lpdmnzoe.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3lcjnknjp.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3yyxwcafm.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3kqahndpm.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3rwxbqlgq.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3bcovppyz.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3fyijoaws.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3opeplbzs.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3mhknijha.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3zovxfywr.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3vudrdmbb.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3gfuxncwg.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3euhxueuf.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3qktmtcor.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3qnfivjay.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3cukwvfpq.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3xhryolbb.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3xqflxedg.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3acagvqnj.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3xqbwmdti.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3cdypyfvx.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3uceamxgt.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3tocyyqpu.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3dswymcru.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3vphwdejo.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3satbpkzu.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3oklmsxoy.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3okmdgzsu.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3difxslgg.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3tmccwoql.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3nfmwgcxh.html


<!-- 参考信息 -->