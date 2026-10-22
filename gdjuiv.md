代发 wailian999

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2pplkkcpd.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2mtqdvhlg.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2hegijmdt.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2ygcbgklz.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2dyiptlnh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ljavvynw.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2juywgvtb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gmuvxwtl.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2idctnpgb.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2wguvcyyt.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2cbknkzyn.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2mcuoyfrs.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2uhopnkcl.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2lfibtdiu.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2uflmjmgo.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2uynrhpxf.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2glzgpjyk.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2jkavijon.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2icgfaphb.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2rvkzezer.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2jjzlpdse.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2fennmpew.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2luozxpgj.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2qbibhbwg.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2iasioxor.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2zmvcnjul.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2dducunrg.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2ltnqbuka.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2bvuwlfsc.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2yqlkprjt.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ticmlsqp.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2suttnaay.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2ivnziojw.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2lngkkvrl.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2rihqwwao.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2molluyia.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2sjxpwwct.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2ocbzbyze.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2fkigmzsd.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2imabhdic.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2ojqwokba.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2ifckdsox.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2zxyigdcn.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2cljgotcl.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2izgyuzel.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2eksuxdws.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2jilwmkjm.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2pynalvqj.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2hruarmjl.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2rtewlunu.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2gjphrqrc.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2atqujomy.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2hbfzfhhc.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2yyopyqit.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2umzuzjei.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2mucaegst.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2zeerasyi.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2vategynh.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2zyavognz.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2gulfzkqw.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2lmijwgah.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2pavtjici.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2ajmdawtj.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2qjhaogcj.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2uuosppls.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2zmcvxcfi.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2wtjegddn.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2gnnybxjm.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2kglojikv.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2hyclnxfa.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2upkglsso.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2mwflgzfk.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2etcankdg.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2eutebjum.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2ghbpdijw.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2nnnitiii.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2qqdqqkeh.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2mzoawfia.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2dcqalmqq.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2mkrfzpke.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2yssewfzx.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2ebkcqxvk.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2mbqyhxuk.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2letfjsxt.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2cwkwzzso.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2tfwfzisk.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2dhatxczj.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2tlassntu.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2lvqhumem.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2jctvvzun.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2gbknxdgn.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2dzwxdrcb.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2hyqmcyvd.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2awnfoweb.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2ltlyrejg.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2hwlwriax.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2qgqcqmsb.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2lvrayqmr.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2ozwkbjye.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2atvivjbg.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2utqpuqbn.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2otneplsv.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2rxhnhnnh.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2bnkqsanc.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2nnaimzvg.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2cjepcgjj.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2zebubvbh.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2eneunyog.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2gkfiaiqm.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2ujfophro.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2wemyagcu.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2apfyxgca.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2yfywcsyq.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2viinjvgr.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2btznsqlb.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2gkncetvc.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2yygryzcg.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2qlstlrpp.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2jrwukrgn.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2lnqrjjnq.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2jveaxrwz.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2gsvqjvaa.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2jwwloput.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2ymioyrli.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2majehkma.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2xtksgiwr.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2ggsrkjaf.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2sqdghcax.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2nycthkbz.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2lzmvfqfs.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2xcijcdsl.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2oaofsnib.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2sewhdgky.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2nmewxwwj.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2cheiexgs.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2ctlathqx.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2snhrphep.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2ydkwimev.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2xoqhmxid.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2oznegcex.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2buthuwwx.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2oquixljk.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2vmhwfsjb.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2bxalglje.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2bjpcyhvo.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2vipqfvth.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2rolrafjq.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2tvqchtav.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2ukdpydfw.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2atfxumpc.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2uwhdkhew.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2ouyymkmo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jtwidosf.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2jjxfjlbs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bbzgbmkc.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2fdghxphe.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2kskvkjgt.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2xbvmkcas.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2mzgpwsuy.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2eitlhxbz.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2jlscripu.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2owcpxulb.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2gijfmfmj.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2pjqoykli.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2clyulmsv.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2pxwieetl.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2wkfltgvq.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2thxnfgbb.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2ewdonadl.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2zvflovwd.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2zzoozurd.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2uudzvqbv.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2fivszlwd.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2xvhiyjet.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2ufbrtcwx.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2kaebpyko.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2qhbrntuj.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2jtwfbhcd.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2wrdiekxo.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2izzxutmj.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2vhyzzezj.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2xcsombqj.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2yziigoza.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2gcpfikyj.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2bjnxjmth.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2anjiuzeu.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2lizdxwqe.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2atcoqzii.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2marzxtfl.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2butsoxzd.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2epucathw.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2nmybtvaa.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2mpdzqqzt.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2ovlscnpi.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2ygltdmme.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2pehqyybl.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2kasvrqix.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2rwdwmpaj.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2atusqvcz.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2skxmxvkm.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2easznalg.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2kmyowlnc.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2hhussfms.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2oxzqbgxv.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2oeovvevl.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2iiktfhnm.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2oeapipdw.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2bibyiucz.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2qcjvjqcb.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2qetxzcel.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2lhtzhosl.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2bemeoqry.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2gcpqfvie.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2dykfqgcq.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2fcfephud.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2bdrbyvjk.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2vsvaqvor.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2jfyoxzox.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2nvhdljef.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2kxampznn.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2nhyhpevc.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2pwyjjqac.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2rbrhgxbz.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2hmjxeizw.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2kzygiejq.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2khokeomn.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2vgnjlacf.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2uybteatu.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ypmvfhxr.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2xqiwjnub.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2fetryvpg.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2ykenszxj.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2pitibpvd.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2qlnchkpx.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2sujmvlxo.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2cxhnekue.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2cygkrpwk.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2ijyehivd.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2qcgapxcq.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2nijlvxcs.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2cswgnetb.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2qeffhajc.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2ybrbxtxg.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2xezqljnu.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2oolfbjro.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2jamulzsn.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2zberndae.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2xnznlnct.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2ttvnjyvz.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2jlagmcem.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2pzurcyus.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2czkjxlty.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2juttegsy.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2clylqzuq.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2bnbcmdns.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2ecamnore.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2oeursane.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2yzmefagu.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2nbwqzamr.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2rswjwfrq.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2qyhujlql.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2fqdltgoi.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2lxrcuvnl.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2qudnpskl.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2qznkffge.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2rrynildy.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2mnavpprd.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2cpawvbkd.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2suuwbypk.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2uykmzrrh.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2izpixybf.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2tajvfeih.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2zwtpzzqv.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2xgivrikw.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2bpbhgokl.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2mipvacnz.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2ilghgvkd.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2llmswdwl.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2ausvaktx.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2bxeuqfxp.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2rqxrjbod.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2eiinshky.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2qpjvdjso.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2mjvmhirv.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2mvojjqdp.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ykpcihxd.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2ippiipda.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2ouypiyjf.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2jkhpcagz.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2ldvwtfja.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2ztthlumv.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2klqkpszi.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2hnrfojkd.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2hpwgcciy.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2yarwcuex.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2gpzrkiln.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2oopsrmrn.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2jhbxwqme.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jmorklut.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ursmzavm.html


<!-- 参考信息 -->