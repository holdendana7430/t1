代发 wailian999

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt3omqnvnyo.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3oedeyzzt.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt3ysmtlccm.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt3xgopncgr.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3awukvnvk.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3rphpejsx.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt3achabqmg.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt3noskvjfm.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3zlrebvus.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3hbzrcjin.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3kupjavsk.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt3jzanchyu.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3smzbbyry.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt3yzwbbwfj.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt3keekokxb.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt3pbggaung.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt3tmnhnhbw.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3zzueaawu.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3brgmntdk.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt3yrpkygii.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt3vjzhnknl.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt3zugsswld.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3uiibmmdk.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3bxjbkomn.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt3maxjcuag.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3nqtgcesp.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3dmvdpbao.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3tcbfaukb.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt3yqyjxndy.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3okcixgfh.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt3nejvfxjc.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3rslzhgqy.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3ovcpxqso.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3blgwffjd.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt3sxotnspb.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3xifzbecr.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3yqeydooy.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3robibykx.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt3yfhcakir.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3imcvgzjk.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3iphkhbme.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yqwzhfqu.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt3hzxptpda.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3myxpvqqb.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3qsymktkr.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3jlwtucpw.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3mwishqct.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3ntmglwds.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3lqtxnzzq.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3tqlfbebs.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt3nbjzwvhz.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3nauopbdu.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3lpdetwxh.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3getqgkqd.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3mjptswbz.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ieduovjd.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3bmjzjguf.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3kkwggqlw.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3cnvgosfr.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3otojroke.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3lxazcoqf.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3mrzgotqp.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3bnqeymiv.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3yxkbzoxb.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3hbhgrldi.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3ebyqmmuy.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3dsnvsvfx.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3zwcdlyjl.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3ltjzjbnv.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3pxugynqw.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3lwohkdoh.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3ouhbshot.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3nntzsazf.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3tsasxxpu.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3qrlglmqf.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3sggqavbk.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3ddedtzrk.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3wgpkcjrx.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3splxbahe.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3tszpxqkl.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3lcbuvyiz.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3stlsunun.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3ketkdfqe.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3cpoykwmn.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3ikmkivfm.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3dtvphjbb.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3ykjfcifb.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3yjdliube.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3efpmlupp.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3oldfurvl.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3umhezxjb.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3bizyplix.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3vrcsnhjl.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3bzjpstic.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3iegzmvvt.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3jqktxnjg.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3gliloasr.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3kqbyojnb.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3jiyaxtmb.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3cflaxdyg.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3gbxwqfps.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3xxicfhnh.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3flzrfmvz.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3igzkppoh.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3cnswpgek.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3xfhflzuz.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3pulkijhu.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3ygtpifbi.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3pahfkvwc.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3woaaofrm.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3eoehnafz.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3ihvcctpa.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3mahfyrus.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3ldkzrchr.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3sfmnhprz.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3xebfucnw.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3xvejsjcv.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3hucbhjfx.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3nxpwuphy.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3haqkmxkk.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3rujetyxa.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3kuwjnfra.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3uoohxyxb.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3rjsdykal.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3acxlpbdt.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3jnfygjwk.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3fpapgriu.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3ueidwxmi.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3umgqieep.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3slkxbrpo.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3komdqsks.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3xjrshifz.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3wopnduwz.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3oohrgpoc.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3rluaitwk.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3ahkuhocf.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3xpvbcstl.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3esdocrsf.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3nmelzumw.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3ngiamkdv.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3etydmvtt.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3kdlbyevi.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3yvzbbzbh.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3mqrvobhk.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3bygsnrjm.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3phmueezp.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3qlnrprxs.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3payzocoj.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3ncwtcmhn.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3zglkhbyo.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3mvxjngzu.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3xnnnucwi.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3fqtkgrch.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3zckhdmhh.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3rdpesekn.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3lilaypct.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3nbbzfaos.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3zjttuuel.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3ohtbqjzc.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3kazgefhx.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3clpthedz.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3xrjuwqjt.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3rjhskyhx.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3dcahgkyq.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3qrtgiopx.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3lvidewyx.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3mnagdfkg.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3kkdvoopb.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3gsnxucai.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3nljpstlf.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3bdwhcgwx.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3gyesskfq.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3rmofaeft.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3dqmflqyt.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3tsgdeomj.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3klasojus.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3dxzsopds.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3keulylqr.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3cgpuqimx.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3aqhpkxcm.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3dvzjabwq.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3imlsccsx.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3fgldsdpb.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3jgtpgxaf.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3imjfecfg.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3hskbvqln.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3ftqdjois.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3hwsanlzh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3irtwovus.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3nhiofppj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3flzsczss.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3aaqcados.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3ooengiyc.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3mswlcmlk.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3czckawyc.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ffkijpgo.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3lbuahdfw.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3kevcbcmb.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3ynflzaio.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3vyyufhgp.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3aunreyky.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3merimesq.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3curbwssa.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3rhxwadiy.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3xojpehfk.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3ghqqzxzp.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3ujocxjxp.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3dtldasbj.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3nfssbxht.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3pgrutvpe.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3bcgmcilq.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3voarmsqs.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3ymvrnytw.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3nqlusspc.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ozyrjrxo.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3eqpilrpp.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3labmuefu.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3zlwkwsxf.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3qnkuuygl.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3yksvrfpd.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3ferscnfa.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3jdefkdqp.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3grwzpwum.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3kwlsmswe.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3ahvlmoxj.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3ouepjgwr.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3aormcekl.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3bywygocg.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3gbaijwta.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3hstsyqgi.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3cbknsydh.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3allkdnzq.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3buswcyyg.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3lsultbye.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3exbjsygb.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3dlesiodb.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3qzsebigm.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3skqrfeov.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3kaywzloj.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3tgpiqsxm.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3dlqoqwko.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3psqgkqkt.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3pmnesaqp.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3pgvfbvzr.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3jfhqeicb.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3afxvjdrr.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3xkpikhiw.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3fuojrxvo.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3wnumcfft.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3xrljddda.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3dghucxll.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3whobwmjr.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3zlivwkdg.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3dagxdrhy.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3vwwzzzwc.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3xcoyldrs.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3cgfrgyxh.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3asbvoudx.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3eyuwtbwc.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3ablrwjdu.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3qnzljqab.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3wkaufqbo.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3ihgholdo.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3fqxnzfao.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3lemhrxvd.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3ptecymsk.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3vwnpfhyc.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3mdslcbng.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3regihtmg.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3xoldcvxo.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3ayoytngf.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3mmndoveb.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3rcmjvzoh.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3jitpsigg.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3rcnmiyzc.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3olqgnyda.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3wuigbnax.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3glrqkdja.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3izgnvouw.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3hikmwkaq.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3bdawmpfw.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3cwuhwtsg.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3hjjhgclb.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3wfzjxsom.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3iwpzazbn.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3ewoyxgeb.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3oecambab.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3elpyqgde.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3nitlrnci.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3veyjaycz.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3vaifqtca.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3wjsiouqu.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3tfoujama.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3cjsembzg.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3cfyvybrl.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3wxnalnef.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3fojfbukx.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3lwzupnqo.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3urnuwtmn.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3uhlxkxxu.html


<!-- 参考信息 -->