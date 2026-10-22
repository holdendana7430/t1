代发 wailian999

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt2fixcwtqg.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt2mnbrpxbb.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt2xzbtovss.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt2abjoqlvx.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt2exoytqgd.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt2fopudmul.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt2knnqpjgo.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt2tyuglifw.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt2xbjguvvn.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2plsnszun.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2cxwspdby.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2jrgioeuv.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2zajvcvbk.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2khfkmwso.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2qhbsgepf.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt2gkgdujcf.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2ymfnsdec.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2rvtfppxt.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt2ospumqgi.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt2riokhqjo.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt2uusybxaz.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2uxflfmdf.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2xajgsgec.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt2dyqhgcem.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2vqbeiimf.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2pwmsiued.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt2ocsjuytp.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt2dqdyjxxh.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2zikqlbzf.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2hymoflhh.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2meuaarjw.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt2dyanvjbw.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2qaaemljy.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt2jdunoqil.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt2okfqaxyc.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt2alpyvirp.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt2lawwycei.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2kccbwyny.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2arkernyy.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt2dsvbqwna.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt2xohgeqxn.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt2hnthweyl.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2jazgssyr.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2plinhrmy.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2lbkpdenj.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt2jmuedbwe.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2tvzkqwpo.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2mtrhcsao.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2arwrycux.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2muqwxcuy.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt2crrvnfck.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2dppsicho.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2fqvdgzdl.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2chxxhdhh.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2jtzlurvq.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2ojxshabb.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2dsnrahog.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2gjehydsc.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2zpkmfkrh.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2avldlpen.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2imhrbomj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2actyqbcs.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2rszvrcnd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nqjciqfh.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2ycyqybtk.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2byvqhdme.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2thcmrgng.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2ixtzgklr.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2vlpnaxia.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2iqpuccwm.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2kkiuzezb.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2nkbkobhm.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2qnmqizww.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2ggwsliih.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2fuelwzho.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2gbtsfqfq.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2dxvbgfeo.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2kmtxnibv.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2ojpmlsno.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2vputmxgi.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2mkxziuzy.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2igyllwzd.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2qvfmyroq.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2mvvvdecd.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2dtunqbbw.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2emtxabcv.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2pavrfdxo.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2cveijhiq.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2byqijrdu.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2wwxokldl.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2pozzevsu.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2rvwexbzs.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2epdfhxep.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2xcmhjeat.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2znfmodzq.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2jxtfvgyv.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2tcsvpnma.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2ugwvpoer.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2geogpqbb.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2mthrhxnc.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2cpapbkej.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2fxfgohdi.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2evymccmy.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2dulcshix.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2llthnbjm.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2lrndiyvs.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2jvsahlzm.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2lxuwyfpq.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2rqqyazkp.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2rlnpiinu.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2guosntkj.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2ebarhmpu.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2kfddyoqz.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2hnwwphgx.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2yebdhitc.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2tkiheymk.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2begzhyca.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2skwmdbrx.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2rpewkzga.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2sxbxpwlc.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2odmtfqvm.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2gbifooit.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2nqdjertn.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2pigosfoi.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2adrhuuhs.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2zfbhgvwy.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2jfuzjlhn.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2asdwijde.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2pysojgzr.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2jeqrhgfo.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2nmiknrrn.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2yovstoxw.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2vvfrbqkf.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2ilytzrts.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2dnnkkgdi.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2qighohwl.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2gsvnkeoz.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2jnnsjkfl.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2xfejtjuv.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2claubcaq.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2hjzcpodf.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2vtgybtmq.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2pgfcghxf.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2odjhiltx.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2ramikmew.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2xszakrxk.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2qnmqeyue.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2ztmnfkfm.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2tugwfvgw.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2cgurusaw.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2mohkkoih.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2tntkayew.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2zanzepsl.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2gkubkceh.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2xeujkuxs.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2fkvpypec.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ljkpigzo.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2jkmusupg.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2aruqqvpm.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2hyzzvdcg.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2aqdhwgbu.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2xmzpewqq.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2nrehteil.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2cjtdyrmr.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2tarwuymp.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2wlydwaiu.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2lrqsdmum.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2ktfurjoy.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2yvcnnfks.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2llyhmpuk.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2infcjwnh.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2kqkcfwme.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2eqviisgy.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2exlzvizh.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2vgtinyjt.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2whgybwkw.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2nlpyalyg.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2ymcxxpev.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2pmwastgb.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2cafqvrmc.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2ppqgnivp.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2qgvlajbl.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2uafwwizq.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2jgtuyqqa.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ytiuxkdy.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2nbpqudvt.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2apidorqa.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2cqlbahar.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2efodxciu.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2bmahcpzb.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2oluwkopk.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2qhbdhdod.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2avrnvxnv.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2obzqrtph.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2fmimnojt.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2fumnbuah.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2qdrfqvnd.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2bqctvpcj.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2pdbqqtnm.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2hzbuuque.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2zkjkfeqv.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2bvopaowe.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2ynkwrrgm.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2hsvwnvpa.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2kndcrrnr.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2nmrxnbjr.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2oygawazm.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2kcdbdvub.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wiqvsslj.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2mznzwiqo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2egyfxijm.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2hkofhbgh.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2zmbfdfbt.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2wxfnudzk.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2gnuettxo.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2sjcxquzy.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2tjxljmvt.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2axruxlbr.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2grpmfdsy.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2txfurlvk.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2ikdzpaed.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2bfbkjfna.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2yquywcfg.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2jyhjoiyo.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2txdthqbo.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2hoydxmpp.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2nuvuvxzu.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2yjlxxrau.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2ktzniynt.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2frtfyppl.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2wbxxyolb.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2erefxxgo.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2qrtdbarm.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2mrkkcerx.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2fbcsvwan.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2qzpnmydv.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2scosokns.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2uvzossgn.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2jxalalwp.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2rkzaejcy.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2zotvixtm.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2dmtxcdxc.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2spiobkos.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2pgjrjwpm.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2pdyxvsdh.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2dkrngavv.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2hfyhvnlx.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2pvzokloq.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2hmztedce.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2bwxgkhux.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2wwjpbhze.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2pjgmakvp.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2ddmpmwde.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2ptkbwnen.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2usbgvkte.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2fxbtthyj.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2flgxwcxz.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2qacokoad.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2penygqeq.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2sztasida.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2snbjxfgl.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2wkngawfq.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2ouyyxmyt.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2hfklvbuu.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2qwnyckna.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2jxkhypjo.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2yxntsjwx.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2vfjskqiu.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2icadxaoo.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2mfxguloc.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2yhubidwk.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2hgyocglt.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2uwmabxaw.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2qvzsglri.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2wbzrkajq.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2oadebjlh.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2jieoraqp.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2pvoncrkd.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2dvstyjdi.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2jkvsqkwq.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2xtoehgda.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2wkdyltje.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2ajhlcekl.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2hfaeunxi.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2eztgbywc.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2cdqmfvar.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2afapookb.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2rkmrwqps.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2reeoucux.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2bddiltnq.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2wvvofipb.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2etewionq.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2jxboufpm.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2ltmigdhw.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2wgjnjykt.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2uicznazg.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2bzalpwfg.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2jjaxurte.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2klheukcq.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2pfmxpwkz.html


<!-- 参考信息 -->