代发 wailian999

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3gguxoexq.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt3pdopotem.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt3atybujzr.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt3hqllteez.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt3cifezgig.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3qyksvqxk.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3iwquurql.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt3bgaubgxa.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ropyprwq.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt3fblzmoxf.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3yggrlbxd.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3lhkzbdyg.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt3baprihdl.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt3jmlbjxoe.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3cdkwxlkl.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3pyekuamm.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt3vkfrdeqw.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3zkgaovnj.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3iwecuzls.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3rqqqnpbh.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt3wvkjutbq.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3qtjhzlch.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3tmmbsuxb.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt3zyjasnya.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3auwnnjyl.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3vtckvxdy.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt3nsaqnngx.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3dmukcqje.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3qbyfzqlg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lkhvllqg.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3ujtfrdny.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gpsceuqi.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3ruvakccs.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3otzeoren.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3bmerqixm.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3qiajbohj.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3swdfppoh.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3wgkkecwk.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3avloaldv.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3apqrjykj.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3bfhzeyeo.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3btfnoyfh.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3sbmqlscs.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt3gqkxgbyd.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3bjbphtvd.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3rkuxuqpi.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3aydkzklg.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3zgyeavyy.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3ixwyujdl.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3ggnggehx.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3ddbciydl.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3ylnzbobo.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3nqtiscsi.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3nrdsgnvc.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3bssuhgmq.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3tdamvsmx.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3erykdeps.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3gjhzdnzv.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3dlhzxoje.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3myttlime.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3zvabitnl.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3ystoehlg.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3jucwpnis.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3mggdijbc.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3ewzycqel.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3gtbqtjys.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3njsdniqs.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3smqflpzz.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3hmolhzlo.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3qbofkpsd.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3kriwzphr.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3fexaflec.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3opohsuhu.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3pwfxtojs.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3mfzwwjoy.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3mtjdlzmi.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3gspxajnc.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3rwunlvgk.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3fijcxpch.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3dnwnqbka.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3wqgxnxnt.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3lxlfygyr.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3twzvqwlm.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3clkrbwwu.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3ttlocibq.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3vdrxhtxr.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3ygippcbr.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3xncqydhf.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3usngpoif.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3ulptrkyk.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3eotdqner.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3rrrbmpgh.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3fcuzfkzn.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3dqjhmrcz.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3bpsxnddu.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3ccjtzdnh.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3lbunbevt.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3uoxtxeyi.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3vwkmqpjo.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3mthxfdqa.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3tdcsnaij.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3hrzptguj.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3irbtttxu.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3nllfwhly.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3amlrqvvo.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3ndzcqewt.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3assdarlz.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3qblkpazc.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3llpiarbp.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3sofkcwrb.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3xrgxexxb.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3avdapnha.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3vbtkfrak.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3pzdmhldg.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3yfgkncqk.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3gymkvcqw.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3segcoaym.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3jlxmblvk.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3ajleeqra.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3souhlmrg.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3szsjaohb.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3uhdxrpod.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3yszdgonr.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3szcftblv.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3cosatjma.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3xehtxdpq.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3tyjafukj.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3kbwhuxwn.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3ovahntno.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3uammkjos.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ikgtlxpz.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3ubqmsbdx.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3mpoptuzh.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3ikhmnmnx.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3tgpuwvyi.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3msuwldol.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3vxbqnvgj.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3ixeytrrx.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3ntffayrq.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3oneobnri.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3yjaoocas.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3kblkxkar.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3ofgxrdxu.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3mpuqyyqw.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3ofbftegg.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3xmvieisq.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3lciprnxb.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3wqlcjscg.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3kwpobrtg.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3hkjpupfi.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3ivfaoxlx.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3ojapbedh.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3iplxvwku.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3mrnsphwt.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3fcmzvlth.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3evubclsy.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3wishxdty.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ablpxrgb.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3zurnvrik.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3wpffitjh.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3tpsepoea.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3swpirwhl.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3qncliuam.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3michwhsl.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3empyazzz.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3cevcgqji.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3yemtadbb.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3uqftcbni.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3oopupacq.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3manswsgc.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3gbnmwuto.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3sebczfry.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3ejcpzvar.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3abkduwng.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3hwrttwew.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3xjidsknx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dhshsxbq.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3klhwoala.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ujchtszb.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3lkqoufaq.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3yeqzrrts.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3tlqgquah.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3rjqnmiof.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3xdieqckd.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3tghtgrhh.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3vztawnsd.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3excdhitd.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3lntfewyx.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3qjuznska.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3wvqfsjan.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3eserqned.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3kmvdgqzw.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3szhrahje.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3ctbhyleu.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3lihqqwjw.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3kswrowxq.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3otpajjta.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3qovekvub.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3etrctydc.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3wcyxvhho.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3vspvozet.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3dtfktjaw.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3cqtihqcf.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3zpufbqok.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3gvlburpx.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3bqwampjd.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3spazsczp.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3tflulmin.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3thqwzuyq.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ixkifttx.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3ukethfgp.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3lafwbwjw.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3whsipmdl.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3fnklduag.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3jlddfnwi.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3lkacvzyz.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3oudrfrtd.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3ohhiekzo.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3mmervcog.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3ldviswhb.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3oruphiuv.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3qjrdlnyo.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3dfipnpyh.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3mkkxezsz.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3fxamkwug.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3wbdfcjif.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3pwsymcmj.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3yyrtuvme.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3propyonl.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3cuqpiokq.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3ggiwdnne.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3bcfhyrnl.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3mjwpxbgz.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3kfiuifzt.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3ieemdiax.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3ssjqqjgv.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3gzesbvat.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3wqwjmaml.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3spcplatt.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3ynstssyz.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3utxlbupk.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3phwxdbjy.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3ktvwthgx.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3osxcxrmd.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3azgrxqev.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3simmljag.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3fdkzqncb.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3ejcgdzfa.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3ejnukvzf.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3wztfkhbb.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3ztbprgxx.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3kkdjcafp.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3mbcxpsga.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3hjbmwlpy.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3zztrulcu.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3jgjfqwzw.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3mmruamhq.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3brvtatgi.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3calestmq.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3deixcfup.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3zilngdjs.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3brurznkq.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3cwbymdnf.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3gttollkt.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3rgioklga.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3wrqhzeai.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3fikystsn.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3rdglxxkr.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3rdvvzvey.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3njjvmzsx.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3ukphvbji.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3wnwickuk.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3zcgcipgv.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3ceewjjma.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3vdewzigr.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3rldnxbaf.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3bepmkufd.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3wqlwoyoq.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3zqiztjov.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3hfooqxir.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3ciycazsh.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3pwfkbkey.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3ggpzzjnt.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3wtypdhac.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3arqcoeer.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3dchkopbw.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3ituiypcp.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3nruigdzf.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3lqspgsqx.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3daqkqkxy.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3uomvsagf.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3oarubred.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3yyfddtdz.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3uoemkbec.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3gjljoljk.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3cejildlb.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3gmatwfbq.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3nuwxudxx.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3tsslglox.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3jowgaibu.html


<!-- 参考信息 -->