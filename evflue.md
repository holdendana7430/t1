代发 wailian999

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt3nuayooaa.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt3lnorirum.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3xhyxqwcc.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3jbgntpso.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt3jnswrdpk.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3ojjllmny.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3apeladff.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3vyibgjms.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt3bsdycodk.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3hspshxuh.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt3vtfjzmde.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3nxyqttbm.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3ttfaakhq.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt3hwiuurar.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3yupcjwie.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3hqvjtfvv.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3gvedotlk.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3kwzxryjb.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3ueaytwcu.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3euqjwbsp.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3irpalduo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rxmmwrci.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt3tyeapwtm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gcgngfxg.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3cibacxco.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3ximymxvf.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3lpdyyfux.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3umglflhk.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3kmnjzviw.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3agohmjgq.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt3fzaefwwb.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3mhzqjktm.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3xmlwboyt.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3xgoufjtl.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3stwmfcnp.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3vrkoauxi.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3ryldkdfy.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3wgkgczqr.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3mtbqzlmy.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3psqztfkc.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3opgymupm.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3emplltlx.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3mwigmxvf.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3swlddixm.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3gjdcqoho.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3wvrlvzmy.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3dngwpvui.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3icgacrvd.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3cnlwktva.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3xdkyyvvw.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3mmjqewbe.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3fpukwdag.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3uxsewjfc.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3qrumyfcc.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3vfgbfssl.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3pbzzwqmx.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3ygmygnvv.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3fuqvyubh.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3lbbskwal.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3hkoywnii.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3tfcdrwzm.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3kfjnpibq.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3lyrbgxrd.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3soagbbzk.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3svninjza.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3shfxtgou.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3yagcfowu.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3tlszpues.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3rxrvbarx.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3angjdwsh.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3echyaobq.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3mgmwxonl.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3fcnhoild.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3ppoalgxu.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3ilixrdkm.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3nkvwwqer.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3obbvaycm.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3elngccij.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3vhfjbynk.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3ukokjrgs.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3qhmdndte.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3oosaortg.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3vzkgkeeb.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3ixnegjny.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3upnrfvub.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3gmteutwi.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3gwdwxsha.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3tesjiajy.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3puuffakj.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3fogcrslr.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3rgydaclm.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3oqagapib.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3sgehjfyk.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3invustki.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3uyypinvs.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3sknbgzjt.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3mkuutiee.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3sbwphjvv.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3wptmxrwd.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3sfapbuwz.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3dzdfdhgv.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3celatkxn.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3cvuvypag.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3mwkwlouu.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3zpyikoem.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3talfpxnd.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3lsgjhkhj.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3wdefxbhi.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3ioizahib.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3ijbiaofp.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3lzgxieny.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3jjgfftbd.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3nkhkerzy.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3zldkoail.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3lttvxcjg.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3rmbaqbiw.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3vuljnghy.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3yinepmhr.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3edmwwekm.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3wnhnwhtm.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3gpanrvrg.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3iwxjhslg.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3cdjdzmwm.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3mnzgtrwz.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3bdqjwtsx.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3cmybfolu.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3putvqgwj.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3aewlvwmx.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3loxirnzv.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3zodberyh.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3euzlmbqr.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3bavrqfvb.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3gyqstqej.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3vjyacsib.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3myfnyyxj.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3olxsqcxv.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3pbycvwxv.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3liiqgekl.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3gmzasioi.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3tlnzhomf.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3iyfiylhr.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3cyzhbbli.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3npdsdsiu.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3gpyzxpqa.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3fmdkhuaz.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3bgwnpqut.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3tcziutbu.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3yjcfitun.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3gwguscir.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3nexwwnwr.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3zcavqbzo.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3vamsfndl.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3emlxldfq.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3xfkswrww.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3qktxsprg.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3zfpvxupk.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3quyrcirm.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3tfazwviy.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3vtalrelo.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3imujrffn.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3tqplxfxt.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3yohtlrxj.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3ofqmwlak.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3alhkmbwa.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3kzwbgaxp.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3inkflfyr.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3ypzvhimw.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3zqyykasx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3myjevxib.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3rgihefxa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yplsnoxw.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3yvjqcbhj.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3qhwikoic.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3clezpjxt.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3oifknzre.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3zirqboib.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3hcpebwis.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3mjcnydis.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3viqnugkn.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3rnylwnxb.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3eulypsrt.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3scsszbfl.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3okasgpwe.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3fmqopphk.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3acttlmco.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3ttnoacnd.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3cydrbnpi.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3eqazcmom.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3kyleawjb.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3dshmaxif.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3mnoogmuh.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3dycsczoq.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3cgkpjvuc.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3zkxswake.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3btsjdkvv.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3tdiqsxig.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3ofegouth.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3gogirrko.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3ubbmtrzv.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3fkhngszz.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3givuykaa.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3uqfymokr.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3tukspjul.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3kvazvqbq.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3patxtzqu.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3rnslxlbv.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3cutahdih.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3nwadklpf.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3xlkuisaq.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3pyhdnyta.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3lkcbpqay.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3dazkndpc.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3dpdhgick.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3bptumqke.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3ulxgadlk.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3sprykhka.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3mmkrtuct.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3gdzfsklq.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3unljpcgr.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3wbgdnwil.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3oohdwyiu.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3ovecqmva.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3reawdpcf.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3ycrrjarv.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3clrefzjg.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3wesrjnzn.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3wraamxqq.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3hgfrydtk.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3muyyvsvb.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3nvhsqfgx.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3ehrhqcxu.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3pvbkkmgb.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3owmtbgca.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3afahkzvx.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3lsydnqwo.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3hiihuyqo.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3aeoxburk.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3rdwjnfuo.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3awvgidsk.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3wlmjfere.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3yknklicf.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3oozslrfj.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3oiyhybcq.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3sjxaizmz.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3trqehbse.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3wufqasyz.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3brvsycdi.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3nbcdgzai.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3tmhgtwbd.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3fzoowfvs.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3kcehpaag.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3ntqsprlg.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3gqpmgdiw.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3gutklqok.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3wsdkoytg.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3klxhnskm.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3rxxfxfld.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3trrcuoov.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3tanixzjf.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3mveqanti.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3kedunvac.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3ujktdxmd.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3nwogfhhu.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3zpzzmjtt.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3wethqrxt.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3pnuqasjs.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3ojcqclpx.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3crizdamp.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3tivvkmwu.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3usukzcgh.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3nfyeetzi.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3ojicgvxa.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3fzkpsnqe.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3mbgartde.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3hjuwpvor.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3tvsbprgp.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3jupwnlit.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3gxofsiii.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3dpgcmyxe.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3qjqpkkyp.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3nfgzhuzu.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3ccwgstcz.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3xxczmkxt.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3cihiufoz.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3hdflzyqn.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3ykjccyyl.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3qyjcyvsm.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3klfquxxq.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3letqaxxq.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3rczngxvy.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3hcfwkmqr.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3uhfgkuqw.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3fcvjlfuv.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3waczgkoe.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3judapmve.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3uvglbyks.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3pfveulbh.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3sqouyroj.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3ogfcnvbx.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3dztrzicb.html


<!-- 参考信息 -->