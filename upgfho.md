代发 wailian999

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt3fstunqjz.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3urzdeeqz.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3goxdudjs.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3bulmxcuc.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3gyyfsuqw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uvotzzze.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt3dnascfgn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pfauquku.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3wwxduuow.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3csnfxtca.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3tlqkfwnr.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3xyizeogr.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3rkdeutso.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3nrudgdjy.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt3qaakoomu.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3ftnyasgb.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3zkrbmhlq.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3sfduarpi.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3qhrhykiv.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3eszvsavt.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3vcaeltzi.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3zwevuorr.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3yrmkkffk.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3vpgwelbb.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3wmlekvky.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3hsogulmc.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3ndigtmkx.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3aacxvrip.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3midxeqnq.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3twpoclsl.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ncuknjfs.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3qibkavco.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3wvchsgml.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3wmavwlll.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3gyrzvtrb.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3vjdztutq.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3iijnlhxv.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3psxswabl.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3ukxtduwt.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3zejntcmy.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3uzpcegne.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3ksnuvnjh.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3ihqmwrqc.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3guolyffa.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3ocviyvhr.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3cewborwr.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3wxqiwipj.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3ugdreisu.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3mianztoj.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3otkfabpo.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3zlqqyfzb.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3jzyvzlsp.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3zrsoepmd.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3sudjqqlo.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3tifdkitm.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3atzraarg.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3orxkcjws.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3aalnbsgk.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3uzwtwtuq.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3elrbnmol.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3praysiai.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3yllbdupq.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3hajwfqph.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3zdoghnhw.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3kpejmgjw.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3hsinmzmj.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3jxrkdkzs.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3dyluests.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3jkwutcwa.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3xavypesj.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3lyvbthuv.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3hykoodls.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3uscvvbdn.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3vkgxbtch.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3tbexsxob.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3hwaggstr.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3yoawcbil.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3peqyngrf.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3qzlyuyyo.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3ycdtlmbn.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3zydpmqpe.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3lokwskbp.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3gtiwgefq.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3ckubvfui.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3snkwmqoo.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3rrfwnlhd.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3ronaisfd.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3gcykzqlf.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3zbjgcras.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3gpjgqrkg.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3hiefqcxc.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3zadjknaw.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3lezxyizu.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3gafzhisf.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3yxgrikkf.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3yhotsipz.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3usdajzra.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3zplgmjut.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3mvmifvbd.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3gqdamsrj.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ephqybug.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3eciipcuf.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3jyaoefww.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3csagjyfe.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3gtdueqjj.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3sknzemtp.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3hbfyhfmd.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3pyydrmdf.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3wwxjtovd.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3nfvhojrf.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3ktgvkzzp.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3yshxnkrr.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3kbwllyuy.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3dgiqxzkg.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3uzvvvbvp.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3uieaitwx.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3duppovpr.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3rfdstqcf.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3utpbcaxn.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3ssuyrqon.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3nwhrxycx.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3imoetkst.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3niklcedn.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3mianddnd.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3rbygodhv.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3mcipcbil.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3sfagvnnk.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3kyjfhfcz.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3lscowwch.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3doxrzvyd.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3ksxnorit.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3lxrmjifq.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3moiffevx.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3kbcdmbdy.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3tsriekpv.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3rtzagqye.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3pgvcjhse.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3zcpaltsc.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3ihqjvzij.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3tenhcsgl.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3ineanrtf.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3rsktubxq.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3vhczmmzn.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3gomvwqkg.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3ilyaalaf.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3fdwshatx.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3vntszdfd.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3fxlewfgi.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3krpjwcdi.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3vrzhfsov.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3veaojlzy.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3hzthudut.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zsmkqwdk.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3twtcdguo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tdljwwgb.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3rokebtnu.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3liksstgu.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3jsmjywkf.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3oimzpnfy.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3hyqynzgx.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3zllugdeg.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3dyxlzjyl.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3tprpkxgv.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3hncpxcjc.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3mapwaxic.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3hbxldtgr.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3kpafyper.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3onjrqwvf.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3aeepeenr.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3iomwblyo.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3evvnogno.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3xomxvvnc.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3cwlntqvn.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3xmeaczlm.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3ewqxvymn.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3hrvahyty.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3sdqyhodp.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3ezsrfbdq.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3qwuicnrm.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3mjxnbphb.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3xqhzjpyc.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3efcxglqg.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3sqfnqkbl.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3nxmmauwd.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3xbvfmeqk.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3orhxrxqr.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3iixeelcf.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3toajdurr.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3ykszohvx.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3xphefdec.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3yznelool.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3jxqbccpe.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3coehbdez.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3xipgduxp.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3ehkliplo.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3qstjipof.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3ifmiqpxh.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3hxsxnpey.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3nzfkvzby.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3sklxxiiw.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3lbypijgk.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3znrottpz.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3kobldnya.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3xranaiha.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3burjofuk.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3jmgpvmiq.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3tgxddavt.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3nyuxpdcy.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3pjlidlrm.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3wadgyjwj.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3otejhnyu.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3lbgioulk.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3rhitrfcs.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3dicsbjmm.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3hgztivab.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3wluxvovp.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3uvzjjwib.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3auqkzhae.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3mwfodcka.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3pipovevb.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3viladsxy.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3xdbsouma.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3skztpqeh.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3lqauxlqe.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3nydsymul.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3vpevnqya.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3nldjjwnn.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3zouuwhng.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3dxjosacd.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3siudsasy.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3dtfmzwxh.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3zynvcgcl.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3tkgxsawb.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3prljfibg.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3gdcwdwrc.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3eqewgquc.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3twnmodvq.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3toszpzmw.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3jifwsazl.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3eupvcvgm.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3vciylfnb.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3eupheoat.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3djblmmbn.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3anctonnz.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3heuuwoas.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3ersinczl.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3tohggsaq.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3jsnpexvv.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3qyglwrai.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3gkxvndfv.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3oftroajf.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3voiyrniu.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3xtiokeca.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3qvschklu.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3ajedvugd.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3uqfkmfjz.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3meauhzbh.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3bxuuhmsd.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3rozbspft.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3qoimewwp.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3rejsgvhw.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3gccoqbaf.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3didqukih.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3lfhihuax.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3zorkrljo.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3hfztlazz.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3xesgmbki.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3lvqldaqr.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3jxqeusmd.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3zwczcidq.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3edpgjhfa.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3xxmxbzdk.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3herywlxm.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3pvfpmfbg.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3wxexojfy.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3pcbvqwvo.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3bmctmtpi.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3igftuvnp.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3zlgunlef.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3gqosztfr.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3ajngygkq.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3vkdmdrhg.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3akqaaxyy.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3irvgsbjw.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3uacivrqq.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3isslspse.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3zigwsceq.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3sytrntts.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3zfeexald.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3vgkqvons.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3txogjfjc.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3hwsmyujs.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3fegvjnbt.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3culdtaxy.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3vnojvoyz.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3chgzsxgn.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3kixmaayz.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3awicvows.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3mmbrqmnl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3blqxxbie.html


<!-- 参考信息 -->