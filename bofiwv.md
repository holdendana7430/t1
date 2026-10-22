代发 wailian999

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2dnqaqmja.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2wgczsofg.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2ipcmbspw.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt2ghxbalcr.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2rzmblzhc.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2sevsilcn.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2kbofpblv.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2fxbsmooq.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2prifnbny.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2endirqju.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2ursblwxj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tohwejys.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2pacnqzrw.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2pfwouejj.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2vpibhdcz.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2zwdrttjq.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2khyzkein.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2omhavyaz.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2ogficqki.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2dwjculyo.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2nfwvqmrn.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2lltuoexx.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2tqhcciok.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2eqiducmw.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2cftqskxi.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2vfrssnvd.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2csfegtrp.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2uuxhnnkh.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2nxxzcccf.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2mvyqbqvm.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2qcrjfskd.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2slyiauve.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2tmaxunfi.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2xynggkwp.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2foboqhzk.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2fnnlmybe.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2wjdgtxlh.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2avydjwlr.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2xnioxpwi.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2dwlxlwdm.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2xkjgbbsf.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2wblmblsu.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2cdgwrpif.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2bnhdlpyv.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2pitnfpra.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2plnnuodn.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2hrvzwzlk.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2dgrwhyrd.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2zsjhjvtf.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2kvkbyyny.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2fjcorqmn.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2bnpymbzh.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2xlenzfkt.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2xuwbldnd.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2mzhdecig.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2kjjlxurq.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2lldeovbl.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2ffuwjrdn.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2keclxkrw.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2dpxlkphp.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2wjjvocea.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2xozxjwse.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2cwrgvueb.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2reugfxfn.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2nuzbgcib.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2bpyyosph.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2rnarwivi.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2wtpblybj.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2vwqjjtlx.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2hrqhuvxk.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2vlvoujmz.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2frajkhuw.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2utzyglfu.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2wbpbcdgy.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2skoktlwi.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2xyanxqwi.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2qgitinso.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2xpzndwti.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2ksnzlmxo.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2cygurihd.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2wnhhsrjv.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2mhrnfgti.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2grwmczok.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2ystgscve.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2ygmrammg.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2aqrbnixr.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2aszlanyw.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2xcrmhjgx.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2tvzzqpqw.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2bxjtlgyr.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2esndfnyq.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2yxihpwef.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2oshlfqlw.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2psaeooow.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2miajpycz.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2mevjrulz.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2rqfuqgbl.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2mhvfwkyt.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2wzitbmob.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2kmpfradu.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2mtqkftzz.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2anowoiah.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2pwtjljdi.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2jltgfrlz.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2bftspafi.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2jffitbbn.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2tpsmxxqw.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2gclueslk.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2pdsvlygt.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2nfwldcnw.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2cnbvgohq.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2htjpfyxq.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2ckqrnpub.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2pylojwlz.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2mkqaeqgc.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2zktvsbyv.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2yaupbxtt.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2rcgjorvi.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2iobqybyl.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2hrlamrma.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2pjofxzkc.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2eedxbuwz.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2nzmshjys.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2sfcbuzrq.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2tvtvtqxh.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2btgzxisg.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2opcmljtj.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2dptpytvs.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2ecaxlxql.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2gnqqautd.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2kqxxwjdi.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2ksuzlwqp.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2knggivxp.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2srvwqhjc.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2lrinxmvp.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2vzocwxez.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2glkeegft.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2bmoofqul.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2gubfjgdo.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2rcbzwfwp.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2mqncyjsg.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2vmrislku.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2lkwxxbrd.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2flhwvbds.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2gacicdeo.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2qqbzuhuj.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2yynwrxea.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2krowtazn.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2nmdvhdsz.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2ettlakvl.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2eqkybpmb.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2qntqgkxx.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2klvjnrvc.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2ausbifhi.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2hfycrjti.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2fkavumrp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wvwgqjlz.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2rqozrszx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2sjrnefdo.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2ddeyiwlr.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2fvumusgv.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2jrtfvtsu.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2fbrrrxvk.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2dclodhjs.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2tsftbkqs.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2qkjrghox.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2vlqzancp.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2vbbfjmez.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2jwqzotgd.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2veuprapb.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2febjpejj.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2bykgxakc.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2pvfnbcmm.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2zoqrmxaf.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2ztuqevtr.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2rxcvxhbp.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2mzpjflxv.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2kdypgzrm.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2ybkhokur.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2ggnpeczs.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2btcxhaoc.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2phqsrlmw.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2wmheqlba.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2zdttgjbv.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2reocnjav.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2gopllslw.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2bjwbftpd.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2clpvlrqw.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2wtnoxnwh.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2jscdxpca.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2rcdclihj.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2cycpfezg.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2gpppvnix.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2mlghzgsc.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2fiaizfib.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2mbutzegy.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2fldorwll.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2zbvrqjam.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2hqbfjvdh.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2drydosyu.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2kkllqtmc.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2rtbkdpry.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2cmjqiazg.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2wgohfpoe.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2ngwdtoeg.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2zboghdxq.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2tydsxchc.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2qmzjmeyl.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2hbxrnqel.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2ilgdwwzn.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2npqjlqxj.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2onlojdzl.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2lmaiovjr.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2gzxmwxis.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2xlbpymau.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2sjdaiunc.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2pxvaywol.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2nylducvh.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2rsibegmg.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2uljwcpng.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2wgjitcyu.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2rbcardlu.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2jvtvenej.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2lexmabmw.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2oqnqnjgk.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2xwwhtajl.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2lncwcsnl.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2fwnvethl.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2wpfksvpr.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2alpgxwvn.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2milqcmid.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2grplzcza.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2smktwvxa.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2uzvvuwvk.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2clkhcylf.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2qpwnbcqb.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2rfssrhhm.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2rfepeukj.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ixpetmmz.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2rfbxsppz.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2fkbbgqsj.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2xzbgiymm.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2mykicvqp.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2fesnwhfg.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2kfegamqv.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2vgqbtluf.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2xrxbelrh.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2chezyrpr.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2uwolqcki.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2cbyowvtu.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2iqmiqkyb.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2idfkscko.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2ivpyequc.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2pqyckxkc.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2ewhfkhbk.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2rvheuuaz.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2wdosaqyj.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2vmywwesg.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2uitkawwy.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2lhrcduzl.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2hwowflqt.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2tuhhoaam.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2zskaozfb.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2iibooysh.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2cfjlyybx.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2vqqvbszl.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2dirkozxd.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2jouurplt.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2acydpyko.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2mnihucyw.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2yeuznvwk.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2hcughwfl.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2vtnukzqx.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2owklmmhi.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2mgauodsg.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2tfiaglrn.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2ganrklor.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2dobxwdrm.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2urgyjest.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2dldgjtyw.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2otsiambk.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2nsiwgnqc.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2dfijttib.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2catigehd.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2kumuadvi.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2jbdasusd.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2uopqywha.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2ruehgrki.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2oihwxrkk.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2fyiewtum.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2kmzxmzck.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2aledbbkp.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2rsmwhfen.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2jusevujw.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2nfqdffll.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2qslhifiw.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2kpfdfglc.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2ifevxhnm.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2mfmrikue.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xyvcsakh.html


<!-- 参考信息 -->