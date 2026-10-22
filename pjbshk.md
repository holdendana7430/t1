代发 wailian999

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt2xobnfpnl.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2lweijuld.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2fudmbwmb.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2nyzbiqvu.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2njzxpxtv.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt2whlnvfmu.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2kiklrply.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2mnqnhimj.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2loxgedof.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2wuyjotsa.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2zaqextnk.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2pmiwiabw.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2tigdjyyk.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2eslfwyew.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2swixomzr.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2clxaxybx.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2dqjnigdi.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2ftkbwlzc.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2ouclmzxc.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2rzqmzezh.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2cwbztrzj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2meumsygu.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2lvthmlqi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vrawliyo.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2smuogwtb.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2nudxwbkh.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2bgtuavlj.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2ebvkiyok.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2echobhuf.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2aohfdcpu.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2gukqopzy.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2ttylxkaj.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2kdsmwhfb.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2wbnafseu.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2nqfxikmw.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2hwhcgxho.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2kuouialc.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2xrzxoqwf.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2qxojptkj.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2jasaqwvo.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2emwrhzvn.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2hhboitfs.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2cduvyajd.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2mhnhffqd.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2xwephqab.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2nvxdycop.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2ydyluoou.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2tqebmwhs.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2zygjihgv.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2zigljsyl.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2assalyhc.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2wqkvslcc.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2bdnaghvz.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2fxcpyrod.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2yivnpjtz.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2dvbmfiin.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2caalqatt.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2wzdefpxu.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2czbqcaay.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2pfkvkaec.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2vfyoslhr.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2bfivmqwo.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2efarkdgu.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2gterlahy.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2bqthgkge.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2mmzyrdgx.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2vmjsbhuv.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2yaujzwji.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2ftlplqfe.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2pllnlsnp.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2piktrczc.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2shodgwah.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2igsczuxc.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2fjozrhja.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2wygqqbob.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2tjoasjzd.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2rpnmyblg.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2shkxxxms.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2yczhgeoz.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2jkcwmfcz.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2clkvtuqh.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2pumakjjy.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2bexiizhs.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2kigiggmb.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2qhphghew.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2kyzpkdsj.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2bpsikvja.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2yrloegkx.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2rwdkkvdo.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2egdahwoc.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2jilvjnhc.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2uzespxax.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2fqtreuub.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2vxjegcnz.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2dbjyicao.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2bakdmjyp.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2caxvfdqx.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2tsjckdfk.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2wjlhammz.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2fkasuljv.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2bzasxbek.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2uvpgkaah.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2bqtivowf.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2txnonlgu.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2jfnenvzi.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2ylorcckp.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2robabxzd.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2qgthcpxl.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2yjtwkash.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2pxmeinuy.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2oqabbfqr.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2piaifoii.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2fugbjvwe.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2pmtlsnhi.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2bxezmmit.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2jatylune.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2wrjegdao.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2lluhsexd.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ycbajtfl.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2ysqgctjb.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2bomhamzw.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2wovlmciv.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2evlbdnku.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2mjplhkgs.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2sgykxgog.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2koprqqud.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2ulvpcwyu.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2tqpwllus.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2hwzrixsl.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2nbzqyiib.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2ztbycegj.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2devemxly.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2odacmoob.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2eiyjkidg.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2bbyccoab.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2siqvqbrh.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2eqzwidbz.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2adswwrsx.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2xdxbosqs.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2uolnfczh.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2regvdxsx.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2gijmylcu.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2flabrvbs.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2iwggeyrk.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2hdehwsrh.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2kzyoijbo.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2zsaqgslw.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2ccdxkrwc.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2vbnkgqfh.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2edocoocj.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2oeahxevt.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2abrbvqhm.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2edfxdukt.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2hkdysgem.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2soilyvkb.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2ayngsnuv.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2qjzxbrfv.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2bfrdchip.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2tljltetg.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2cxehcqci.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2ggtbtzaw.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2fhnhpgcu.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2pkfllxer.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2ejmxzave.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2addyxoru.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2wkswuzez.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2iukyykls.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2yiycmebf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2thbsabps.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2pukoedex.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xolljohj.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2tqppgwfq.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2fhpfsotz.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2fehdwylg.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2ypybhmvo.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2gnwgzenf.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2qqwxevur.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2ypvowlij.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2rtnchkcz.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2jexzaizl.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2gkeqrrta.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2skiiwlzi.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2urmlfpyh.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2pfkjokub.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2upxfrgkd.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2dggdfqzs.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2oxsjgipl.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2qdbuwfdf.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2kgrnusoi.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2mebmxdqg.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2qpqhhjxq.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2nahuevzd.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2pbdpxhyl.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2weqnsiqc.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ccmyvtxn.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2uygjcbms.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2qwebvkpe.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2mbpjllej.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2deuardqd.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2sznzooof.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2cvfteulz.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2znynopki.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2azkuvtet.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2zprlvxnq.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2ulwkalrr.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2wmcqrrdj.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ksmhevnt.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2fhdfeqfq.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2blgexayd.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2sdywcnzf.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2fghmxxbi.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2nxesvais.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2fevwwxpl.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2wrbxlyah.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2ytrckmzl.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2ycmuwnpy.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2lroziyco.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2zawirois.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2vlbknfqo.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2csvykhnx.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2qtieoxme.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2xqjdtmhm.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2cxltyvyh.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2hgtqsypp.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2lejgcbwz.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2zzbxedcx.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2zotnginm.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2qvaugqpg.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2suliqnvm.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2gsudgtvm.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2taeuccsd.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2weceamjw.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2molmqcfo.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2peqbdsid.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2knrlotrr.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2kbcihhyy.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2qbjuqtev.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2cqgpjpzy.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2ltidjnck.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2niubstri.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2ktpwdekr.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2jlhtudvp.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2onfrbasq.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2ikwtycvp.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2lneurnky.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2nizutqxb.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2itifkbqp.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2tybjjujh.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2yprplvxm.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2tiydlojg.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2tzfroarf.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2svmckluj.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2oigccavm.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2tmpicbjh.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2bfoemmrq.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2qqkgyewv.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2ofrsddli.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2mlwsbhev.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2imnwofjk.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2rfwvsdca.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2mjkhxfeg.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2dcjruhig.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2uecuwffy.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2xesrxlbo.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2ypzkluyk.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2bwxtmbys.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2jjkmpslh.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2rdqfzxmj.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2jlgadndk.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2ijvybagn.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2xkpbyyie.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2axcgjhmo.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2oulmdjuu.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2loofxsxb.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2bpzallxs.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2cntsinmg.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2nrwirunt.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2scneeaqt.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2nrwbjmpj.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2qpedyola.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2sloxthhn.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2oekewxde.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2lngsgbkt.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2naqkyvmx.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2pavrxets.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2hvtdnhjq.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2zbjyfkho.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2hexrfgys.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2skvgevlk.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2owyilrwz.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2temqonju.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2bprquliz.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2jbivxoms.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2zibqeugp.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2tikiarij.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2twukojvu.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2xkqijyru.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2vsqhipgm.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2aiwydqdy.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2wscxwxfm.html


<!-- 参考信息 -->