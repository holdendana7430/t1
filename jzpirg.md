代发 wailian999

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2geschoph.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2fdtqqdvt.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2hdowwenc.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2wlewyvau.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2mjetwupq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2terweeko.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2hunkhque.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ttddkftl.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2znwmfmgg.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2xmqtrcgh.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ylieqpsy.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2ehdygeuc.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2ixgjzijw.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2twlnwzgb.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2rpoinusl.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2qjimwyfi.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2zilpkaqk.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2wpavuhgl.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2tdgrhwjz.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2vrrsyhqg.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2wibdbfrr.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2xhreijoh.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2vtbmwbrj.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2wyhdqblh.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2jwqndasy.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2yhbjszbd.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2wpkvsmdr.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2hmtgxfkm.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2nykzsxvz.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2jkmopcqy.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2iuzmlveo.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2sjctraru.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2nqibmwkg.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2fpevabpv.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2fxgygtor.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2qtltoeys.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2wcagxdhf.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2luswnhpr.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2bpylotwd.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2tbalafmw.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2sygnrwrj.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2dkmtoejk.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2wslbdsuw.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2hzocsnga.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2qhhnvjbp.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2gcalqnaq.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2chmieivn.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2oqqeswxw.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2dyxgfbca.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2tsawfyze.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2jqafsbgc.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2morjwwsu.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2veyhhbgk.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2uwsayrnh.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2nxklpzkn.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2mqyfxsly.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2nhhklkcy.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2flacwwyg.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2uwgamhec.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2eiwygxtz.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2uftklnic.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2vshouqad.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2cnutxati.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2xybmghhn.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2latruklz.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2cqslknnk.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2jszfahcv.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2mgsdirjx.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2zzkbwyku.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2ymgntmqc.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2gjtdrdrv.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2mkguvsec.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2tybqjsza.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2lewtjvdn.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2vkgigmzj.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2hpemlugl.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2yioeuvsu.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2jfdnmvtf.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2cehhgbyg.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2asmtmxru.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2zzblxkkl.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2hjzjdacp.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2mghyawax.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2qdmdmgwz.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2ihzryfct.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2tvwdrqha.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2dqndqnbv.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2eubzzyem.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2moswbxtp.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2dirinryt.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2ocnoprbu.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2wbwhfixb.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2bkqdqofw.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2ekdlstsl.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2bfujgurc.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2okehuleu.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2jkkwkeri.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2jdrpjzql.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2ygopomdk.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2wyldmjsz.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2kkvdodnb.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2bbzznicc.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2mvrmwqjp.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2jjwrxdiw.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2zvezyxci.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2lsrphvqc.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2yduytjwi.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2lswntpvz.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2sgopqawi.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2apyrfvhp.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2qrpycquh.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2nhiuzxhk.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2jpgkjtvv.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2jxlhakgm.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2hemkpfxg.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2fisiscap.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2hdxjlzbx.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2sykasdei.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2rembjduu.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2jdyqgzxj.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2pbrtytbu.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2cioqediw.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2ouxxxkug.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2cmcollws.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2uzlnqkrz.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2jjfcvvvo.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2jifpnezm.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2bgrljiul.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2ogtcewda.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2vxrpxkyd.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2toffojlj.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2auewynyn.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2vltngdki.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2siltolpe.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2oolkqusj.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2rsxahguj.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2dndwfvhk.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2jmffehzb.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2pomiptqr.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2qtasvgqf.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2xxnogkrt.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2uaydtmuk.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2lhvkrvpa.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2angxvabv.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2ghdtkfka.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2dkkdxhfy.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2vtutihvy.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2ueqzcibk.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2jweyifwf.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2tpiorbvf.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2vvlvqtro.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2ajxhvtfm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2spfdyaxi.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2evbbgqdz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dpjhedwf.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2uflkrmyv.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2mzhunjjd.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2kctfauim.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2caspygpi.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2pqmfpgti.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2wbnqahch.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2ehiyhmfc.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2giikzauq.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2obqskckq.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2rznuxmic.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2nhqlgzhv.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2foshythj.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2jvzebldu.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2ypjcllmm.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2yqpyevtj.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2vwkncfkn.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2fufjckgw.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2ksilrfpz.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2iwbzrlfi.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2jspchpvc.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2eoaypukq.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2abfirktk.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2ofsjabtg.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2bqvitzyg.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2olupqyux.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2kfkbkmkk.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2wdpnigno.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2plnisppw.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2urnggqqc.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2nzeyemdk.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2fcfvntsu.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2wouhbfsq.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2unndgwmr.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2gxfohhhk.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2yckaswlr.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2wgkdwlma.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2ooenlpty.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2jgkvjzfa.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2acpfmmbj.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2atfwchry.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2umamgxqc.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2cjhslyvn.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2eawpewjp.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2fizkbivq.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2udraftpx.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2sabdlyeh.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2jjotieom.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2takthczg.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2xexlfoyo.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2ffylicct.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2yfnibgaf.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2cxlofpsh.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2xfrsbamh.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2rqpirlxt.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2dtdkzdbg.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2dsebaypn.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2qtqkmbgv.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2rcusdnwv.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2gpmryvzs.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2rnozqnog.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2xpwhfsze.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2hxycbquq.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2fadjmcpt.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2ynuqezra.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2iwlxthho.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2kcmvofgc.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2vbskawxz.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2llduyskm.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2isinaqhc.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2szlghijy.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2iaocokyv.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2aaojyvvj.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2rcajkcpc.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2ipkbuofm.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2flkmjbko.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2ipsgviqg.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2rapuxvzw.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2cczedwvc.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2plntcvrj.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2osfirkpr.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2vsklfwbu.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2bkgruaqp.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2dsziuovb.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2qaiuejls.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2wfliubrb.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2emxuohqd.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2xklgfprz.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2fuskyluu.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2leetfriy.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2kxkbqoso.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2ejlxfyje.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2hkklmeky.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2qrsskiez.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2lxnrtghb.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2kaoqcbar.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2twtjybqf.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2xrpabzup.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2fwepkyin.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2vetlmexj.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2hwrvtryq.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2neikfrgw.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2bbffztdc.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2kqfhvshs.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2aqurhjrq.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2dbcixxfi.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2pvvfytol.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2ntwshrdt.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2llfyvqxq.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2ovnrdlcx.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2zuvckcxv.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ysnkweup.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2txszzepr.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2fqhcqlju.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2goqexmvr.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2frwiwrfv.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2cmtbhmmi.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2urofvwej.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2fzbynkev.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2induubxc.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2yfknoioy.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2sxhwmysy.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2vewedtbv.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2wwmwxomu.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2qzomgmfu.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2tmyzteyr.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2yzgeyxyj.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2bsagppxk.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2uarjcvwx.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2doofrymh.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2oixqivky.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ucyddado.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2tefikbih.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2vblpxple.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2uaghpqin.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2uwbhrykv.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2anqbjalv.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2zvtqfyzx.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2zbohsjfv.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2tomqmgui.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2jctklvqe.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2flwuqmis.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2mcavidcx.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2opppetdv.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2lzmlbhib.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lkvzsnio.html


<!-- 参考信息 -->