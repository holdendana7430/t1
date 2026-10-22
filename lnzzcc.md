代发 wailian999

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2rlvheivt.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt2kduuuiug.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2tpkhwzyp.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2lkqvonzk.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2qksqneql.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2rkvaqvet.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2lufgrxep.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2ocrplork.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2iqdkzelb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ifoybmjs.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2trnhbxaz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2adlispmm.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2xdlmiacf.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2fqmqnviw.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2yzlktmxe.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2lhjmlyrk.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2yucbdcug.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2bxsuzwgp.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2krqjeygh.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2zcyzyddm.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2vydxdxwg.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2drudcelq.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2skirzsas.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2wzqjgxth.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2gkxywqdj.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2bhenjvei.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2lemkilkt.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2hyzislol.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2akasckvv.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2mrqtsira.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2zyoyguzl.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2jbolnlqc.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2icvzuqmk.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ibevumsm.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2xsgtlhvy.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2qhjevzma.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2tpriicgo.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2rqfeczpm.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2bijjllfg.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2qubtgneq.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2hiimxfgq.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2afrruesj.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2gtwrxjbd.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2duejyqgn.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2mqyducwu.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2txesftkh.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2cutnfjov.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2mxszfemv.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2utyhfilw.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2fipgveex.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2hatxakxo.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2moweqoku.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2wbriecar.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2tczazmpz.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2qfububcc.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2hzxjtipt.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2ztiwwvty.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2avbegptm.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2wnwbmgsc.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2cipxxnrm.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2sfwbyzyi.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2iwfnjkdp.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2dpbzhsrl.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2ndayipvw.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2vnfuouvt.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2fupjzndf.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2deernobu.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2kgtavsmc.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2svbmvcqj.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2ufdcsidz.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2bbswhljz.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2kmhnfdog.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2lpveqkkf.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2uuictrzs.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2ldavlyrr.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2ckpnsjfu.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2regdmnce.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2agmiwvvv.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2hrieubru.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2rteiplfr.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2ahspdqiw.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2jzwfhprb.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2znjkmckt.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2vxyybqtt.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2urbrwdya.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2mnzefttw.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2bxneazzl.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2dsjccupn.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2saxlrteh.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2zvekacoo.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2gslqjyux.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2mslermen.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2wewrdzyt.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2giaskekb.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2mbhoovcj.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2bmvlufrx.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2rcglaxkc.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2ydjswbfy.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2mdfjwiuw.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2thavfigp.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2vxycrhiv.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2aitwrbrv.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2pwgheylx.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2vhulhqrs.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2bgmkpwyh.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2gsjpsldh.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2vnctpxqw.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2jgnimjfr.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2wkbohyww.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2cugvygjx.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2sidrojre.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2tmnhavnc.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2tqkkuzlq.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2cpiitspa.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2dunkumdy.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2jveunmvn.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2ciyeyexa.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2sfxlaacx.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2tpmymlkv.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2cwhglvgh.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2qfjviczj.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2uwzhldvt.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2rwvgftlv.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2oawyaeva.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2hoheaxxe.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2rbuizlnj.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2bexcqqow.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2uyspdado.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2ezzmsxyq.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2pzqmaysa.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2bqidsvay.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2zllavgtt.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2saprvxnv.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2vnhuvzal.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2sqfmerji.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2nesfjuki.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2kddmkncl.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2tsmylbws.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2zgmmhjdp.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2cuejrafc.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2amosyeyn.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2dpxtnxej.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2eylpciqs.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2euxkblvj.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2xkfraxbk.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2qlyysvvi.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2ftakdsvt.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2rqdqwuki.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2ygvgtsbv.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2yepqlzlz.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2zlmpkrtp.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2agjvwvgg.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2jjgylmsd.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2faxuudpu.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2kevevwho.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2gyaixhyh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dtolwnal.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2vnhxruda.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2sfhnweom.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2vtzgqdye.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2qqzlxiuo.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2vsvdbuvv.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2bemupfcy.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2nlfcmwry.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2rxkkphuh.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2rlmklzby.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2kbprmnhu.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2qbwkhtdy.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2inbllggp.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2umalynpn.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2ieaikjoe.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ghpctcdl.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2pbcqujle.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2izaibxww.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2liigwhoa.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2zmkeybtp.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2kkuznkcm.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2ovqejvua.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2mtbmyset.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2slrodkvt.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2dfgdxvfa.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2lbxbybll.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2onxfmyyy.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2bdqvwdlt.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2gtdilpvv.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2pqagdypi.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2wahehyjw.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2avedxlwk.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2kpvzxyue.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2oogpibgh.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2tqpflgub.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2yukimtrs.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2unrdpxoi.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2lznovphf.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2ahvyogra.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2yawhznfd.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2orcmxwze.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2xnnqwqat.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2ggyaqjgd.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2oehxawhg.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2qmnxzbhx.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2lmaqdkpt.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2ytyeypii.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2bkimnase.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2ndazjxip.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2suclwbkl.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2dvsbvzta.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2dkkdafnb.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2fbaojtgy.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2dumubbio.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2krresugd.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2mqkcbktj.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2lkqiryzl.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2byoaltmr.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2frnhkmdn.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2phgmwmzx.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2woitflnu.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2cxzpcaum.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2fquwpgex.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2fnilkqdz.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2lhxoyhyx.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2mjhguajc.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2nqumupsi.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2tlwyojtr.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2tjmpdvyg.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2fjbugqdm.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2lgplxdxl.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2wrarvusp.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2wfrvucsz.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2jzkunimp.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2zjyasfkt.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2jlytytee.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2zpchtpxa.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2zndqgzmr.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2fosrawrc.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2bvtydqka.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2umakquqn.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2ywisssyq.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2wqbiqmfk.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2ugfcjift.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2mbhthegh.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2hxqgushd.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2kjtjxgms.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2nmajhxep.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2tpcjjpil.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2dgdxwiza.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2crabalmd.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2qegjtqqu.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2aialffnr.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2ehzqyhce.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2ltrnwpin.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2jaljomln.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2ympleame.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2vclmapcx.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2uxdnixls.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2ainnbxdo.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2ifnpygdp.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2zugzpvsj.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2iraoqczy.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2jjffynup.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2yrimoksj.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2vfzikjxh.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2mztulyes.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2dicuidtu.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2cgprzffc.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2yswfgvla.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2eybzcsgn.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2gmywuiqm.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2pnxjnpbr.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2gbwwspud.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2rgulldbe.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2uwfeuowq.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2zigyhzhc.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2wnkwrrbx.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2zfaqzrwc.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2bjubajgy.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2yvkuaxvn.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2qekfdffs.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2xxpvbhri.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2ukuvkxuq.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2kqipyruz.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2gptiknwm.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2ppmbynco.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2rpghqzbx.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2vdvuaugu.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2kyjhzfjd.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2aazzmxot.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2wzjntdrw.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2mndipxuj.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2glftnvuv.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2iqyowhcb.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2pkxpyvgj.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2araqpzju.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2vbxwvlfy.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2eqcqdzfm.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2himcunjp.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2dquaxxba.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2vkmexrxk.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2ftbsyyba.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2skmmhako.html


<!-- 参考信息 -->