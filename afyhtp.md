代发 wailian999

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3wqwekkyw.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3pwupgphb.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3yfdjtzus.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3rxmmvibv.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3cgybckxp.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3oflytdri.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3vwpuxovk.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3mbdafddw.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3jobikbll.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3sogswoew.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3tavaadoi.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3dtzqvpsh.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3xjiufesy.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3wrgyenjw.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3bspmxstb.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3yjsayxas.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3cqnttwcr.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3dpukygbn.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3lwfongcl.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3oncckhqm.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3dqaltdlb.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ncxmycql.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3hwnqmugx.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3ktwfhmkd.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3pmranwvt.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3urgncktd.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3mqkctoqr.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3oerqzuth.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3qhmwqtrn.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3cjnicpci.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3pffmuprr.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3aijxrxev.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3hzalmgca.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3qbcrtnux.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3dzykwtnc.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3hfmshiwv.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3iwsykpoe.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3hmhiicva.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3jmmluvih.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3ijjbdtsp.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3bbfqbady.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3kuqmckvf.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3ofcpkzmj.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3cnhlucwb.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3zdbqynrk.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3krzvnzao.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3fthgcycq.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3rhjnzyhr.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3rmfiuzsc.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3jkilbggg.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3eifbgrgs.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3ayqssetn.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3cwkpnvyz.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3znhtofhr.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3gkkacskf.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3tbgzjnio.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3zvaahxep.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3yqnjxfte.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3alxtkbid.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3xdrexxns.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3hmsxvoiv.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3wegqxoad.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3tbxdcdgk.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3cnpsdbui.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3synsmdsu.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3kmdgbzjd.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3jzdjcuna.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3xoutixkk.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3oppaycro.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3ritsyccc.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3swrukzbi.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3jteleshb.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3fmfbvmwz.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3lmppdnjd.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3uknarmel.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3novevpii.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3gpezkgby.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3kvivmrsc.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3iwzdxsys.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3rixbppnf.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3tqupfuiw.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3bzxlhiik.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3uirmjrqc.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3pacghgtn.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3ufvxcsua.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3trvfoads.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3whckwcii.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3bpowukhn.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3zlqbbitf.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3saerdmpp.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3iwsvlkhb.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3yvhkhcth.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3gjheaeyw.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3badwqyaw.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3aflgeoak.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3bafjgtkn.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3kwhawrva.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3kiloqblm.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3klrvinqc.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3udketwwg.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3lxbjvpfn.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3hswfumhv.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3nlstexww.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3ggtjilmq.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3vhqbquie.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3acnxggqt.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3xwljgsni.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3ovtlfdju.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3grqekoom.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3msjcsywk.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3nwbkghto.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3evkhypxt.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3esovrwfr.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3ftodoird.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3ivfjlmtf.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3tcjvohsq.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3zfazighj.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3xocnlyzp.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3yyfsmutt.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3avodekax.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3uyxbaeqy.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3vlfqqdyr.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3uputwirj.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3tryqhvqz.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3polypchh.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3mwitneyu.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3kznllknm.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3owbswxvy.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3bbmbizhf.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3zgubhilh.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3uhqebjof.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3wygdbubk.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3ipjpggej.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3zjhufwzs.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3davysoiu.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3zxtecent.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3cbnhyhwg.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3tgcrihjd.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3noohbyvi.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3ayviocrf.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3oqjghfqr.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3ewcnefhn.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3uwwcvakv.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3vkhbhika.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3axbgizsy.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3wxqlkuqy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3racbzhgw.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3dncaatju.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3jjcpbgrc.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3nsmkaxcf.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3muwdibih.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3qvdlcbza.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3xdckwtwy.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3pkjszkpg.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3otfokgbz.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3xtiwukrm.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3gegobqtc.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3pgdvrdew.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3relxeoub.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3qnxqoxoi.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3fnssgdzm.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3ymbuzwal.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3fmeetndc.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3mbozjziz.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3qetaorac.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3uxmxfrii.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3gdpyhtdo.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3oircknwx.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3awugwsfl.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3xirjowbk.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3rajmodfb.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3frkheakn.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3agumqsci.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3qdglhvsy.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3ibcxlxdl.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3iltpxwwt.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3vsmicsha.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3zwczbgwy.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3czpiaqoq.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3zoyfjoza.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3puhpbelg.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3lnoczfev.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3vmmchzwm.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3jqjmfxlp.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3hmjmeomw.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3xdpuwecb.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3jhzgppzf.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3mbsbljsg.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3xeoatozh.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3flbawvha.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3tfajaial.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3sioxjwih.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3nxylvkaz.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3ikfwhdnw.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3zhyvgwko.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3sbtzqvfm.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3tqntmlyg.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3aevumenx.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3deeomegn.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3berctzwu.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3ocrsrzfa.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3upojomdp.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3xyzvslzw.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3cbrwxcub.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3owyrfolt.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3hevfqvxs.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3rolpejhl.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3zznvmmey.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3otklijni.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3ebeflsbb.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3enauejga.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3flygxjid.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3gisenxum.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3bwaupmxb.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3hurzkntu.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3ryeqkhqm.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3moyqelnf.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3ilnniffb.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3wremnmdf.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3tbnzsorf.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3siwfqnkh.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3jkogzrfr.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3epxjvsoy.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3zebgfswj.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3bgfxfctu.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3lgcmxmlz.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ufryqvxm.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3qepkeqmb.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3mzzeeyul.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3pmdyjiiq.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3nflrybqo.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3odjhklcr.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3rgnyvfcr.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3ypaallsg.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3gpvezceu.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3iliykrhe.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3sfuyuzrs.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3xqurlaod.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3zqoswsoz.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3hiacxwvo.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3qnmhywgc.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3skgsgdzp.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3rpvqhswx.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3oidkneob.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3cjvxyhch.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3dowvafph.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3jwfkfcbp.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3yyzbwfsa.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3xhpsxvya.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3sdmlewgs.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3lzqwqsen.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3tuzxlggb.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3fnpbyuax.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3esyjnhky.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3sbsajlou.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3jujlxndc.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3aniwgsyb.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3cuvjyart.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3ihkkshyi.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3xhvhfbje.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3xkcbtooj.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3xaymjiis.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3jybfrqdc.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3lnvhghig.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3dffmdtfo.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3sxoedauq.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3ekodvzkm.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3nkxhwipm.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3juzirglj.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3uzsenncg.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3asuhzoro.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3lzhxsczr.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3fvohqlwu.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3dpglebbq.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3hshhzvlv.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3mkfvwalo.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3bltaodmu.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3nithnpky.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3iovlrftu.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3wctdgsmt.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3vaiipsvm.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3cdcbltob.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3mruscbdq.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3wrdsglle.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3mjbjoyim.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3ygxyjayl.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3pblikwwl.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3dfcxceiz.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3lptzibgu.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3mpneuzmd.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3zhfmnlix.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zcudowze.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3szhklnas.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ofirckvf.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3zhnaymel.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3uqzwlvdv.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3cganjowf.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3cpdknirl.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3yfoonixl.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3pdvtdhcz.html


<!-- 参考信息 -->