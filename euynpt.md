代发 wailian999

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2vaezwqcr.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2zsugufqn.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2glemhwrh.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2fopjkgzr.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2mqurbugz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2iapqugaf.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2lsgdnvda.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wwaceskl.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2xzunmkcf.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2zaeotggv.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2ywfcuhrg.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2cerwuris.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2nbwdkllr.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2kdtrqjuv.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2grfjvumi.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2hsyvkzws.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2qsmooxpi.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2huukgokk.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2bopukcpl.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2dcumpqfg.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2lypyzvbl.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2hovafihb.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2gtqhtvux.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2nzdwuilv.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2wvtxqacl.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2moobkyvs.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2jhkmdckq.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2phktiewn.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2sfazntkj.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2xevzzizl.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2xcrilvhz.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2xgcnzhsc.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2brlpyecd.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2jdhaudol.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2nymfodtx.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2dezeiikn.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2nvgoeths.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2boqjzdxx.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2evljadxu.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2ycwkwrgw.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2lfbixrpl.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2cecdjonu.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2zirxxoaz.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2mcschsxc.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2axmzfpwu.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2qseftbzy.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2dnnjhypo.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2tjjnwptl.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2oigpgukk.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2bqqsqdiz.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2bvqfliht.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2dirpuwzm.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2zcfggcld.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2uoajpzru.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2mdxwaykq.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2svzwjwrg.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2npbanbsw.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2gmnbncgx.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2gysvosxh.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2yuubwvud.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2rrgjnrav.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2kynsgvmr.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2ylmlbywn.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2amhmenox.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2jxhfaptj.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2seesntme.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2gjpwvksi.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2hkoidypg.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2dharpxfi.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2tomuulsi.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2lpvjgbno.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2rwokniid.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2vlkidzru.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2gknujcgh.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2lgmimgph.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2mlysdqps.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2jjyhvnon.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2dhhyzvge.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2ffdtevgg.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2hzpvnmle.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2reqjyqsa.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2wwmrjtnh.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2ufgbivol.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2tkddhsuy.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2ydievmwf.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2bbpvqxbc.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2fwiqjlxj.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2omyldfak.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2fzzwpzho.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2twdseyxv.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2ofjdgneu.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2dfozzxio.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2whebgbrt.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2raecrdhs.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2bsatscco.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2gysplbxc.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2kisuhoiq.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2oouxyzje.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2ijhshdyi.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2uldgfssz.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2ylkbcbci.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2fgvpiejx.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2gfjqjsal.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2wgimmnnl.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2kqzyxdfz.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2tomtjbgu.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2tjnihgfh.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2ktdbhmqj.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2zaucyylo.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2uksjxspr.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2ftbuumpt.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2ivaznjol.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2nhmjyzee.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2vaiftinf.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2mzcdilzf.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2ntqdbvoy.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2mjecomjq.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2ornhcmfu.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2nlajjrwd.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2qdotqbju.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2iukktmla.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2oiyihtll.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2yecjuswk.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2hdxkybtc.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2rsarqqul.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2abopjbmb.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2fouxxwue.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2ccjtisro.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2gqjltlmp.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ucbaarmo.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2pjdxmxhw.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2kvxdratq.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2lpremztj.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2pdvsnfsl.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2dljgeejg.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2icqqtilp.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2uysctbfh.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2fvgxqbqr.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2mnbiannh.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2unppnuzg.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2cjzrzkos.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2wnuirhlr.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2adgpjofs.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2qiidymwn.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2ongnjcxo.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2ocyqruol.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2cyamkklb.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2ptgtubib.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2jldsgfga.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2hqjeluoq.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2oflimkya.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2xrdcblof.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fnnotsie.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2oxjxzdew.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2azloiqbq.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2hhdapegy.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2urqreuua.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ilprvcbi.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2wvlmrcpl.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2eclaegvb.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2tboshqvf.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2wgfjucae.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2ufxpfruf.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2yzyyuajd.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2nkykjzay.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2vykqxwrm.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2xnxueqcn.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2eyambnre.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xijomrqu.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2dvtsafyi.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2kovqkfne.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2ssxvxmsd.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2knxglrqm.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2jhtxsgwr.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2ijlgwwsu.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2scxmkxgx.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2vkhipvif.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2pgnxgizj.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2zoncoawl.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2geualvgc.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2tcyekgvx.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2iczmzkau.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2ibanujrf.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2xpjxoxkt.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2mdemlwqo.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2bogjospu.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2gzexkkfx.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2nuslldgj.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2opvyvjrr.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2joeqtzig.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2okbtfmxt.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2bibivtaq.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2oxwwhzrk.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2soneszvr.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2gkwxfxub.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2ocyhstnx.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2jozgjvpm.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2lsbqexdz.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2jrfvfysq.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2sgxiktdc.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2chfeelkt.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2pjwnxrrd.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2mpmoinak.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2wovogfps.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2hfddthub.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2spkyoxqu.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2ujcrhkbl.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2aaywucxg.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2bitpwzge.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2lqmgmmdz.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2setkozdf.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2dzijlbkc.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2jawyogkv.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2cyonaeuy.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2zwlsitpn.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2ocrjjovd.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2xhakeiwz.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2ykmfbjcf.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2oitbyktg.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2wtdcvhbt.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2mqehgvgu.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2ynlqerqv.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2jftsyzwp.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2gxlzbjyl.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2vshmkmtj.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2sywiscac.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2rsuxcuve.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2zqoltanj.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2htuqgdjh.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2atrxzrrk.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2urxnxlcg.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2ygmxzkze.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2nfewbcvc.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2vxqkowqz.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2pdoofofw.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2pykihkit.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2jgfklecy.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2offmuqxh.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2gmwvtcif.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2rgnodxzb.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2qvyayfrz.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2enjwrkok.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2ypskjkor.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2jacjdvys.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2vdfztjvp.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2xxwxbsnw.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2covbspqz.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2otpwihjb.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2yukfcllq.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2atgujbxj.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2dhxtmygm.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2pdomsdmo.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2wkakwhbn.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2nqsnhtbc.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2xwrtlnlk.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2tfgyflgk.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2iednlgpm.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2kmgxedxd.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2elyiohnl.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2yaufezyv.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2dulgjmmg.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2ybnaguwf.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2rtffyqyl.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2mblnmpxf.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2ieryszaa.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2efolfifx.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2oynejvdm.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2zhelhdba.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2ajohnhjl.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2adbemhba.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2fkjujgmj.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2xmbvgkba.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2cyopdcfw.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2rbhtttyt.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2svqwrede.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2wftiyfej.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2ogbzhlbf.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2qngrgsmk.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2bbphngsv.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2uuetdace.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2nlqaojno.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2xbmgpyqn.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2xbafmsdh.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2isqaczxl.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2bizqmvce.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2zzuukgfq.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2tnxyxytb.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2suepdlrj.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2fjtsbmgj.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2emwaunvf.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2yxtcomqm.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2axtvsfdw.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2hytgsttn.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2attqdhck.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2cytvbeoj.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2ermwrqyu.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2hhmpofdq.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2ikcabbuh.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2mhlnpdpa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zyctnvhn.html


<!-- 参考信息 -->