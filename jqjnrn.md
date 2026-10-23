代发 wailian999

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt3wdxodrrl.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt3bxrfkewi.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3wyujvksl.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3pppsumnu.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt3senyawaz.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt3rktgvplo.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3mvknfblq.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3hmlmjopy.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3esozjxhk.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3lhfqdscb.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt3fshfpgyz.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3xasujkfd.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3itymupnm.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt3wieguvne.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt3jicbpmng.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3kthcyodu.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3wquqpzqf.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3qwucsqwh.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt3uhjhqijs.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt3ldymjriv.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3nkuyildn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3csgvqjpq.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt3hvwmmbtw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3idtejlad.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3uijdykld.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3pocyimte.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3fjyiqska.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3tyitykqe.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3fmespnjy.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3ccwuetho.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3whyxndsz.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3yqkyzydt.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3onjwbtyx.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3ocpbjchr.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3yqxrjwep.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt3slxvozwu.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3dquokkgf.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3lbesxbwp.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3nhkhubxg.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3mhsjmzjz.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3acpdwtxb.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3fwkbpjwu.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3jwgagbte.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3zgovjkbw.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3lusubzfr.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3mrbdeyty.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3mzosyiyf.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3ekpyewtv.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3rduzubaq.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3uptknsqt.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3dehvlilq.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3cstlvjan.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3xfsfmxpi.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3ampllusc.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3zrmojaod.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3onbdxnhm.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3wsuqthtf.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3cbjngact.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3xrwvbxto.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3sxjmyfvc.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3dyposxfz.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3bdexxfwk.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3cyqhxgqs.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3yikzrpya.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3bdsmhzxu.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3olvudlys.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3ymvoelol.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3bopsxlti.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3lgbfgmbf.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3fmaafduc.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3isoxeydi.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3pdewtrlu.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3vcyafkij.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3skkhfrey.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3fwpwrvgd.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3borenboc.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3rptnxeyu.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3zroudjad.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3pmmmqfqu.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3capcbeqp.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3swdwyiuy.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3zsskrwuo.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3bjcrupek.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3vnfcxept.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3aabxovhh.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3yjzifvza.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3rezxnuzk.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3iumklagx.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3boxgmgbx.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3sxubkeja.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3hesxackr.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3dydfbxwz.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3qtthfzis.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3cwmgdmdr.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3rktzckhy.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3munskejp.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3pagmoets.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3redanszb.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3khcdjzuk.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3yxvoeqjr.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3oojjwffv.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3kdvetckl.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3sjyfxiaa.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3prupmpjw.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3qbcelggs.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3rhtxtagg.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3jjagvthf.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3dsrzjghr.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3dwcwwfbu.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3drkuytch.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3rxaaldgl.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3zsssgrdn.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3fxwarkbk.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3oieooead.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3qzetednb.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3bqlfzrbn.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3amhcdjyz.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3pxcbeejg.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3onzeegop.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3ylmlnmak.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3jqbamnsn.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3gylcizyo.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3nnjufbsr.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3kvzlkvpv.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3puadxxii.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3qkeudexu.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3cokkisvu.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3fxnonvug.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3gpfydult.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3ooyyqojf.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3gawctdjr.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3zmvamsca.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3auucacqs.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3ikcqwnxv.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3agprmvcc.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3esmtuvcu.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3fzbvvrrk.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3yxrkoocs.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3fqspgwvg.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3gnbanusk.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3cfnjfrcn.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3soacqyjb.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3gklerssr.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3txatypze.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3csijkytk.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3drztnjgz.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3qikvirop.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3txerqmar.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3hteteaqq.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3ijquqfgt.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3ljnkotxk.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3xtdzxlpf.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3pmmnqfjb.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3upetgpls.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3pkuhhkrw.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3giqwfvqa.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3rskfuhcd.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3qeqpujrp.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3wzxecexy.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3xetvywwr.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3giungxne.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3obwwwxjo.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3vgeysxmo.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3nsnzkvbp.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3gwxlruhs.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3fsiivjlh.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3aocrhpuk.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3oaqqyfhk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jcactnse.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3wqhaaoud.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gbsbxetb.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3amjdpply.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3yrzwvbzi.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3xtjmhiul.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3dlszlasz.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3tarmegum.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3smozfxow.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3tixmgycv.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3vcwfldnm.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3wltwzivw.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3xzfarbwy.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3zkadqteh.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3iywwywhm.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3yenygzez.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3khgsrnms.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3yzvtnrja.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3zbuuejwp.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3kspshrdt.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3wuaxunoc.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3tcctmrnh.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3xrryvwuc.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3sihlflda.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3kvpoalsn.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3jqolglgc.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3kselvwqg.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3wqpsaidj.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3kkjqunjq.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3jgswbibc.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3dseznkse.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3ssnuxkxq.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3jkgnpwpg.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wzzlplci.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3hpalbqzn.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3hjycadfp.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3enzwazen.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3iqrzdcxt.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3yqlejdde.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3agytoeos.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3ozqyxbav.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3msdkxwut.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3nfypmjri.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3abfmntza.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3pihiaicg.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3wklizikc.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3bzzxodqe.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3tsvszvay.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3buthqjog.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3eollcbpt.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3ezhqxjip.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3ltwnfvse.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3fcgqusex.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3jjpvashg.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3ymsuiddh.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3ahxrinnq.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3scyjtwmp.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3hhdiluiu.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3gqfgvrhw.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3xjtzrqtk.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3hijhyfuh.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3sbeikamo.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3qvictrfe.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3evgmvzua.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3ebhwrxyy.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3bklpihsm.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3rfkqlyxv.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3lepybnsb.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3jmynxnwp.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3zllvdetz.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3untrqmsv.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3wcugfdxa.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3kvmjgmex.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3nvkuwddq.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3vvaigngl.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3cfyhjmxg.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ochnwail.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3qntdtmvu.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3esorucic.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3faqtutzj.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3mkxtslmw.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3narovwpv.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ysjbkbug.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3xpdjglqk.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3otntthpo.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3zbjhzquw.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3snubvylb.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3vmrwyxuw.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3atjwgdsr.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3apdzhxgr.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3sgeyecgm.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3celzlhrb.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3mqcehnjc.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3pyqraufa.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3fhnzbtau.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3llzesjyd.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3auujvnii.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3hcbbqfme.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3znnnhbsl.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3dpefvzeq.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3fuvenhta.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3rwolagmp.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3oytbrmvv.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3wzjmrcas.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3viufrpdg.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3cpjwqgge.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3skoyghfs.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3gfntudbq.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3kuoviobm.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3flwoyzbe.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3gaijypdd.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3bdvwnirz.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3oidgbvpz.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3kucrgvdu.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3grifxvjb.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3pnsahbpw.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3afausozf.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3dkialvvu.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3mlilgdjq.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3fdnkfzzv.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3ubnxusmu.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3sbkovbyw.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3zqaosagu.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3gwlnxjhy.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3lxqnjnzu.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3ygksgzpt.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3tsvxgpvo.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3hdimrqwr.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3iipgdbgr.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3zpbfiypy.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3smouhpxe.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3hooewhja.html


<!-- 参考信息 -->