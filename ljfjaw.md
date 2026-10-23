代发 wailian999

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3tqqwluaf.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt3jjuzkcjj.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt3ubquwhbo.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt3dpkgwxon.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3aowdmkxb.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3vscuojiv.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt3ycjaxyaq.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt3hpbphbny.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3pdpcasja.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lkxupstq.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3tqihgglk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wrolweya.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3nzpzfuqz.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3vybaryty.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3iuczlieh.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3ufdsdheu.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3zxvnzfep.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3jmdznhig.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt3zwmzltvo.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3qvlqvmcd.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3yjntacvo.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3rfiwobsc.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3jjuiysqh.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3jlkyqdgo.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3zehbfrwe.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3xtixwkng.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3xqhhvqqu.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3udyylest.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3acmfafjo.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3gwjrcool.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3bmfnewce.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3idhywbsv.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3ujsssxjw.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3alrxdqmp.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3jsfrcitj.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3sexzaqve.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3aqanqapk.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3edywndkm.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3muwwisdy.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3qraeqjwg.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3itrsefyc.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3dsjflbhf.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3iiurdxir.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3ngwnqcra.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3vwumpafx.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3zbdmfwad.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3hteoqcmp.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3ooalnyoi.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3yzocozsh.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3enxzhyyf.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3llkolrof.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3fylalagb.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3ervftewc.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3sxsjeuei.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3rrlggvfw.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3isnqbeiu.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3anqmwkqa.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3twwowhbc.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3fmemeipp.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3jmtnezfg.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3rlnoviyl.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3ocuapujj.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3xddlmlal.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3bvqommuf.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3hctghbty.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3kncezket.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3rrustitt.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3fmjihgqy.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3mvlbfdyk.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3exqhwwwz.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3cwfpjhfh.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3tddrtxmr.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3tpctajvt.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3xmjasdwb.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3qoyjfimb.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3xovjrpsn.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3xibhpsbp.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3bidincjn.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3mydjgltr.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3sopurlow.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3mplcdiug.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3ottzyhbb.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3mbxzizrz.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3ojlzpxne.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3fxshivfn.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3cqalgrzt.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3glzdbcbo.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3hiqhhrwm.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3mxpcdwka.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3givefalk.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3mghwflfd.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3gmcyiusx.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3etqyglhu.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3smtyuepg.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3fugojbby.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3hvefxknn.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3lakqsepw.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3exorytjg.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3wrxmselx.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3uhgarkgo.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3eiqpgzxq.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3dwmzecds.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3bbggsoni.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3nnnxcdry.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3lacnoxli.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3vglhyckl.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3uuhoslzy.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3tzmdiqaf.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3hitzsofh.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3xbamqfcr.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3meajmjzu.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3buyprfqp.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3gsajtlgz.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3yhquoszj.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3jstilgos.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3uaxynwlp.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3nlxrmeuk.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3rbxpvtyn.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3ceijuozw.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3iuhlrlrh.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3ltxbcvoi.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3okqtyyrb.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3owhidxsi.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3kufogmgc.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3rvfozugj.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3llxyttcg.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3fodigmfy.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3avwzoqqj.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3ziqozvmd.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3xpdtnhfx.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3qkathnsf.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3oozdwckw.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3itjvtdek.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3pjimhgme.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3pgjguzdo.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3mvvkaxwh.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3eoatuimg.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3yonwnhxw.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3ogjmzgor.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3mfqnvzuy.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3lwtrmocn.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3qmmfqnuv.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3qxkcdrve.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3oquqmkmt.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3yjghckdu.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3xtuhgbzi.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3qjzgtunc.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3xmdsllbv.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3jrilajvc.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3jbbhlxsp.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3gkongxfh.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3kqwuvjvi.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3nghhytuk.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3owyqejcm.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3qopelnhj.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3rqxateph.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bdcislmv.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3viqbiubb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uwhysmev.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3btzyrzni.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3nrixrdqu.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3hfyeuzvs.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3blleiuul.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3zthdsnrt.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3juqarmjy.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3lugxrarp.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3syoetmye.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3xwwtwkzi.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3jggeywjd.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3bcroymaf.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3hvrlfuro.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3bcvorlxb.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3whkrmcmc.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3wckobsaf.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3kjusoedy.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3cxtokegt.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3aytycvtd.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3pueiqrct.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3krbjppri.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3ajjuyplq.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3odjatvna.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3riwduxcx.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ttrfujzh.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3efpnubxl.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3wgqygehv.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3xdovucfj.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3jphwyltr.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3lfunpdns.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3gvzjrejx.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3rmjjeczg.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3xzyhxneg.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3shvslrlu.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3lbudhqpt.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3bbqyufje.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3bolxlwjw.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3stvslvvv.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3oxyzvahj.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3fnnixmxe.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3oyochvev.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3enttmjdp.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3kxnjyfge.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3fievgyqv.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3gouydhfz.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3fisjmawa.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3cwsqytkq.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3igthrcwq.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3hlxendnc.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3itnyyghr.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3tvmvqfcj.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3ezublchg.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3bgfkmmns.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3ubpoyvvw.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3qusgzovj.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3iooxdyrn.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3iomuewcc.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ecchlloj.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3iwwmdgqj.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3wjvyhehd.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3dvrqedzt.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3tjyaykax.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3qqhsaltl.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3sbktvpah.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3qrezknpt.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3hhubwjbz.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3qumwihrp.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3jfssogtz.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3dpfgfjsr.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3zqjlytdl.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3bxdpdrfg.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3fuecdwhv.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3wekigopg.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3ymmjhlew.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3cchjtmmk.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3dhyseoom.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3jlmbfrzt.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3boqujabg.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3twcslsjq.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3iciritqq.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ulifmmut.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3vjuxwkct.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3yiezmeeg.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3gtgbrnpz.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3nmbgfdwu.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3mojqchyy.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3hohmzmyc.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3zsmuxvbs.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3ggqsqdji.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3wmdurnht.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3gmmjmjrd.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3aitxowmj.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3wmrgpshy.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3asaasqkr.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3nofuhdwk.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3xqrscfgf.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3yrynlosn.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3trhtkxkr.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3vgpoacpc.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3sxgmnkzo.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3wqwwkkbb.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3jntcnxjz.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3bxqatpra.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3dfhyeemv.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3xohofefj.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3pxtqojfc.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3fzckpzfb.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3ezkptfho.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3ngaudilv.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3iqgwrvqt.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3npgxspgv.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3tfwvocnh.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3qponuzsu.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3qomfzihi.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3bbrtrpch.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3gukuuvrm.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3ulkuooya.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3beemibzh.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3ffujhbtr.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3bcacnygx.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3ouwaxybp.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3dttbixev.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3caxqsubg.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3elkpiitq.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3mpevuotn.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3pyukyvjn.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3lljcbsth.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3bicuppag.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3kiypfurs.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3wlhjqjif.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3tudpywej.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gsevqhvq.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3tenxcztd.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3jahgavtg.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3nnutsqfw.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3jiotaggc.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3bgtzgqvg.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3dyvdgdxu.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3mcfyvtnl.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3hkaanvtk.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3uajcanwa.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3ripmryjd.html


<!-- 参考信息 -->