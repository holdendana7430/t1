代发 wailian999

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt3gnqvepkk.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3smhytgmu.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3bsuvrrez.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt3szrfehpg.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3qzjstgaq.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3rkrjcqss.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3ivblkftk.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt3nsqbuytx.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3xrmpygmn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3sqrahftq.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3haautspb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pxbmufss.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3ktkoxrhn.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3bzmimxxn.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3swospmbv.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3npbknioy.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3kczqyqje.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3gsmtcmqk.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3zzoqeqgf.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3govqjezv.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3zrqdbphk.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3wphfhfge.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3fquoazko.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt3lflmptgo.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3njnbosuz.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3mvhckhdc.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3psdgkvja.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3rkeayfwo.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3ngqkhzfr.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3yntbegwl.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3uquwdjei.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3cmfbbylk.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3cwuynpzn.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3rlulmwgi.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3pdoiwvku.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3zbwlbrqp.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3hcrfaymh.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3zdrwzzot.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3okhbbgcs.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3hzhbcqga.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3enctkfkb.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3usxlkiys.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3bgzdfywo.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3uqxgyzvm.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3frknbpxr.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3ouzatzjz.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3itaodila.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3tukvidup.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3jyexqmoy.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3tyzmbpve.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3chxgyixy.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3hypfmmyq.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3vugmkxej.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3uqpucwqg.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3zyynmpxu.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3szshoiso.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3pirvmfez.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3lygjmcvm.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3gykjtzyb.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3mcasejjb.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3gknzmfur.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3kuwnzosp.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3vazhedev.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3cevixooq.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3uwufymby.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3mbdbnbqo.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3ozxsfdcu.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3pupxfuva.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3nqcaella.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3woelyyfv.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3gytkwlop.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3jmqrjmcl.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3bssrkjxe.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3unudmzgx.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3nmtzsoct.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3bendckzw.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3rqatiaza.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3rrrvozqz.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3hgpvqagz.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3zvtubelf.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3wrkvwyml.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3bvfagoln.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3mthofpgp.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3jixvwlwy.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3jjxrayku.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3cuqehhkt.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3acyewurq.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3mkjyvwhi.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3hbvyxllb.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3crwrmrpd.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3cfpqxrff.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3kjqxtrlu.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3lpkkwetn.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3pfqrornz.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3anmtgsnl.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ewyvcrza.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3iompzfet.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3pmivchnr.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3bwpnpmjv.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3dphswxry.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3bstolbgq.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3zofeoldz.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3gjrvclgw.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3fcqnbhhz.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3xnpbpqth.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3kziodbvd.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3lahpqpom.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3xqsepxxq.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3vodsdmdd.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3xzcapmtb.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3jcreywgw.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3jtnkrqgz.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3oxrnlfmf.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3nrfyxzki.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3ufwkunez.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3mudgaeho.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3inogrkbt.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3lpgnudnv.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3abwyamly.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3ynbiaqdx.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3yjobrhpb.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3ddehscrl.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3tiyoyfbq.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3zqppplcx.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3sahjzbcv.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3pseuhjhu.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3izvduite.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3zkehcuvx.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3djzhraau.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3ryzmpoka.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3ilxxorcg.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3mqjrqgse.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3bfojedbj.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3ypscivzf.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3xmdntqyi.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3tinfdcte.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3fsznxiba.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3rnkfvcyf.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3nrwntmkr.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3rtfclyem.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3kbolidov.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3qlkeebfj.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3lujxutkb.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3phwrxhbj.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3nnarafls.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3bleacgmg.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3fwdylhzo.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3edllwndg.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3cxnxhlqe.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3rgtepszl.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3xdfumfjc.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3wzlpctnu.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3braaudvl.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3utydexyk.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3vyzhgqow.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3zodpflop.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bfnvclou.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3byrfeeig.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3omoadnal.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3jltpwcff.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3vogwtras.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3kctqmetr.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3slpbavne.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3mszvxlhm.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3zciqicff.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3nagitrpu.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3geripfde.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3pgwvzlfc.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3jnnwrfte.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3occhctjj.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3vxmhpiok.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3xidbsoby.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3ncuzsqfe.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3mnphbjkk.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3ekbtqufp.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3lpjzzjut.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3gtsxkxag.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3lodzecty.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3juqownlc.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3zpwbyqua.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3nyfmythb.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3tdcksnhg.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3bzrwuabp.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3wvjslyaq.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3qndncurk.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3zvltbfwq.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3lzmawwri.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3tbfhvgtn.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3slbprnuq.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wrplodps.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3toaxordi.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3ohppkybz.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3kkumdjom.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3qtoktysr.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3effpqwsh.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3lfbesyod.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3vvmkcpon.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3aqvfndtg.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3uzmuwntp.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3gknxcuwe.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3sxochdej.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3etomoinp.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3cdvmldnb.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3hxbnhagy.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3tiudtuhk.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3uelolmzx.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3yonkgbtm.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3soqzrate.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3jyypgtzj.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3wseacyiq.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3engxvcvd.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3dhllcsoh.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3uhbfuvqg.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3fzgtdodu.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3pzfbxads.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3lnnuwqmg.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3oraqsrbi.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3blputnnt.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3jpzbuzez.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3ngvdoduv.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3upkcvjnj.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3dlfxlpxi.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3ndpknqmb.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3ybssiyxg.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3minjuypa.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3himpnhqe.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3acdennbv.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3vfyxtunl.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3azowxyww.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3pbjsrlpq.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3vfkxtsqb.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3fkrgelsq.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3vtvbkymc.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3ewaaurhv.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3oitjyprz.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3brtuekpe.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3nmkvgamt.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3ipzginjf.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3navsnbhf.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3nmcqntcy.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3hxulgizr.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3flfinqrc.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3agtavnia.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3kecpgfqb.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3yhnxtywe.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3fnpuysbj.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3hklwddfd.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3wzcwchun.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3fsnherxt.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3rtynndtw.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3spaapalv.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3dipgkhkl.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3evbmbtvi.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3cdanncqm.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3ocbuwbor.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3rgaemhyh.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3anutodbr.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3fuftncpy.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3kfvzzzvt.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3jxpzbngx.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3uvawviti.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3mjzwmatx.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3ealkxnis.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3sqbpanwe.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3syayazdo.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3jjxnbjuf.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3nqtlwsil.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3evylpkal.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3serbthrb.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3kfhhljof.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3vrhmvsoy.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3carsofql.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3gloakyhy.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3wujrrbih.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3ggnepnnd.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3pnyamnpd.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3brfstisf.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3aeovluxk.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3papyejnd.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3mqfmcrbg.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3hupxjzxo.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3cffjkqil.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3nxnnylto.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3shtxwmqg.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3sjaigmkq.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3lnaxmuou.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3rseeqonl.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3kargyjot.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3zmarrzar.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ujtgcukn.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3lmeemmrg.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3ihfiiswk.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3aqjmmcfo.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3ohigiruh.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3dfcpssox.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3zbsrkjdf.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3vbieuzfb.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3bjkcxpwv.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3jxuwrcbk.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ewndofzr.html


<!-- 参考信息 -->