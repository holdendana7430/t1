代发 wailian999

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt2rqcqmyut.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt2yhtjsbcp.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2lxjffipx.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt2wcfuisjh.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2djykhfnx.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2vxewjxzr.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2wfkvtwcc.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt2ndkyzafl.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2rgxiqvpj.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2pfeormyo.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2dfummegu.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt2daicbbrc.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2cqvdlrpe.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt2jvknahci.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt2lbesnqzj.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt2ufddpfrf.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt2zadoouae.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2jinywukt.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2sxbesmkp.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2yuzmpmmd.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt2frzgmdbz.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt2gyhjtbbr.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2gokdiraz.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2gbuolwwr.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt2tdgzqqao.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2uoyuiqwc.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2lgpqcdwg.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2ehulbnaf.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2dwwfkaog.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2xlpjjtue.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt2bpiekvgu.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2raplwaek.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2hjbfznug.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt2vrunuwqp.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2eiteavfu.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2desopctj.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2mwonizev.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2lrtfxhmi.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2myxgpyin.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2nvmolahc.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2dgmkhsoa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2sycqyurl.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2zliybwks.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zlmgsldf.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2fjdmcxsm.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2kwwbfcnq.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2famhltyq.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2mtjftfqx.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2fcibpgbu.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2arpeedng.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2zcbwxzjs.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2josmnqta.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2sxddwrso.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2mcsvzerj.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2krnrqayh.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2haeqymil.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2egdpvxaw.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2fzdacwen.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2otrgvscz.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2puzcjxaw.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2xdhzlizc.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2hvdmwhxl.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2dxhemwak.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2smbmyxmv.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2kwtzkwkc.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2hlmqlsfj.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2leitxokm.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2zkktfnwg.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2ydwhkqtt.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2rwodepoc.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2tbyiiacb.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2umwyqwfa.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2ifetfiav.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2kooypwow.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2uidousnq.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2vgjweqeb.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2iweusqyu.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2ckwgoqsp.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2iarfbahv.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2khuguhji.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2xgjousfj.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2srxolflv.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2ipxercez.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2jiknxahh.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2nmzlmogt.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2nucqdxgh.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2rgkndzio.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2aaxnvghd.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2tcrvcuzb.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2ruhofbcp.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2rovpwloo.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2lfdxsrtr.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2eveziuhr.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2owbhkchb.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2gqleibiu.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2hcztxesk.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2dyinnenf.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2wedbvusx.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2vllvlemn.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2wlimncmd.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2jbtzcwen.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2pqchjzfd.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2mlclmcoe.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2ncrdaxbe.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2bucbwfjl.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2vrctxqqj.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2zcvwerbq.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2ykorxiwx.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2trmpwlkz.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2vaucbtbc.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2iicysrcv.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2pyvtfkwr.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2burdkuqs.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2vdcvkxys.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2ctsnkleh.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2iiaeupva.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2zeezlmhn.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2sizljjfc.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2ozunztpe.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2ysfsihab.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2smraxurn.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2rxwjdgjj.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2hrzaledj.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2jtcnqnyy.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2deuclqpx.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2zxrawtmx.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2qxhwulta.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2thusadqe.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2ffqnjuhd.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2nmxipyok.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2gfnciihv.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2wcwsckwu.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2eqzfbayi.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2prqrybmf.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2mppxpfuf.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2owbuwmwy.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2dmiquimb.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2qzmsfrzj.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2xvjcubvc.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2ijtvvjpg.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2dwntvwox.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2wukwfvyz.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2dpikzaus.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2xiwwsejn.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2meangumy.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2qxleaysj.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2utftxoqp.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2gqettaxh.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2imacmcds.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2lgmuqtct.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2lnloxyyf.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2mgpeoypp.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2zxwoqnpv.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2ionkpdnk.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2qktvkayj.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2grjccwjw.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2xfcbxlld.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2oqkpfsgn.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2sbblgivo.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2zspisefd.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2nsomwngq.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2jkhbssrl.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2bemvccjv.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2dblxdznn.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2gutensno.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2yphtxfsx.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2pqdfysrt.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2aknnjgav.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2xasoutgz.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2qhlyqueu.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2hejggwyt.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2jzbcrrzb.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2jyksjwoe.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2jvvbqtbb.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2ozvbelas.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2flbiooek.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2nwujrlzi.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2kuxagevc.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2zxxuqhbl.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2ytqvakzz.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2vycpyrbd.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2kasqhcvm.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2udtecaic.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2pzcitkjs.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2dgkmuvtz.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2wkiluzya.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2jydrheke.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2neilpkqn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2viinajlf.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2czviaybz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pxzowdsw.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2vcjzqsnl.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2lduvnujj.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2ubikjgug.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2lgipfdxt.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2frwjenps.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2zrxsclfc.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2dokkypns.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2yrujprfw.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2ktbprohw.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2gqspjukl.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2cseklekg.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2vsdnyjqp.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2kzrakzmp.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2hgsmbtfu.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2yktjpidw.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2vnalmsmd.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2zsvkexhx.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2uhlbxogj.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2dgvtxyaw.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2nhnqahnn.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2whgwzmhh.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2kdcaxcip.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2tvtqjioo.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2stzndkaz.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2doadtprd.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2fuqitrvn.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2vqxblndt.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2oimrmzks.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2nbqgmxgs.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2obqklbsc.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2gonrmvti.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2qcdgcadv.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2fauqgshb.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2fsztlbfp.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2odjmdfez.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2peqtilwg.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2emzfjdbz.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2dkdfvnph.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2rkuemale.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2adkydkrl.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2rjrkpkys.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2jufxihzi.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2wgrmggjf.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2bloxfwgq.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2insdlcdc.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2ofnfddnf.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2gynoukbu.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2tnziuuba.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2gvnlzahm.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2nfshrbvt.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2bklehlwb.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2phkwblfu.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2vikmwdpu.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2ujaxmbrl.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2xwsopyjh.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2uoslqpep.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2gkojzyum.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2hklsppwv.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2yazlalgc.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2ynqtxelh.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2zziziwzb.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2mbfjjcfq.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2lrusguqc.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2yxnwqnrv.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2mxzefpnu.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2eblvrurl.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2ymhwbqgv.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2wrrznybu.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2onskwmjj.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2rcnrbwmj.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2rasilady.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2zycvotyt.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2znkgmoot.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2psmdijjh.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2zavmybvj.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2vdnczqru.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2ntkznrbo.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2hputsdav.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2vthxxstz.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2tdakmzmh.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2btpzvinb.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2izszxjiv.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2enpfodox.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2uxqmwmvc.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2prlrbmel.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2yskqjobm.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2kvsacqiz.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2pyiyzvpd.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2oqtmzioi.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2sreereoa.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2vfhcvgnf.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2cxgwcivc.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2zrzdacbn.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2atdqppbu.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2kszsenau.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2mfaroecy.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2iermwdho.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2fuvaweyc.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2dpjhhgqb.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2lugqmreq.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2qmixzful.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2bnxhaugb.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2lhwqyqeq.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2tjfvqqle.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2zilozlsf.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2wuximegf.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2kwmgfuvf.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2uovzudfe.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2ofbzcgcn.html


<!-- 参考信息 -->