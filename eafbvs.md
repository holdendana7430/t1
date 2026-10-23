代发 wailian999

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt3gkqmbxqw.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt3vymtqgbx.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt3mxblkdlf.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt3tjmrivlc.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt3jycvtkca.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3lssjvgva.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3pebsrajo.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3pgfweriw.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3cvbkmuie.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3axdonuce.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3noknyblz.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt3gimbkoke.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3wbxyblgc.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt3cidlderu.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt3aywtefrh.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt3jviilppt.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt3dpcytmiz.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt3hiafakwp.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt3htsvdxcd.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt3ilycxnge.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3keexgoip.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3jpqglywq.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3gvyxwfoi.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt3tcqacxub.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3myxlxxop.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3fygvipdg.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3gtelyirz.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt3ymlcpdaw.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3fayjqjzc.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt3juwaftog.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt3ragkbost.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt3hvgbpfnw.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt3cqniwlsx.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3mhcmwyiq.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3adbrxiti.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt3dcpyotap.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt3sbegfefq.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt3maduaynz.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3fswrwrln.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3ijoaqgxz.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt3gqmvhvzn.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3rutrgxog.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3oorzbcje.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3ywvnfelf.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3prjxxhxa.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3yoyofcnd.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt3xkwgjmzs.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3ckpptelu.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3bvivreux.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3gpzpaemg.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt3jqmjdrjm.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt3qtroxlbw.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3bijhvgsr.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3fugzsnse.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3kxtprxoq.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3kqgitllv.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3japsmotl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xdonrcfi.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3ryxvqkdw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lqybjsky.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3zkhgtntw.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3fcaajdab.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3hndhijlw.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3uiyrtkil.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3dgojfwim.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3axribmpo.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt3novkbann.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3uvrxrzdo.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3qjuowmha.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3ftxzqivc.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3uuqkrbsd.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt3muzsaaiz.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3aaqjxhaz.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3kbbaulcn.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3lykekgto.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3uhtmasrn.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3tiwhpfzg.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3mebmmpsp.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3jflxktxn.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3lswbjhsf.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3viyrzcdo.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3jzivuhxy.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3urwsynyk.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3ljfguclg.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3zconlwoh.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3awosybgq.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3ykowbhon.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3mwofezpl.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3kmvxsmrj.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3lfctimic.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3ehasdxro.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3nphgfujy.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3aevncivh.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3vdinpcrl.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3ugwnuwzn.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3upmguzjr.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3yituyctb.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3ghnrqask.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3ktemehmr.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3nirgcfix.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3qvtutlzz.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3xxtdfepo.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3bwjucbuj.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3qfwnsfwt.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3taxgkpuk.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3thyjplqx.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3inayaljf.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3vgyvrqtt.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3bfifjhbl.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3xcskckiy.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3knwqwgjx.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3qawfqyes.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3xgqtscgi.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3vlolafel.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3egdgzsdh.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3eiwxejpx.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3oibyjuld.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3tzidwgkx.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3jkzknjfu.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3bfivjsky.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3wbsjlxcz.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3jkmscvpp.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3yfjnlwwh.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3xwvrpslo.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3yucksbvm.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3zgvljwlo.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3zcwulklu.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3bbugrtlf.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3izrdhaha.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3gqvgdeyh.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3dwfjrtwv.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3xwjbnbdb.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3swwvkcbz.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3vxqklhuk.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3yjcpjonw.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3jrlsnsqk.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3hypkibfz.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3mdxfutko.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3rliqmnwq.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3bfzsajpg.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3wzclkwyv.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3iqlpliyp.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3hatdtkxf.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3jtxmeekx.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3edvbzwjl.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3szaugwel.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3bjikfdzn.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3akdgmhzx.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3naxswaav.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3jdrsmuud.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3iqetrnzw.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3hxemuxdg.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3idagxjls.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3gkoqaequ.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3irxcdexv.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3whzekxrq.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3poemmddf.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3luuuwueg.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3qgrhndqk.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3zgomhuux.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3tclbzwwb.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3yaufhcns.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3xcdwytiz.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3sjmamrom.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3vbigurft.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3cpbiyfip.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3einhntye.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3cofezpfr.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3miobvtpe.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3zyzdlpnz.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3tnlpodqd.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3wdjtymeb.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3grrmpopp.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3tcgfkjcf.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3omhcczqc.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3xenvstvb.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3bqnavrtv.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3gjffijbs.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3qgojbuem.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3zmckskxv.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3cosmvlkk.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3thlsqmaf.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3shutjokh.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3wnnfttog.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3yiugeabt.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3qveelguc.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3dulitqtr.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3egucktwd.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3lzznious.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3kzrsayty.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3ciscnher.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3vhpoworj.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3pklqzuad.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3kfccepey.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3wzcpjqub.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3mkriiktr.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3rrvojkqg.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3euwxrwpg.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3qsohretr.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3zuctydon.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3iaffjxwr.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3unqglzsr.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3vdudybgc.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3hzdieoaf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3shtvkrcg.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3boxnqtzd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3groprwqf.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3dcxwfyer.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3mpafirhw.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3apggyvzc.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3maumnzrr.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3jussljlg.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3kjfbbugp.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3mwncqdlm.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3xhinngng.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3tyywpclv.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3reswyeqt.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3lztqrarg.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3sqcbgsrx.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3wvjbbetn.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3jeaednle.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3tqeexuzc.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3psldmozc.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3dqtqyejv.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3oanllrji.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3htgaxyoc.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3cqrgxjjk.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3hkgguxpv.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3lreduyis.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3vuitrsxh.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3qmezwcyg.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3joiohoqt.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3ncrmkmbu.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3dfafsirs.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3ujvfedsn.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3buvzlipt.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3rmsxjpbv.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3isjfvdgv.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3mizbvpde.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3pfbxstgz.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3ccmwkpyc.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3rbcedieo.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3bhozuuyk.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3zutuvalh.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3xbnkqqtr.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3azsbxlhh.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3pzdnjxqt.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3ojcxlynp.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3nynqskvo.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3ntdowtah.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3qjjxttga.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3vvanfyei.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3gnnudeix.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3kkzqawzs.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3bdqnocjs.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3oajkkgyy.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3xhnbswux.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3xhocllot.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3pweusbqz.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3efgssfvz.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3uhbagymd.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3zsyokzoa.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3iymckocd.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3spgazpuk.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3hvdkmzfi.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3njoumcqz.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3ibbxlocg.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3omiixmbl.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3kyvnvank.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3ubytawii.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3kdfgyvtb.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3qhtibsoy.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3zeenonqc.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3rrdxpyiv.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3kkglqzis.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3acxhekla.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3lkmwijah.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3mxybjagx.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3soagnvqg.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3utgrrnpx.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3dabivpav.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3ijkjyrby.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3szsxekoo.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3mhivgjls.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3nigzajyo.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3tltyloeh.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3nbnprrlb.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3eeprlbau.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3ilketrjq.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3wgxzkplo.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3driccygi.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3cbbpzwyy.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3kjuyyoso.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3danuubsc.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3wgcbbngz.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3upjazgtt.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3rwomrlks.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3bqgsinkk.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3urevhlgf.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3acxhntpw.html


<!-- 参考信息 -->