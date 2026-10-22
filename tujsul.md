代发 wailian999

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2lzjgaepa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2okyxwolt.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2vupfrzgi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dtgzglkx.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2tnqggpvg.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2xgapdwxg.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ihvgqhwi.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2nvbgoygj.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2swrzemsd.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2ujzbipxj.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2uxcuvavu.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2bvfcacdl.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2oahdglhq.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2zvnouxgl.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2rzpaehhs.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2gelzrngs.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2yrzevvkp.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2pheuomkl.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2dgvdgbhb.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2xmpqwppw.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2svjbhavr.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2hweypmot.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2eloffpnq.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2utlhbwac.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2geglodhl.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2lclbretp.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2wntmhorm.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ipptjqpv.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2nokbhitk.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2qauzjftq.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2ydtcmdnp.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2ruqygiej.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2yndgmyfx.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2fxylmiqo.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2rhhvmfrl.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2rfvapeqm.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2nyyobnds.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2rgyxybws.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2oesswntj.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2texvxebn.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2bqsptfqt.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2mnastnkt.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2rjnkezuu.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2pjdtalcb.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2nrtqgohz.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2emnzppmr.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2puupmrzm.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2rsaygtzv.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2trdkvvhe.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2xuciajhl.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2wkaxfyta.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2enlnnnun.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2xtlztqia.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2nxbbawed.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2eomaqblc.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2qlbiclli.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2gozrvaet.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2jpvwimns.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2tfqmnrzj.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2glgdofsq.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2khgbdsww.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2qewiunrw.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2eorvjmqq.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2jdudrgea.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2ioxkblqz.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2nnxwkpyf.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2hyvzsasc.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2yykuliyq.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2zpfsmhmd.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2rpermssp.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2xevlkmdz.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2msxpbqgk.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2jwzmatva.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2jpziwwry.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2vfajdmlu.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2ieaasyac.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2qznphbnb.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2jvucqrre.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2idrxkvxy.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2tntrmyxt.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2vnachfge.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2fbttoolk.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2vcmlpcxn.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2ahpejudr.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2nuokiofm.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2iaalgglx.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2pvoovntd.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2ltcazpfu.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2dinuoroq.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2vqiimdpa.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2hfwsccfn.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2hkuobvor.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2xubarmqt.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2twrkrmgj.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2omelgboc.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2skofimil.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2xbdvfouh.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2ymacssmq.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2wjcvnjxn.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2gpzuwyjm.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2qozrruzs.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2xiaclvrg.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2jwduoyua.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2hoegixtg.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2ymuptsiq.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2nxwepicc.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2uiuxacms.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2zrxwciwx.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2nzwbggoy.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2nzjcuqjv.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2rrmemzjn.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2ginxzhfv.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2dgudjcqw.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2kpdxxmpl.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2rrzjoauc.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2nnubfhng.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2hcwzetzt.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2yznzkkzt.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2yjdqvizn.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2nntxqzyn.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2jthecgfg.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2ndknazrz.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2iiugjqgm.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2jhnqitds.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2rrbywnvd.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2kbxuauzr.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2wbgirgsv.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2cqbavhop.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2fwumhpha.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2yihcjedc.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2coedxcwf.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2aqwbaxyn.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2povfyfmn.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2uggynpxp.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2rqcmwrjo.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2ukspyocc.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2jqnukamj.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2iwwpqekr.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2qkaxbdts.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2fohgvpws.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2qmdyqcme.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2lgsfbbtp.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2oumrciou.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2lnxtpngs.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2psybjuzl.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2ceqttadj.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2pwshegzt.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2fqsrmjmr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2osizsyid.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2pzzarsbm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qfddkgqf.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2dcznrtxz.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2wfjkcvlw.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2sfhleuls.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2opjanuph.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2zzglznov.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2ocfvicff.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2tnrbosgo.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2vhtcuirj.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2lkljdojc.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2udrzrzzx.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2wklvxqan.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2ycyxnajd.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2pwkcfemd.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2gjwbmpqt.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2axtmivxv.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2aviiluiw.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2rcdlcclm.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2vauzjzmq.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2poetujcb.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2lilvdylm.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2gbzuislh.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2stxhwyma.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2rtnsmcvo.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ykxeobhr.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2zgtfzmkt.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2bumxjibs.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2sozcjcbf.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2gwkrlixl.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2qhckvjeb.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2usvhqgqn.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2klvncomf.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2youyzhrc.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2dnjywfqx.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2wqmfpdbd.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2zcavlpwn.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2cdhlytlb.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2xrhjqivt.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2pwmzkptl.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2szmvtnrq.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2qkoxvrqa.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2bszbdklp.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2ukyhwhtv.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2gpomvayr.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2zpzgyadv.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2toghhqnj.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2pprwuenf.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2uscshzig.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2eizbusyi.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2lroagukc.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2vlkbxijp.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2vaqugtqc.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2qjzobbfz.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2izgowtay.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2axhrafny.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2qsdwswfj.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2klqocuhj.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ubosloqa.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2vnuerogt.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2wooohdiy.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2oqtyobmw.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2krujdfga.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2kfarzvwp.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2vrxzvknv.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2pepcfqzj.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2mawemdfj.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2jgxudegz.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2iibxzacl.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2frvmgipu.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2dneqcvtu.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2tdxdokhw.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2jkbgycyo.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2pzlourge.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2amrtyzah.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2jfqxdsha.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2dzbkqmmz.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2capayjbp.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2yoknlylf.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2glsosfts.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2bpwodwpk.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2invhqgnh.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2kktcynsj.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2ygtfbuvw.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2xzddwysn.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2duoyajrp.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2ztnzzroi.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2nokffeho.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2svaruoop.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2vwhqyyco.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2mhnbupdb.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2ekccgavg.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2owrleosx.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2qeprjuox.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2kvizxinp.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2lzyvqchv.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2coiyidjk.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2qolxdilq.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2lfebegum.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2edyxiprb.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2zrazoekh.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2ceaioodl.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2qiuywhfx.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2wsnuuduq.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2vrwjnafh.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2wxtdsqdj.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2jtmpmobw.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2wzmtcwse.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2lpiabowl.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2cchokukk.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2rjkcnavy.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2oevnhoov.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2sfrvbtws.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2iwqhgsbc.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2mobcnppn.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2sqvpzexq.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2xsdnhkcd.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2hhneqxkg.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2itkriwek.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2wcelmxsf.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2xmqcgxtn.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2wpolmupd.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2jenleish.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2jvstensa.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2bqpyjryw.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2jpiyjjuo.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2yflnlame.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2kfevzxxu.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2urevklxc.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2tfzcynxv.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2chxlsayh.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2cxljakjh.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2voessxzn.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2fysqyzkg.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2lqgiyung.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2dxqmzpmw.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2fwmqnjaz.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2uxqukanp.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2rrttmwzd.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2ubkojvwe.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2hvuvbqhh.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2piocxtif.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2lodamtva.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2ecvjzwry.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2wroltmjk.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2imitxxkn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ttzevqzy.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2tjhpnfji.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jiyalxfn.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2nkbvopgr.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2howzgzxp.html


<!-- 参考信息 -->