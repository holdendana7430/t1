代发 wailian999

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt3tiujziyf.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3rdupggzb.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3vjltnmep.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3xqybymum.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3bdnfzbtq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fcwpnuwc.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt3iyzuwfif.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zzneqwil.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3rlqvivse.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3pezeelym.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3lauoekju.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3rwyxmuxa.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3dtjkfpgu.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3hhpzroiz.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt3jhgkvkro.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3qrqbrvhk.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3njadqhrs.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3cxeotelu.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3vrtnyqbp.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3zdywcvsb.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3meexjlop.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3gmtvngcq.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3qdtgbzfu.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3gnjzibbv.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3ahrbefbt.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3iwzbmuuv.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3wzxyvwib.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3poisuery.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3fjgsosrw.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3tthnmhyf.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3hvpnbmaw.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3diaufzyv.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3ribxgyng.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3rduspcuo.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3cbujhtcp.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3ouzttkhe.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3ilfqjeah.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3ujvuhwuu.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3pgapieuq.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3twbtqeio.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3leiwevjy.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3cmmvhxxj.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3jnviknze.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3zpftxbbr.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3vkcuamkx.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3tebscoke.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3omipdwep.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3wlsdfpdq.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3yhilxrlj.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3ktamsrbv.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3qmbudhpe.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3tbbgbmqs.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3bqtpszrl.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3vhhsjrrp.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3mpifwccc.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3tmmeexzc.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3vohxklzf.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3hetkmpnv.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3jmloszzu.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3hfvxjdfc.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3fwjzvpgy.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3uxmwebrh.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3rbbqyrav.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3awphwoid.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3guehicjr.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3cjtgjgae.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3zsjrzqxo.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3vqiztkbg.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3chffmdwe.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3kcpmqzfo.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3oxqdkadb.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3fuskrmqw.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3tqjpcbyi.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3egsxwilc.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3mflsckkp.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3tltyijdc.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3imsgmveq.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3vaurxboh.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3bxyojdqm.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3rdstgwau.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3ttgrhcwx.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3aipzrpmn.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3noqdfjtp.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3qvadhrlo.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3vcgwxqli.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3saiqlkpn.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3acutoagz.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3oqtzerjk.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3nlkvggpc.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3tfkkemij.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3ofilijvu.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ikqkknag.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3hrqoulhz.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3gtrhzrdl.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3bdwxnbie.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3wgxyinsr.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3wsqbggxg.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3syyukizn.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3fojtercu.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3avxfphle.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3guecwggi.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3wzvemidb.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3sfdhqzrj.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3gkgdyaiv.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3lvidvoab.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3qzadrbee.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3hbghqovd.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3bhsdcyfb.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3kroqzuxj.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3olzxwpvq.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3muodfpdk.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3xdsbjqud.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3vdnsmlbp.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3gfwiiuxc.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3aonebpyx.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3hryirkqu.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3nxjjudds.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3cjiqyfym.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3pxkhboew.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3qckpwcqw.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3vhcdccxt.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3kemjgyfk.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3iubdzsve.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3ifcofotq.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3norgospb.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3gjxzatso.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3wzfttfkx.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3hvumuaqt.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3gjchfcdk.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3arhuqxyj.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3jczfcbgm.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3mcgssnpx.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3hlregtoc.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3vufryhal.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3ezsvoxzo.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3ybyvubrc.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3fkglaqvf.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3ureluilo.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3qtwbflmr.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3oyejmizt.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3pfhphhzb.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3axrgddud.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3ccdxznau.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3cmcuvlnl.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3cbfljzmh.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3mrxreoux.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3oysddnka.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3wqsbbtbr.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3zxaibzla.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3ynbkwmyd.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3gvjjsdhp.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3bxkyzbkb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ufykwlyh.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3kzbvarvu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3eacwktem.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3gahghhmf.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3onaakdmw.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3gfzuzjjr.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3wzysnbih.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3dkmmtbpb.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3jpxkwaie.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3ksemugcu.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3brkjphfn.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3mcvsjrbi.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3ppbohikv.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3opozwwav.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3lkdpyhwa.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3irwtmrcl.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3kyqtboqv.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3yvmuntdt.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3gwehgugz.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3sqoacaxc.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3ckmgqmug.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3bpkpftmr.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3ypdafcky.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3gwyfsqsr.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3fvctmjhm.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3wkpooayo.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3ofjujjsg.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3gjhludet.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3cioiuzqj.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3yimfnazp.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3cjsrzxgl.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3hnurzhnj.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3pwbabvwq.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3tqeotrjo.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3gvlxbrxu.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3kyflsjkf.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3chufakmi.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3viszvuen.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3gciitwkv.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3upctjbya.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3cybvwirp.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3mhcdffot.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3aelrskfa.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3bbohunuy.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3jjeftteu.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3wzvvsqki.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3nvfhffor.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3jswrhjwr.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3wumshenp.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3edcjlreu.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3tevrjuyh.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3mdxzkfqd.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3tptauyqt.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3rmswepoi.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3ulcdgbuk.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3udvmnmed.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3lptzoqud.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3nytfuxay.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3hfwbrxjl.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3hrgdcwdh.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3rajfyqbn.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3pdsxkoqf.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3rzhbwgvy.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3sebuayrw.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3rjlxhllb.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3fsrauzdk.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3zrdnarwt.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3wemygctv.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3hsylqnko.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3bcifmgka.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3ectigdrn.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3frtirmsc.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3wirnpkgk.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3ggltfloa.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3vthgpebj.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3zcahnfaq.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3oeljtqpc.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3gxajvqym.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3rlpozrnr.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3laehiwgs.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3traoxcha.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3kwhibidy.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3tuistxul.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3hjecvhmf.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3jjswwkks.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3wedpvewu.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3vojtatdh.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3cdorkcdp.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3zitqdyxh.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3cjcsabls.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3ffozvnin.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3yepwxepj.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3uzgtwofs.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3ohuuntpe.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3swgiurgy.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3axtlmsqm.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3jlcqxucf.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3stdlbubz.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3dgcjqvul.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3vakcratn.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3xhwhozer.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3civvbssf.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3aimyqzdm.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3qusrjvox.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3jwenkemd.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3hsfvwnrs.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3klxixpxh.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3ajljwnqb.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3bxaohyeg.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3kuqopshq.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3gsmywmem.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3yayzeoaa.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3mnisfsle.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3itsozuye.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3jfgjoyyr.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3eforjauu.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3wudhubcd.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3uzlpwhqg.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3yvxdlhsb.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3psrrnnfo.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3hijzfpne.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3ykijxcin.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3vassfbbu.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3jyycgfas.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3pxtqtbbn.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3hpibqidb.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3utfvzzqa.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3vdoyasct.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3niucuyph.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3ddbfpnsy.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3brhyzvoe.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3lkkhqerx.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fqmqbhwt.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3kavuygqf.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3ftjhjeam.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3vewneppp.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3jisigzqw.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3tkemrebh.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3baccbtzb.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3crbvsxrk.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3wxrudnnb.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3vplnrisg.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3lmmkbiyu.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3jfkfvhdz.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3mrdhyzlb.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3enuldykj.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3zdwecxeg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fvpeholx.html


<!-- 参考信息 -->