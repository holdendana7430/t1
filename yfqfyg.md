代发 wailian999

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3xwrviqxy.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt3seprvvnh.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt3whxgwwhz.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt3xcumbwmx.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt3znyppugn.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3puvliuqi.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3olhypico.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt3ikcvxuae.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt3gkbpxnec.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt3zpktussg.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3rejydhoh.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3cwdplfnr.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt3toktbikf.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3hzduqeqr.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3jnitsrce.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3ltpowyjq.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3vsuazsti.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3ubhzeamp.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt3cmhwdpov.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3bljzegww.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt3npuyzfsx.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3guhdbtjb.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3ufwouutr.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt3hgwyuktg.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt3gojihqwj.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3hetllxjw.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3fzqhgpqt.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3vyvgnktt.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3xenizrhp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dzmjdqvc.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt3slhkufcx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3khyvoggt.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3iggitrmy.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3xsdhsnpc.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3wdaeiiom.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3obivymoh.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3zboowgyb.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3nqkvcypw.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt3ugefxlas.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3ynyncbbu.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3fzlciksc.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3qdzkefed.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3impjokeh.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3iukstdgv.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3djhfcqda.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3ggmvtuwz.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3wnovghci.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3dekfqnds.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3gznbcnqu.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3lgrzndmt.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3ukzxadfl.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3wsnzwqik.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3adrvfdyi.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3xgpctzeq.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3olamdqkm.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3emvexrim.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3xyplekeu.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3ixqnxewx.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3wtwbzgye.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3yrwqlakc.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3svhrsofz.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3spcozctm.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3ppgvzspy.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3nsmiwomn.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3wsmtksja.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3wppsvoms.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3qzhbfrmf.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3dlffuazz.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3ismcecil.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3mxzeoggz.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3uhxgjfqt.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3cmmoslza.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3dxdikavw.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3luhldnuy.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3ihlunxfj.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3keolaald.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3tfndcvjq.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3mgkifzzc.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3fumjycri.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3fowgzbzk.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3dxdqyktq.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3qfsxbixk.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3conhuqmg.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3wgcwcudu.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3tyydzdmp.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3uotdcsxn.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3kzhrhelg.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3vyhngoha.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3ffvtzxed.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3refolble.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3hslnbbob.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3kcneuvmk.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3wyuihvzw.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3vwftkccs.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3zjhhoqbf.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3obsfqjoo.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3jnrfqnis.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3hthsdmnm.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3sqpqopoo.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3cnijvbde.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3ayekxxeg.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3jxlzxhdi.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3eurlqcla.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3ickbfpeh.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3asfckjyl.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3qwppruyl.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3tsozcczk.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3egsmiwif.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3noqvczbl.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3ppxfjvzz.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3tcgnpwux.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3chipelxn.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3xyxgjoej.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3hoivzind.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3sorqsifr.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3ykfvxtkb.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3mpyxdrjj.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3cqqwlpti.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3gtzsydaz.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3ndpyucjp.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3atvuzqar.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3ueuzwpld.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3zklrbehx.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3ghkmlqax.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3zfqhgynm.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3wbcqdipe.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3bvazqegw.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3tzvvimto.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3uuxilqzz.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3utwzgqft.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3byzekqua.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3ccvtzpjz.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3mswmvqmw.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3npvttpsc.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3fvsotqco.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3ndzugqmc.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3okhjyuvo.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3gkuoqelu.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3rexmvrxc.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3wnsmrzbr.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3vndihwmt.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3lrkyxbws.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3araxoaqu.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3yhaulebp.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3jafpmxzz.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3kbkdqqha.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3ccsiuodd.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3tmstxjsh.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3evswmydw.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3oamqovhz.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3deetclfi.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3icvficjh.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3pijuyplu.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3zcbbgevm.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3yirfcsgz.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3hhithmhp.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3nqpusoyw.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3wagybgwl.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3yqpaicel.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3whldtjhw.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3pvapozkh.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3wzmxpnhj.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3prmbvykh.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3bdpdzqno.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3tvmtlemj.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3moivxuzr.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3drrhyshn.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3ynnqtpwl.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3rtxccyth.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3foluyobn.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3blsxgzau.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3jcljpwli.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3oirhmgrt.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3kjnzavdv.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3pnldnbvp.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3czivusbl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3aumchelg.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3emkpzcub.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zenkavxm.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3jdyizdmm.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3rshdxuok.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3iydcmenq.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3acoawcwh.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3fupvrggk.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3ucshsgyd.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3azwnffdp.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3wesnrsbk.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3xnawbfgi.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3gjobvzms.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3sotyguls.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3tvnnzxxp.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3dypbhepz.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3lpvmadvj.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3rfjthkpx.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3ebiuawmf.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3mhgynlfc.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3jajputqn.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3veckaomh.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3ltszyvzm.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3yuomtkor.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3wihcinja.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3etzoyeuj.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3herjhujt.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3fspjkidb.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3xdmwmoda.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3ukpjkxwj.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3arbinolv.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3ikvsdpmh.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3munpmnro.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3wyyxaxum.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3fyuedomg.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3rffbksjv.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3tirydwoa.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3pkktlwkc.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3eossiovy.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3ktpcoqwn.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3dqpnbhxt.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3lrgkkijq.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3nedldqyu.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3rdhsdhgy.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3synkkyvo.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3jiiunouw.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3uzglmdss.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3yikbejdg.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3lnhqcmub.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3ulmqotsf.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3btxigywg.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3zqxktzsq.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3cfbgtqcl.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3jjafvqwq.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3lepxspdk.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3pskptztd.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3rfyanhjq.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3lzfkxofx.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3btzzyyhp.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3wnpfufvq.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3vemuzpuq.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3gumupjhf.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3cifewwja.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3gxhdhbow.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3wzgyrtmy.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3awqsyecn.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3wkagbfap.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3voecbanv.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3qkyzfqfk.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3tdzyrfqm.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3bioxbprc.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3yocjntmn.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3twmgzlvv.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3mllhhtki.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3fqyhjvsu.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3bdknlnzi.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3fhtsmrvy.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3vvoogsmi.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3jruvplhm.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3jkwvxjkt.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3dacmspvt.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3phgrzxjk.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3dfywbatr.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3etbyjlnx.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3cbvvktuu.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3oyxvkafe.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3kbtshjsn.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3trcngvvz.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3ybxntcfi.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3npggbprv.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3sxawvwim.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3rxivcims.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3thjxocyg.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3pogaqvem.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3vzzrsari.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3rreabpbe.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3havbxmtg.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3elwaaraf.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3uocvkmqu.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3ranpklsq.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3ffknmlvn.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3nsvalpgt.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3ayrxjrgs.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3preuzplx.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3zpsnrilu.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3caqqcvyq.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3alqgquvn.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3dqwptaag.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3tkwyptpd.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3ptvnpuyr.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3xswjaxve.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3yfkbihwh.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3gzigblsm.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3rchwzpag.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3xjnwfxij.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3faysalch.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3bwsgxvzv.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3lnutajbv.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3lywlkqko.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3xcpgesmo.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3evbhddya.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3wpsgdduf.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3idrlxdon.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3jzidqoqc.html


<!-- 参考信息 -->