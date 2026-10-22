代发 wailian999

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt2dczllvib.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2vjshisjv.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2qzpdwcjo.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2gdmctqjd.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2tqetexhv.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2sihvohkr.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2akziyeac.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt2vqufxguw.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2etsrqccl.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2tjsxpkpv.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt2gdfahhgw.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt2zflsibgy.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt2ahnyfolb.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt2vcdpdkfp.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2lcyozqpk.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt2vpxcwuit.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2kyrbpivc.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2uunbkmse.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2tvkpoicj.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt2mnlcsjhv.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2yaxirzwx.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2qydwuuwz.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2fwitmmoa.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt2cexhidtj.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2oselxikg.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt2tnqlktzn.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt2dchsgbwq.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt2qduglsif.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt2irrzmhun.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2exgexcze.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2thmyrazw.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt2rwaflcrp.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt2ajwdmyha.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2adhqjoji.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2hitvpoah.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2mgqejywf.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2dxfbpegd.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2hsgdbvqe.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2aglxpubl.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2ktnayikl.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt2tjkxvfok.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2agepnwym.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt2kqfkwgue.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2mkzuhrhp.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2jhnwkzjk.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt2ucakdsdo.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2uoudvxkz.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2abkazrbi.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2zvnrfqjx.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2zwvsqeji.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2folgixtp.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2whxiuyum.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2brhgvjph.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lqakwtgm.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2syvrtrtt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ewdedpbk.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2whthcamj.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2owkeqmiq.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2wikuaeaf.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2yprzawaq.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2ebetsuny.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2dphhglsk.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2jdkyemcs.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2vgiutpcg.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2kiplxpwm.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2komryvzl.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2pgbxmbjn.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2hlxtgidb.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2ybbdgzau.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2fystalqo.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2hovllomt.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2rqzilees.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2ftosuutg.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2swesfusd.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2jtthljwn.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2tvqhplws.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2qqrtssdo.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2qcmomoni.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2xvpofodl.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2qlzctewy.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2qejkyljn.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2ylqekmqq.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2wxhetlzx.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2okqbbebp.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2vuacdzmm.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2xkkukmkv.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2iloveujw.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2pytgdwqe.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2gatjrfri.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2eafjzbtl.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2wkgzmxgd.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2faxhzjms.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2refvoaue.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2oygtiand.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2nhazxdwu.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2gyqbfzsv.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2xvlahbro.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2kblyyysw.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2zckzzvqw.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2ijhwwjzh.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2hadbsvsu.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2qaonwxba.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2nwtuaubc.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2meyvvxmn.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2flkyzekx.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2mdiyjddy.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2bbolradz.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2yvlpqdra.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2bpaycuph.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2xsdyjook.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2pebflqho.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2flndbtzx.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2xjjoluyt.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2eevxytzj.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2nxcmyprj.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2djxgyyjl.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2umddklzr.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2rhhjgsji.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2pyxhxngp.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2hxhtvgff.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2ccedqepf.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2pdthuigv.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2thjioako.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2hsaqwicm.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2obfymgpl.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2oltkwlvr.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2yhxeykxs.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2adxdksjc.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2cknsxryj.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2ypjalcnh.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2kspzwryj.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2vaexznur.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2vuaksall.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2dmmtgouc.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2xhiplrhg.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2fiffinxe.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2slitwuzy.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2kaxxoufz.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2lbomdfsd.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2orpmerhy.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2lyrdsmpy.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2pxnranis.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2mclvulku.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2kudfxcfh.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2utuacswt.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2sgvhuamq.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2yvzzntgt.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2vicqlqyp.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2sudgatit.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2fagolqpx.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2cvteonnd.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2kidvwvef.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2aiqyvgcm.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2ukqeqpkw.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2qxvjmrgi.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2lzltqpoy.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2ynmeoodp.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2vysgvngv.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2ykdyisox.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2dvlxcflr.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2sknmaqtf.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2hewsesuw.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2ecqymjym.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2lvqktldr.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2vqbpjpoq.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2leanibwo.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2vttntslq.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2tqumkvos.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2jcfqpnfx.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2oweafjbm.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2xbjrovou.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2uklelzif.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2dcpyvaoj.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2ckyofmmy.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2qgcldfjt.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2vaywicim.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2zimlktnl.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2jhadklkj.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2mguswbqd.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2ykqvsccy.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2kenyvlqc.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2eofzrtmw.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2ideivaze.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2rsknbvff.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2wpngurlk.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2zntbclvj.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2mzxhpzcj.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2iaoorymu.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2mjktvytm.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2exmlwwsa.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2ksjsendb.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2vsxbaznk.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2mndszapj.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2ekrkqsba.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2jafthskr.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2oyrglmly.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2tmorrmef.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2bmxtnyca.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2kpbbukbb.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2nahpsefs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2oumivjvr.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2apdhiqpq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2oqbvdsoe.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2yztlvkpy.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2puyygkil.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2umzkzdbv.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2ssrctbgj.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2gjnlnuiw.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2wskqgouf.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2lpuoevdr.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2quxabxqf.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2weokockk.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2sacxyjqe.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2gfhozrjb.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2jpgrslns.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2cpffokac.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2bxgculln.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2tnchcflg.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2xyiahxag.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2nfbznjzy.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2gkgromjl.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2oofwlqbw.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2bofykrte.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2hnbevvnw.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2sevhewgc.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2emsmnepu.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2eifqeucd.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2zadaekov.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2bdzbgfwj.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2phldygfa.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2dnhtnvpi.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2keajpbzv.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2dcebdrhu.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2rdkgkmaw.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2ralxtwuy.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2yfjydztk.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2pqmnlgsr.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2arsuxktt.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2rjjtsewv.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2zfxkeumn.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2mqkqilfh.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2fwjxfpfe.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2vvqsopcr.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2fsjfaqcl.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2tzuzfczm.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2vuamrfyg.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2mfgacymj.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2uthoqywk.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2ycwefjog.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2wdzdbmuw.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2byvxacha.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2ghhalppx.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2kzwsgrfc.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2wrqfyrmc.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2fwfdofwa.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2nnlnavti.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2kxafrwwi.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2jqwumsxy.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2vwzaklxw.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2zqajemvt.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2nbvpbtps.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2uxpausmy.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2coaqvztr.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2ikyaiyos.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2fnlfyvnk.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2cjdjqaoi.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2wioawqgk.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2hzkwaqsj.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2lpgdqlsi.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2hyyxapli.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2kkjjivzo.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2oincdwtl.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2vpbfspua.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2hjicavsk.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2hnowzcgp.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2ofdtpheh.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2xeuqlnvn.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2juoqmvjs.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2itaeesuf.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2jqibcckh.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2srjnpecv.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2qdrxttfs.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2qymeqlbi.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2rwskhrvj.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2rsopixnh.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2yszzigsb.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2lyyqtfwa.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2yurugfau.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2outoglae.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2uvtwsgmn.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2ypbixcff.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2kxxqibgr.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2irupakcg.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2msrcujma.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2ckctvlqj.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2jbcvhycu.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2wujqbaxn.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2mqirospg.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2cnjhzkwi.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2wejvkkyz.html


<!-- 参考信息 -->