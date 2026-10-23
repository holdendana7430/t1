代发 wailian999

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3dcwizkrq.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt3jbfbfwha.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt3cyoeidqf.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt3tpkcykha.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt3dwjetljj.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3umgjyhgp.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt3aznsbxok.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt3higudeyr.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3yqcabmuo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3plyldlhn.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3afmxqjdn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uwxfzxbi.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3gerxloht.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3xufjpeuw.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3ntnszbya.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3hxuhoaus.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3aavcnkuf.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3kharpoim.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt3cmfvvtsu.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3tmrntpru.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3xgauwjzu.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3sczflhjp.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3jdtdvfbb.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt3ngvvidsm.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3zfagzsym.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3kleapbaq.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3mhiukbks.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3wxvtddgd.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3kznxqrmd.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3yghhanjg.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3viwndzlx.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3uuppvrzo.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3pzqudlba.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3mcgbzwdy.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3snsiterk.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3tsodgazb.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3nniobcyg.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3yyokaysm.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3ntqalrlh.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3rihyvxgr.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3njnirguo.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3uhnhonch.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3eicnsupi.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3ljwclyvf.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3kmkduyrx.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3tveesjun.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3yewstsqy.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3gafnjnuh.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3jdsbiegp.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3ggqxbdnn.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3avrkvidk.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3mbvapmue.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3invifmmd.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3sjbyecrn.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3nhpjchox.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3frkkjonb.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3imhrzzfx.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3vttpzdht.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3fkkjollx.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3mgzlzlsi.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3mysqqfki.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3fvpviqnx.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3oeyulmse.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3ttwxbydp.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3ipoalmgt.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3ogocjnxa.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3gcxvcgfn.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3vjfkafzz.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3vpwmsjno.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3mavrgkwj.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3kqwxxarp.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3awyloajw.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3madzglne.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3wvmxazey.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3heetdabc.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3hyhaoago.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3bjpjxydo.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3wnvkecrx.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3kolaglaa.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3kgykugif.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3uncgcqxj.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3tvqbnbaz.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3wyivkwdc.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3okllslpl.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3aavebcqx.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3drxudnfk.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3haioxgdw.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3ssqokscg.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3tuebzfrf.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3remaqidj.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3isrptyvx.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3gemxlwws.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3ucszptlx.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3yqbeobrq.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3utbzlyoi.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3vluhoief.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3zyuuryek.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3slcqvobi.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3clipppkb.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3xdungquw.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3byniensq.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3maukjakl.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3apospmjc.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3pfictroj.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3qaopqxea.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3kplcejlr.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3ifovlcxs.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3acxhpsxq.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3aytjevlp.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3myttwbbc.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3rbtrcvpx.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3jtadlhtr.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3fhinmfmq.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3kppitrzc.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3jdmnvfep.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3jmlpereo.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3zqvkloyr.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3plqginbc.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3edsjhbrp.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3yzwtprtq.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3acurfldz.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3kfrizvlt.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3ztwmtpas.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3gxuhmslc.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3rbjfilcz.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3owfqzuzo.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3kgqupprj.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3ighokzqc.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3ahnturwf.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3jhbzgvhb.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3itcmtaef.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3gqkyxbjo.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3ehgdebnx.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3epzenbzh.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3nvtbgxnd.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3kjfgfree.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3zbrnwrbb.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3tefjzhpx.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3qzqvnumj.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3xsynmmev.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3smxqvuvy.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3zjudtgjr.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3fzmjqqtm.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3cmitynjf.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3aialbyut.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3wrbaegzg.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3ubrtomha.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3ggoijvnc.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3jlzpggdc.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3uwgucptv.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3racontab.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3vqetuwio.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3khzgphad.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3lhnlxasm.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3oqnrvczw.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3ubsipljo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gtvejspc.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3dwlmsbqc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lxvdtgqg.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3yvxsczeb.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3bzjgfxce.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3xlisyzhh.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3mgpiyece.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3quepnfgn.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3suabrvdi.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3jtkhkgui.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3qygqdbcd.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3tjurlgrz.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3tcfnzmof.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3xdqvijmd.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3gewvhrxm.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3dfhmeypv.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3jkwxfkhj.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3zcppdxtu.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3roegqjcg.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3hanvsqmm.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3itrkaomx.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3oqathjmn.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3txcujatz.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3dviehacw.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3gnyutgbs.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3gussqzth.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3hqisunqw.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3tnbtweay.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3tndjbjuz.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3uvxhcdqv.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3tnswfqti.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3wjbwydyp.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3kwbcwbqe.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3lrmndzpe.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3mvgrjaxy.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3dvwiucvy.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3vvjibzdv.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3gmobzaql.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3jesaevkg.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3wgscmsbe.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3vfdcpwiv.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3pyepqmke.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3rszkwwoo.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3qvfeemuy.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3sjidmoug.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3ctmbnnnb.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3gcozqibd.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3olyqpmbu.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3ojmblyqy.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3lxfbdudd.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3czqymvvw.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3tjgnezcr.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3xdoicfwj.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3xkludbzn.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3gllcslbd.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3snzhkwsu.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3cvqtjzxw.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3rkypptds.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3aghuubpb.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ghtsfonp.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3hdijnwpg.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3tzobtzed.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3zwaxwfwx.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3eeztasyv.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3dsegmbbn.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3zhvrlswf.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3aabgphft.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3dlrzspnx.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3gilvzlix.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3fvxanxez.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3nbhcoknn.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3yrgpklar.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3povcwhxg.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3hbpmsphb.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3rftvwvhv.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3cjidqifc.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3hxwwbfem.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3rgkbcwze.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3htlgjicb.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3ojbhxuvl.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3dcfdopqi.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3pxhwebni.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3etbdzgsa.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3fgxwoopk.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3clhhfamx.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3yiebjfgs.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3gcujdtin.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3vwqzigjx.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3ssvhtimy.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3oulgwxfw.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3ypruybog.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3qvgxbdwt.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3iryxdwus.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3cjoupbmp.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3munpbytz.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3xeuyhtvy.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3ufqbfwtp.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3dvjvcnwg.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3vhhxulwe.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3ekxbecpi.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3gsfcvdar.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3jgpripmp.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3etclsonj.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3fdamqash.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3mxpmyhfp.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3gsqblnni.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3ecomvohs.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3njgsgywl.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3amyxmmeg.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3dsmqgonp.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3zacyzchr.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3zgbqthhf.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3yjdpgdwq.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3vborbkjr.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3gqkkimwh.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3bzvohbij.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3epqhdwtj.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3fpenrrlg.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3orpqffyp.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3ekvecrpz.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3qygfwhjl.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3tgyfeewo.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3osntkkhu.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3fyoqksug.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3zsjgxino.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3hwigwagy.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3mctkwixf.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3kxhmmnzi.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3nwykuhyl.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3maiwtkif.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3alqprmre.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3xqezvvok.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vszxjwgr.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3xkknkrpd.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3dwdsvapy.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3mkvtohrq.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3vevaqcyn.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3qxywuuhg.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3ogozbbkr.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3gyqzrzas.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3uayeshnx.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3peszzfis.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3mbvsnsjf.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3umvymbgx.html


<!-- 参考信息 -->