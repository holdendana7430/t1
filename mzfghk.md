代发 wailian999

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2drqrvfnk.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt2rrblssuh.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt2kcklytjs.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt2cqivdwsn.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt2hssskcbz.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2vfyscyct.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2yinwjoge.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2suuprlmg.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt2timjszyv.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2mdwtrnlt.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2jzkkapnp.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2pawaxsur.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2fpbjcbpd.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt2nszuekwe.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2xuzknfgl.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2vnriyhig.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt2htqbivju.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2lxnqjomq.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt2vfsintqm.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2gqatvvxv.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2tgjcvjlx.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt2bpzlgssz.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2efaawjlr.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt2ozjqyzno.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2cznovrwt.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2nkcauyvw.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2hrjxqfjq.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2xxfjreps.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2ddufojyt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2sruduqzo.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2otyeujlk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ixyvtovl.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2coihagar.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2snaczbhm.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2hopgzmiq.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2vojfgbda.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2nzwlgyln.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2ofjfvwjt.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2culeetlf.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2nzigffir.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2mctkxkda.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2wuuqjode.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2jjzucayj.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2kvozxaha.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2chqumygf.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2ovsaizqh.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2uazmujwo.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2sghtetro.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2oamnaadl.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2gahtlubi.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2mqpowdqe.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2qflnwofn.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ybkzimhl.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2jifqwjlk.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2otmzlivl.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2mqfagoga.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2jdahmqbs.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2ymeorljc.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2zzkhbvkc.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2rshaqymj.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2expozsll.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2xmlteujq.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2ryjscqwt.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2pkdzwijx.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2xnpjmhks.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2opfqdbrs.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2afluadfz.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2woszdxbs.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2ujokrahb.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2qlvycthf.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2vmcrqcon.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2nwvtomkw.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2jcqbshrz.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2pejypybw.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2nwbypael.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2tdzdurde.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2kxxtzpdc.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2zavvwfiu.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2cexpuqok.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ecippjca.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2kayxewkp.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2gzejcedn.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2hjgexxef.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2gbmvobyi.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2phehbtam.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2rbgatoyc.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2mkmnbrqo.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2yjqztxvh.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2mzyvfdip.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2alpzdzrx.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2brifjfin.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2cgvzhpxy.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2wkvlobuz.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2jurvqcyx.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2lteetalt.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2jrzpnkee.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2yxppznbh.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2iwspotdl.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2zhkigwsi.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2rldpvedy.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2jrnjkrhy.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2dptzoivu.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2xhkyqhfe.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2leuutvee.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2mjothcxl.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2tduejmtk.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2hqbnqeta.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2gglobcjn.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2nyerehmv.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2ygcvryxi.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2fcwndamy.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2zehxbpce.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2wkgpjmaw.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2wqvpqtsa.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2negdizrq.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2wvdayukg.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2iwvvtnri.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2osbobvll.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2eqldlper.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2hiaylsjc.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2mqfudawr.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2hraulglw.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2xhqexvwf.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2qzezvuca.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ledrgazq.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2nfgptphz.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2cbdimprr.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2cmwhfoyj.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2rvgjfkch.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2jycodoqo.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2voujetfa.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2agpgbuwp.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2jhbuilss.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2qbbalyxo.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2bdjnlvxc.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2ehmnluyk.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2sgzjnkmy.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2gkktradk.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2wprbcmgc.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2vnkdtwpg.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2gyovtseg.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2zfsvcwia.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2smbycfjj.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2qedluknv.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2cknvpzuo.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2nomyohdu.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2nxuwfrsh.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2ultasbgc.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2croddbgz.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2hiigccqq.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2gucjtrfv.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2rxnahjxe.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2iajscnic.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2cqcjjsce.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2sduysfkv.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2quozeklt.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2kbafzumd.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2rrvuakar.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2rwttuurb.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2quzqmycv.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2ynalgvqx.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2qvvkvptt.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2vzsbesei.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2wcutcdke.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2qltphuoz.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2ucdkvapj.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2jqwzgvfg.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2zuethakk.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2kakuabwb.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2pmssjkok.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2cfrnogqo.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2rwedswch.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2tnnbuubu.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2rbyuzhkf.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2nxbwjmck.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2bcyltwnd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xfbogdzx.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2sbhfadaf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tzlhpneb.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2fbcpwsou.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2fnsgbibf.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2fcnyycfx.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2heirftrd.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2tjfqxvgp.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2llnypdhv.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2olgqdcbn.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2yvgjgcpx.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2kphjjqdl.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2xbvxpmwe.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2siuyadqy.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2opkndqkl.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2iakkcreq.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2ixkxjmhk.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2xeuzqnlg.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2mkhgalej.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2hjwyjwzq.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2vdnyihld.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2dyqarfjx.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2guktjogb.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2zdpxfprh.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2mvzvhlrd.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2zjmosnci.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2fymnembw.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2wqgfrewp.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2emqzfhnh.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2etskwxqa.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2mtatqhem.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2cwmidywl.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2kusarcat.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2owpckrtj.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2lvlxpojr.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2ckijvgpo.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2czedrsse.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2sbvpelrr.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2qrccaxzu.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2thbykkol.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2yxjbtccl.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2nwzauvrx.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2nxkmfyyr.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2okhucgjr.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2ojkhxgpd.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2onbgarpp.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2jjugpxqr.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2foubqdak.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2wbcfrhhu.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2xukuczvc.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2uxxgemcm.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2kicpzerf.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2ktzdnbdx.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2nogcbirq.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2bpmbjywk.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2ebcleptz.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2wnvhdflo.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2jlewicgy.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2nyppmqko.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2bcjajeds.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2yofbwizy.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2crxzyrht.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2scaqljuw.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2lerjmjyv.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2ynggltny.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2brgotgfm.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2qozdefts.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2zcvhlxfp.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2mzvhvgwr.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2lsamazqn.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2lxziwacb.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2lzxmzgxb.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2tmitoywp.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2pmlhgqcp.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2ratahvor.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2qqzjubll.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2cwakyxkz.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2iwhrnpcj.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2iustjcmp.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2rihmxfmj.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2sstosdbx.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2zewtsgcj.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2dzjetkpv.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2qhmmazfk.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2suogddpj.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2yzmgzrdl.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2dyswjfus.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2rrzxyuca.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2uvxeztsj.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2ckguwfbh.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2irvejmci.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2hqolgvvs.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2bkuojamv.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2exlzsppz.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2dvdraiip.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2wwaryttv.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2zdvfmukf.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2qbweupou.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2wyjonteh.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2uzcctyzn.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2timkdazs.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2mizosljp.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2ztolfcqk.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2tqlxapmy.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2wloruiii.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2xudlxdcx.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2inmxbdkr.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2zcnbevtg.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2zkobauox.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2chydeevz.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2wgdahksm.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2pkattqow.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2yooucrpe.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2yxvdztfx.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2uszdwcmw.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2mjwicjdk.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2fzjakfcz.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2wtelbepv.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2ildwblpd.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2doumoonh.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2tpiplivz.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2tefvwzxm.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2eitgvahl.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2mnhmnzrh.html


<!-- 参考信息 -->