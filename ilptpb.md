代发 wailian999

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3xczvngat.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt3pcsszqtb.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt3vxdbakle.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt3qbhqovdx.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt3kxqlyiyq.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3gryxowbc.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3pjkcysub.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt3zraqmldv.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt3wijlewkf.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3rmxdooqd.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt3lpmzotuj.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt3egtsegeg.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3pliruxul.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3hffiezzm.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3wqulfmsg.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt3bedkiodp.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3ythimabo.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt3ucaxfoiw.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt3qfmnkhyz.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt3awmkfdjo.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt3msmcbsta.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3zswbonss.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3scelsnev.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt3ysnyktgh.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt3jlnlwxtd.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt3wwshkwvv.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3khavcjay.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3bsjoivpd.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt3ktastonh.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3llvnjkjw.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3cunvoszq.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3cyzprgmt.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt3hzrkunmx.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3mobdnmum.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt3jvfqyxau.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3blahmyvh.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt3qkxnzbvd.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt3yycwweas.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt3lvltvqbv.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt3neecqhqi.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt3glhmifqk.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3paeemcqf.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3iytuumyq.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt3xdbxegzv.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3yaanvcfi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3usysltpl.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt3wtogsnok.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xjnzxzsq.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3gvjxiavt.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3ujqkbpoh.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3mssqcdss.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3dyzuuomk.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3ljxxsrec.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3ajqypnni.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3fsvfazgi.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3fuqgzdvm.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3jmamhhnf.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3yaycalfe.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3kshaajte.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3tsqzhlfx.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3sdhtmijs.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3yptpiylu.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3eplcpsfk.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3jwsphnnt.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3ceuqkpkm.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3btckmicu.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3yxoiehlq.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3vepfvkwf.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3oghtbmqb.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3dzwzkzzs.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3ldeqtaex.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3iwxnukwm.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3jgndssia.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3bhocdscq.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3plpjbjws.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3qunikmco.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3iijjvmyw.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3ovyuccpn.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3yzyzvzcn.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3uobyjgna.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3gxbyojkx.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3doeauooy.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3pafplhjz.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3kacyaxcx.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3vglzodkj.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3rauebfbk.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3bzydcudu.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3ncjnqwec.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3xovaxxhz.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3obzvchhs.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3oocnfvpa.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3mccdmqmg.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3mnwxiqzp.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3xmbibpal.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3gwfcxime.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3htdndksl.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3bjrkjzuq.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3zzzauryh.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3wwxnqcnr.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3pyuoxphk.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3ircrpwkx.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3dyawurqn.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3iqjbtgnv.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3kmhcnolv.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3wjjihzvz.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3hsvorvko.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3terocqez.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3lamsjavk.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3ddjuqonm.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3vfsnprsu.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3xamruyhj.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3pbgsmade.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3pedtxaoq.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3abxupjch.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3vdlblonp.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3wzygqzhp.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3iviqkpop.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3uwmchncs.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3mpenvnte.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3aktkjxxj.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3rkjxoiub.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3oykznjmh.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3yeccivsk.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3njegcltp.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3uegwjrem.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3djdmtpfa.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3ymjuqjnb.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3ffbryqew.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3wjcziroq.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3zjvoxszo.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3qjubnqcb.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3oabwpgon.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3urcevjwt.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3phzlfdux.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3axwagghn.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3pwypzmzs.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3ljwohbre.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3byynifwc.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3tjldlfod.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3mkdvzmjo.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3yrgeyvqg.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3dgpwkrnb.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3wzyqtevu.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3gjkzpejq.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3dsmhtdzb.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3vhmnezzr.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ztnqmjxg.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3kbivzqna.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3uycuhtot.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3djjascns.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3kiveykzo.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3uriiqmjy.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3oyrkboan.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3xveqgbiz.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3tlgwebsg.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3dmzevrbc.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3iynhwfuo.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3vvktafmo.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3bbsjfvxt.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3fnqxhxla.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3yhcfuuwx.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3coebzpgo.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3pnhjedly.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3jknfucaw.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3fsyfzdmf.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3znysxulm.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3mzlscimg.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3vbluxhgv.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3lchroiva.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ylyuivez.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3hivecrxk.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3qlboxozi.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3lkrvkvux.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3vmrbxqwc.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3crivwvif.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3xgcnnvft.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3difgzavq.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3nufyjwjb.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3ykyxneyf.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3esskznki.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3wsjkfefk.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3ilxokxew.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3hdpqhpjw.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3zkqbwuqe.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3urqsjpcj.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3ftvoszzd.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3yayxrlej.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3yambmkxl.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3mbbzqiad.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3fgfxqczq.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3xstvfhta.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3couqdnca.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fpdyirsy.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3ineisfxq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xpetsvpk.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3bwcbnezo.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3tqdchvhw.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3mgsviojs.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3huzapztm.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3esxszaoa.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3ibpctlhn.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3kbapkwop.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3ukhmqarg.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3yedjovwa.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3tiimbcec.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3wingnmbz.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3orzlbdqd.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3cpxwdyuo.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3zsfcbjoc.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3huoebcjp.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3rwurmzpr.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3xsepeusj.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3igvflnrq.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3lmzrxsaj.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3rjfcjnvl.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3cqzxdgwk.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3crrnjynw.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3dmckzzov.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ldaceisv.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3xefdyxyk.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3mfslzjid.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3yfkelbyz.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3dfxybqcn.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3zxtityme.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3akmggjiu.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3xnodudwy.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3tppryubq.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3awhqfwhz.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3gfltjjun.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3zclnuzdb.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3netlkyfv.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3wkaparcd.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3ygwuvfmn.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3kqwrrezv.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3clxfxwvv.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3awqvnpmz.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3peynoywe.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3nkomitqo.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3nebueytx.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3ztdrrkoq.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3uuyokemz.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3ekmgdagf.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3hjelevff.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3adufldtp.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3eokslkyp.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3vltnbqtd.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3chntoggl.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3jlexhhgm.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3eimdgetz.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3tzgrixez.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3sgliswvo.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3mplxhidb.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3cgyzladw.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3xsofgajp.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3tlfiisdj.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3yyidkbry.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3luilbbfz.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3bcavuigp.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3zwwyciwc.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3thendevw.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3yuopitmr.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3muxtwkbl.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3urktddcv.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3dpldvbym.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3qgqbjidk.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3yigsjldv.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3bxelhbvf.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3jjugjqxs.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3ribyosrr.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3ecvwelpl.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3dyjppppf.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3uofbnaac.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3yhzvjawo.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3bbgpkgzz.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3uuuhgjiw.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3rmoagpqp.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3rgdcqxlk.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3lgivosar.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3abpfssut.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3ljxlcwzp.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3nkwuxmlh.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3lphcjtjd.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3zifegimq.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3exwdbokt.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3kcipbyzu.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3magfcqpn.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3mckbetbw.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3dvuyeyqa.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3beqdbgpu.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3weqolmjs.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3pjbxsozq.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3bxluvwni.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3slxpvblt.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3mgmpunhv.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3gcmqpwqp.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3cxnumpcc.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3zpndwjnu.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3txkovijl.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3zzvtsgkf.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3idjlxaug.html


<!-- 参考信息 -->