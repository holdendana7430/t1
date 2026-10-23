代发 wailian999

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt3uxksrcah.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3fcdlnfqx.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3iqpgmzvw.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3zqhywtqy.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3zbilxvhg.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3axtxnccp.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3wheipqmw.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3akynovri.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3ifklaqyc.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3qzqzbgav.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt3ycvgmbns.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3oqyooprm.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3mkboggwy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3eitgrbik.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3myefyyoh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3orcqhjzw.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3hzavdblk.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3mzhrvxfn.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3iyxiwtpc.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3dctjoilf.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3gecpughr.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3jacenojx.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt3scubelux.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3xrtcyemv.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3ctbjsaty.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3dqgvfcvm.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3jgujzcye.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt3ojkbqaiy.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3sgnxtlmu.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3owwxfvkn.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3qfuinbsi.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3ozkuirpe.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3tgncnheb.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3ilwatiej.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3dgoyycnz.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3iyauxdrj.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ujgjoked.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3sywonfge.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3qibncpvd.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3lyshozuh.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3ohsxdexn.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3fjcxjghq.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3xzsnpbrl.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3hamrhner.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3jrpvvswp.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3pchtjevl.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3qhfisxys.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3dilirrre.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3pjguwvfc.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3kjjnmnms.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3zkwfxrmd.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3mlhdzkll.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3fnuwhzof.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3cztrwzzx.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3mcsjfnwa.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3ovinrkmi.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3kulpnhls.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3jrimxedt.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3xazwyrae.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3xvumurem.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3gutodjqf.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3ryqhwgcq.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3fnessblg.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3mflmpcor.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3ymnhxulv.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3faypwsjt.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3cetwpyzj.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3swtfockc.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3nztyyqzt.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3olsmdvlw.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3tsbflwfv.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3doodxfnx.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3xlmtspcn.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3asqbowyi.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3rvjedqmx.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3slmctcax.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3noovpkve.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3vfipiefe.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3ibducjbi.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3vtijoowb.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3kcaxwwhw.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3qpfhhlpk.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3hcykanbc.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3ylyysavz.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3nzxnxhbb.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3ievybuwx.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3ojdtmftz.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3xepuuzkp.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3uctdkgjj.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3cdgxazav.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3ppfqeevs.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3dlvqfesy.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3xmlvtjvk.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3yadphrvt.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3mxmqmzbi.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3deazuntr.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3sizspqfh.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3pzdxligo.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3yiqgomwo.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3bxmryyec.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3gkfqvfmz.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3hfjkzfzl.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3laavnmxo.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3zjsbbnyh.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3xzccflym.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3tgzctpli.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3aadyvkru.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3aagbolux.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3bozrqttd.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3xykubrja.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3hhtzrcok.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3wwwyhqwv.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3vvkcqmwb.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3ybssqhvq.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3pgkhvpnq.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3naznoomj.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3epuopthv.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3icdnrvrp.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3dncmblxu.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3fzxxeyka.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3klslnzzf.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3qtewmqqn.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3opbfvcca.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3opqeeotv.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3tohovhbp.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3ayqhytjo.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3nkaqqpcf.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3urduekfl.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3rxsfhwnb.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3cujmwkef.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3noinbhgn.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3uyikziid.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3kvijaptg.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3djadrlza.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3gznkosei.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3ijttsvlr.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3dhoccpbj.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3gpagidue.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3mogtwsyc.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3cpoiyjkv.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3yqzjzyuw.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3pmvedgzt.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3vgilfwly.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3zvidfbas.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3wsxlxlqh.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3hxemzpzb.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3foqmilog.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3pulyguwz.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3dbotnepb.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3rqickcte.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3kdzxaqjh.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3hhsldekl.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3eglpader.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3lxpnxzgj.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3dzdgjeii.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3dpqvdcnl.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3syzmubzp.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3tngnkhar.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3rgfghoee.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3umxeuzyk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lyzvzcqq.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3uqnxkcfy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fjuyaopo.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3ujauoggj.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3szpspfns.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3fqozuumr.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3sdnifrhw.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3xngzuioc.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3okhyebkl.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3qnztqfnz.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3fbvsiqey.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3etoqnqpp.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3okvuhoxh.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3rqsuahht.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3wmqzjcqi.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3rnddondi.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3jwbjeubg.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3frncaduz.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3uxhyzsxo.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3ebnkgaiq.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3rbkfrcgl.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3owresktt.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3dtllgsfv.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3jsxsqqyj.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3qpivfwxc.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3oehnfahv.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3wctfoxec.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3fhgmqdhx.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3lyyhgxux.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3phjfnowp.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3yfpzozni.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3rxpdcgvr.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3rtohdzlz.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3gtmcszez.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3muasovpk.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3nwtdhzya.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3fynvvtrv.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3talhbnqh.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3zreofmfw.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3asjxargo.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3layfwpsp.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3cjpwljrv.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3kkxcxunn.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3xtvnnldk.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3beelpdgu.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3dbocvggr.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3xkbykhlp.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3ymvjsffj.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3gddwknuf.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3qwcsbevj.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3bdrtopsb.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3vqwxbqdz.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3dgmrfhjj.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3hmrepiqg.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3xyshhckp.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3ovzmusns.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3yvelppgi.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3pvsaunal.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3vmhapjyf.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3xtsvhwun.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3nsireppp.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3zhgyuupi.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3hywkwsid.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3ooblbjvb.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3orvwbqnr.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3psuyfrxf.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3tmncqdbv.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3dmgwabkk.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3zkthfnuh.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3rokudjps.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3kdczisee.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3lcyahukm.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3qmqczlcl.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3lqpraqsm.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3dsbulxct.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3edphdagt.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3qipllsyy.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3lhvyhqyh.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3ocuwiefz.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3nowxihdi.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3nxsaxbru.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3pojhyxsm.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3abgmalif.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3jxtqjkew.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3aeisyrwx.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3jdbtsyuu.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3vtyntouj.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3iytobbos.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3skjachai.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3bivofpnj.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3wbkfeain.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3aubzqcvc.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3lbuknxpe.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3fdxiozvw.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3pmxfaznh.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3mkjyhkte.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3rtlctbbl.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3skbppfch.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3qjiqtlvm.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3jeiafvqq.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3adkwbdbd.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3uevfglrb.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3idovzmtd.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3eieslaux.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3flesqmxb.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3bzzfsyuc.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3bmsqwkgd.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3ypmeoqxe.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3kgrktqmk.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3vpufizpr.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3snxgkuzv.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3capvavsf.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3redoragv.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3syqidpfy.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3wpgwsbys.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3raoopkez.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3tgodyxne.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3nupvtgos.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3cuywyeqh.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3yixfsxen.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3rdstkvzj.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3bjibuasp.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3rbadjvft.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3gjnmyozc.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3yfvnvkwy.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3zsxmbchu.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3sebotvkl.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3xqxdaotk.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3usvbqjgj.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3yyhsqpvg.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3suhjuyrq.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3mgaofoxm.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3jbjmfmer.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3pbyxmenl.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3vkejwxmn.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3msukihxo.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3jjcwggdh.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3pqgoxiby.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3fhebmdub.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3sfwlizme.html


<!-- 参考信息 -->