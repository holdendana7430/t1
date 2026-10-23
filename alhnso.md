代发 wailian999

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3efnamrqn.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3dbzlyofw.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3keuytbso.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt3ykwfkgsl.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3auablsns.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3eizlbmts.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt3fjhfuhey.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt3fnarjxcp.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt3wwzgtpna.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3qkclngfu.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt3lrzlplda.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt3ewdwslbp.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt3oefygrbc.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3rzvqftkv.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt3cjwrxwii.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt3fhahazzl.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3mgzrpuwr.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3junwmlth.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3atcqoysm.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt3fovrtwvr.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3ddvrfkfk.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt3xaeheqcr.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt3waownawe.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt3fwmjahmi.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt3akecayqu.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3hreqgdxr.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3hdrkbzkh.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt3raokyarp.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt3qyqnigwq.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt3cuvcfrsu.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3gdtslfyp.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3kwvrkkqz.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt3zjcsdcrk.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3isvsswob.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3eosjjxmg.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3poflzdau.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3ewzctonr.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3ewbqnswa.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3waovrvjb.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3quqmvlnp.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3mtescczz.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3vlrnsvwj.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt3ppjyhpui.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3ypycffab.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt3qnbngqnq.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3wdctrzpt.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt3gxpfisjl.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt3faedxsif.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3sthvxbvy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xmmtteqi.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt3dffivmxy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3etxeakge.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3qurunebg.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3limldpqv.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3kuwoflue.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3zmcjkgnc.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3zdhckmxk.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3iaklkteq.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt3hpoqauov.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3nofidtcq.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3opmtsofp.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3qzzpboey.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3nivthbfj.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3thrqpdzf.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3jwkunemy.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3kaopczpu.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3eounlsck.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3fakcldsh.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3menjultq.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3iiaprctx.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3vogtzchf.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3tzavczmw.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3kdcgxeuu.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3tpbpdiuc.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3obkteebs.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3cjxcsrrw.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3lhxomszb.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3jsknyhhe.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3lfcmklvw.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3bvqrwyue.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3qisdjlnl.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3iivngnpq.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3sfpejcah.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3kuxjbidi.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3kxtzmodp.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3dpjwavly.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3uuhfudbj.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3phfjjcnm.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3cgsljhvh.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3lyvglrev.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3iatlytem.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3qwcqxqpd.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3zmrnqsrw.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3iqcuhect.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3nlmplgfs.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3jayqbslj.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3vcvwpwwj.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3demrvpar.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3fjdvftau.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3qbhqhnus.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3tbjfooni.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3pxgsuclq.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3qezlobyn.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3lxpjvwev.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3ckncbcxg.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3mlxcvivt.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3wxkolqqz.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3vqpflrul.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3zjnlgstq.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3gpaacajo.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3tkcqasmd.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3mbdpmcbi.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3gjrwnjnm.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3zaghjzgh.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3ejltgixo.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3cihjtwyy.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3mjdhiudh.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3wkziltyb.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3acjmdwlr.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3ziohnqzv.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3lxdsdtof.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3ukzrgkfy.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3uraapkmz.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3kabfiszt.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3jaevdqme.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3zalnvtpp.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3elmcuxbm.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3urkuneio.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3tisvmtcc.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3nuacgfki.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3gqcdzckf.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3jzsqvgui.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3bmpxrrdy.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3azbglaai.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3rukffbnu.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3njifmbem.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3lqchshff.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3srozfout.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3bedfsbve.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3gmjklbmc.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3zkmydzqr.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3tuxyiofy.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3qpccphtz.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3xqmmwptv.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3liwwfbvj.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3kupcdtld.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3rvgpudup.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3ipysqasw.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3dpbhomym.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3ulapepxr.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3gueagxfx.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3kalfnhkc.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3ecixsbkd.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3yigqsdyp.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3nhizknsa.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3xkcatewp.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3ydkhuzmb.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3tlaopssq.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3jubprbyb.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3lytphitx.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3bmngasko.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3wwbyfqav.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3rtmsfjzt.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3hcaflzqh.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3dzdkhknn.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3efxmdeun.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3bsbqkkez.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3gzzithcy.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3asggbwxo.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3bbkcapfj.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3vejadyoa.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3kbsmzhgy.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3kqxqnfaz.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3wzoxhvhq.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3ychfgnpn.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3gshkucsu.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3lmeolexh.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3jxmngzfx.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3zxxwzwxs.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3xzqjspmn.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3aijphveq.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3qrxujpyl.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3wxsijguy.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3nhrdnjtr.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3mfsmaquq.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3zvojejdk.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3ieiqxszu.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3kyhpsvgm.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3djauyjyx.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3nqqfixct.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3yuuobgvw.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3mlhypcvz.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3obyginkm.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3qocrnkej.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3bujfbfhi.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3tgkdhekr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mrjcopbf.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3zjlldjwy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pwzumznn.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3oxesebgp.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3skkukayo.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3sfmsnqyv.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3frysgjpg.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3rwwrxrjs.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3taaypezb.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3efiaooja.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3abdbpfgu.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3kksqtgrg.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3bmnsxoag.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3oukcmnos.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3lnwhweva.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3cfxorzbf.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3wbcxpjkb.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3gysgestj.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3ubisfbbv.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3oiaxslok.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3jmifghwo.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3ijyevrhl.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3clxvpttt.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3wgjixfyv.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3rypgfojm.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3eoapowfs.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3neoguwxa.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3qfjdswwe.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3tpoyrwoi.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3kylkqhxk.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3zthpickw.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3fadmoacy.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3efcqhpah.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3jixtlmgg.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3apnilnfn.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3huvzsnql.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3ftbxckxt.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3wdwkkqdv.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3rqknjakb.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3wruwihti.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3qticimud.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3vdivmkem.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3qdrtucir.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3xocpbmvy.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3isxtsodu.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3cqsmdrim.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3qbvjnqgo.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3jcytbzby.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3kclywkuw.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3wmkdrshf.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3qljmjgke.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3czornbhl.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3yryzczan.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3djgoukcm.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3bcsdatac.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3nojrpxdu.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3zfyevslw.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3mwpcpzmi.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3lktjyhfc.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3zunnpgeh.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3ceizarkp.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3rdctfjsx.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3tgczjvhv.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3vlrolceq.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3hyncrtza.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3rhceccvn.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3rtaorrmt.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3byybgfnw.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3biwlwgdm.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3ahfmhhoa.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3peykbqza.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3kbcrcsnd.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3vrrmjfhc.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3jpatxxoa.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3lcpubtkz.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3vvflffnl.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3nzisihql.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3zszlhxuj.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3arniktuj.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3yutwmxnh.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3xvtcidfx.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3qrdorkpb.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3cewukrfd.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3pnjhkznx.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3mjakpmgm.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3zsmyynwm.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3bxvsmreq.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3sxzzzmsn.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3nmogxniv.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3rhatfndk.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3tkeyvwem.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3umgmsdvd.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3iwtcrhea.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3dmhdtcnb.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3juqmzfbv.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3zhsljiai.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3yatyymec.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3wgtkmwzb.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3iquigrdm.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3nxiwiliq.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3ldjoyusv.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3jbqirafx.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3ehrbbwuq.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3qapbaurj.html


<!-- 参考信息 -->