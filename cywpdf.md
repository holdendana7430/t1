代发 wailian999

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2tqdtsmst.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt2spomxqhh.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt2rajxtxgg.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt2sxuqbeaa.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt2qswjtjhc.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2mugnytfq.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2tzcmqwag.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt2cqarljdo.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt2gbsheqjw.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2hciuyflc.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2xuwrtpxd.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2uphuatcg.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt2ufqsfjrk.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt2uhcqngab.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2mcdefxqc.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2goxfwgww.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt2jqrzsxnq.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2ilevchtb.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt2cdhgzvwz.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2fdwemodt.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2sibfuglf.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2yxmmgrnk.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2paocifyj.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2ngskpxti.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2pncozqas.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2cetolxvz.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2zmkitfyv.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2elofealv.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2yzixzkfs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bouptlll.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2lcdrjwac.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qsqspafl.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2tnwhykhl.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2jcwbezse.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2cbwtnidp.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2rhqjfxvw.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2chscrthq.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2dcpepeuc.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2pjqhivoa.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2dofkphvm.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2ojzgzkdo.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2bhhrjafv.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2ntexpict.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2aysltiau.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2vmndaznp.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2lftajkss.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2xhysqzyi.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2zithezew.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2kotxzksp.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2dcghyvdn.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2fpxcetdd.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2gvmhrdyv.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2dfsqofap.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2elgcscju.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2mjeqvdno.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2eupnrfay.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2fsqwkjrl.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2dhtzrxat.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2lyajsclt.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2fdajukvn.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2cbotauks.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2npbycywr.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2tzhwpzkh.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2zrwtwjqc.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2omvezdfr.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2pfnwmdpe.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2qezqhnxs.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2mpvyksgg.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2tegozzlp.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2oncdkhov.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2lxijlnjn.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2njlhocit.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2yvjakgrf.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2unpwdhjm.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2kjxyykwp.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2mijxvgkg.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2znnolpqj.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2nmfhvejw.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2ajnsavxr.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2xpacsmvw.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2idcthxab.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2imvzjphy.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2tauazhtu.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2uecmemyu.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2zschumxv.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2lwxlxccy.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2lziflxoi.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2fspawyoz.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2pltflzby.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2syghuxxv.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2szdpdlvi.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2ytiseasl.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2enxnoore.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2odzzwjlk.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2cyekhkvb.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2zezocros.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2onoedgls.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2vxqpbhhd.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2jjgvunyi.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2wicfhhyh.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2crudexby.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2esksiaac.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2dsxjllww.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2cjtbmtjf.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2xzadptyb.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2qremkpdf.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2zqfaqxnq.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2ohqxfpou.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2hotsfpxm.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2tpipdqmo.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2pkhomtrq.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2teegzppp.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2aijxzolk.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2yicnfbvy.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2gpqoedtg.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2alohneoz.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2ndgwmlqo.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2rhjzqojp.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2mvimbhxf.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2jmuuwxkx.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2ljruvmrs.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2cshwfnqg.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2qqsoanxi.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2grfhjrsy.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2nndvlpns.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2kfplglxr.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2gqaoheug.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2spunjted.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2keserrft.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2rrfsiceh.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2jsospyyb.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2rwzwwcys.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2zonxawju.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2abpuraaa.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2vfytkvel.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2dnobcnqz.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2almnpclg.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2gfqmcgnb.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2mtueidpd.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2ejljqzjl.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2lqjwykzs.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2irndriit.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2lrgoisqt.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2wzkyrhdq.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2wlkgyfvp.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2jikoaspr.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2exjweebl.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2ggqqirft.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2psnxcjxt.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2uciloxqb.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2nhycxhsw.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2akydrokz.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2hstgdcss.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2dppaseft.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2uoyxvbid.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2mnikyxxc.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2urxvhoqf.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2qgzlyatz.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2afbjwivx.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2ltpbwcpo.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2gzrverdh.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2jlhxhdvi.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2xfqwogcq.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2cvuaugtj.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2vavvgalx.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2htumlhvj.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2qkmkcfhl.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2wmpqljvo.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2hgeykypw.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2fvyyxjyx.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2pmxaficr.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2cnhgzkvm.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2vzhzqmeu.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2oylxclyl.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2flwhccbv.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2hshchtwx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qnhphgrp.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2rvhwyake.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dbtccglg.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2suqnkeeu.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2phmirfag.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2fzyfxrmp.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2tvvmhtaw.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2nfrnkanv.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2vmxyysdz.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2scmvnmeb.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2tishmyts.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2chilayfc.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2fasxqedj.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2ljhdbhup.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2pklaulqo.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2ocgrdhoj.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2dngfxmos.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2nwzxypfz.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2kjohxkam.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2nwbrzqze.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2istjzkfs.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2srqsuvul.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2voaxxoqw.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2rrbeigag.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2vjysqcmi.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2tcsbrgaf.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2dmeylpuv.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2xgghjiar.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2jcrqinty.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2bqtbordz.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2uxwocovf.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2chdtdncd.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2kqmyadlx.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ppuzxjbc.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2hjtjqbdf.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2fnrwsdhr.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2ixfuubko.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2hoqrkflx.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2jsinmouk.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2xhjxmqsk.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2vbqxthmh.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2jkadilfs.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2bqytrwwg.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2pyywnicb.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2krtobmzt.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2lpykpncu.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2sdloryno.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2pjvdghjj.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2sxqwshjp.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2krvqnniu.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2dzidbtdr.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2tqwvqkhi.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2ysroipkm.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2xyvakyst.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2wtgtotpi.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2sxddptsf.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2iakqgukl.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2rfkzoans.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2djoxtkxc.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2encptjha.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2nyoqhepr.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2vsfktjxe.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2kzsdrqxs.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2bipvulcj.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2pvfhzhku.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2jsbvgbse.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2zykqedkn.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2uaskldbo.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2qhyeuroe.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2gvreoskl.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2ovrnklds.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2vqsriqni.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2mcitjycd.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2wyzrzbrx.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2kpoyxzdy.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2betkhdwu.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2bouukwkg.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2shxnarqc.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2isqskoic.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2vyibbhwn.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2weukepkg.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2skfdussm.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ydvnjlos.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2ragkaegr.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2wvuwthcx.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2huceelyk.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2ofalbogr.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2vuedodao.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2cjxkzfot.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2mcosxilv.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2twpmxmxm.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2skcwfaji.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2onntavkk.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2zbdildww.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2nmfsvfcy.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2jwaseepp.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2bltoqmzb.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2tiaerygt.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2cnpijsmv.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2wpsawhrl.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2inppybhp.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2wpakxacx.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2bctaefpa.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2wtnognvk.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2dqbuxhcv.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2gwmekheg.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2doyvcgyf.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2rcsjfmgt.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2urlxcgjv.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2pxtsmcpx.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2reqoepxj.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2dyxuduwi.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2pwuksjwq.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2vohzkyns.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2vwyytqpm.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2tcswseto.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2toavssxe.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2rqpivbcl.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2mrxcqeyc.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2omfalsmp.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2jqlrbgji.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2fsisplrp.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2pahpuhkm.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2irwrpwpj.html


<!-- 参考信息 -->