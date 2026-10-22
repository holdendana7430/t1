代发 wailian999

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2jxnbqrwh.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2niyllper.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2yaosccgz.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2rftjnusx.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2hsbdvsii.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2hemipruw.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2thzedhmt.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2rygpwmwy.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2voqunhiv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nkrmlqpk.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2lqoaxrqe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qgizzdvw.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2jrutogbz.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2sqnnvyks.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2gkmhjcej.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2tptkfwzt.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2cetmduao.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2ntxiinyd.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2ncarbbzr.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2qhqqafmw.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2tubmsdnn.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2ziyzviaa.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2zfeyyjip.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2uxusdwat.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2hyqqvnyv.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2zyndchxr.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2ydxlmvyx.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2cebzhujz.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2wvaxavhg.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2byxhkmjj.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2cjhflmlx.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2pcqqojrp.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2sneitbkh.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2rnkkjugt.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2xvytyrgl.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2cxbiszpm.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2ebhtznqr.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2pebocvvd.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2agyehhhg.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2pxutywxu.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2xcngrkpu.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2prjlqcld.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2ukiuunht.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2vkhqavwg.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2ltktvbgi.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2lkndinpx.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2egfzoudn.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2ifdsuioh.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2kwbkwhnr.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2zondziwx.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2htqfbutx.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2jzayyqmb.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2dsprahon.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2bycfmwri.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2ojhytsfc.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2wdlxhsxn.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2fzdlaipv.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2cdgkpbbm.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2xfqmrabq.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2umfgjpmq.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2hpbtqdvi.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2yhhnyacb.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2apwqgeny.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2mcjisuoo.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2khloowpa.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2eznjmbvj.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2ltbmfipw.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2tjjaggiu.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2iuwkwxly.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2mgilljgf.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2rtcqlboz.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2enjdijyi.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2bcqchfdk.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2vvzxzrdy.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2qidjdgwk.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2smicxhgi.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2fiypztdo.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2ypcsaggc.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2mndathex.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2gburyhqd.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2bnxbeatv.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2ivnlvavx.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2mcemjoqm.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2iotdphoq.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2gyelmwlh.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2mitulpmw.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2sbhgqqiv.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2ceuqjecv.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2buptlmbp.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2rfgxfgyw.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2klrxbsqr.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2gufmjofj.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2fdrfzftt.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2xyvbfhtu.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2fcxoxrbr.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2hiqigsdr.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2stigquvg.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2yfoixppc.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2uegxennx.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2qmbcjjnv.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2zfbtvtaj.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2uqzsorqh.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2kvaodnrp.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2tojifapp.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2qjzrzgpf.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2saactwzu.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2yyjrofou.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2wfbfpdci.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2uagahkci.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2fzxidfvx.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2quwwnjfx.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2cwhtpnmi.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2mlziqdvh.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2lnlcmqds.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2ojmexyyv.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2uormyusg.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2wiugcdhc.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2dwztmujn.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2jmnuvazm.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2fdaauqqj.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2auhghhgr.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2vjxtwukj.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2itcugfsd.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2mpsqcwic.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2xrotczrq.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2sojfcxrt.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2hipolqvv.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2bxlrlfps.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2xnxexqcv.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2qavuhlow.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2jypdtzzs.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2xbzrhkex.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2eldxuruw.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2pvdiidut.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2pmoxzxdq.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2esldybkw.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2onvybulp.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2dlcozjwt.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2fnmfpoin.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2rvlddfqd.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2toexlniu.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2zqvgsasy.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2uymjcwzb.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2mqlbfqrr.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2chymhfvo.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2jbduhlyi.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2ograezsu.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2uityhjjt.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2lsshggra.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2nuengfwo.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2cwriiqgj.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2eutxwceo.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2zlnaoams.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2gekoekfx.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2guupzioz.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2eqlzoibo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mnhrbial.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2pixspdzr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ibcohpya.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2vntxjwit.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2poppidcr.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2ndaupntr.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2fxvpwkmj.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2znrxmrbc.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2ankdtbnd.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2xklsfrzc.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2cuiescyg.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2umyzeyeq.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2ncaiuswk.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2nlsdtlap.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2jzcadpky.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qmxyroyd.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2hcnypyzo.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2auwabovp.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2xogwznds.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2iudrniuq.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2mnugqsnj.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2grigcoxp.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2cowepvrk.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2invkzuzd.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2wvpdebzh.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2ifqbogra.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ngxzkewb.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2brdhytdg.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2frvscxlt.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2dhclrayw.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2ywxslxvc.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2rmshrijd.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2tubnklru.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zdrovfjd.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2zevaagrp.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2zouarwgl.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2rhalgjrg.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2lmcgvnut.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2uednoxjl.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2epxlrfxl.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2sungjyti.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2dilgqojr.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2seyedtvs.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2kvjzvleo.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2dyppvgve.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2rszxuzrk.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2tsfbvxym.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2yzvgxtzn.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2bazntnzg.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2hngygvls.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2uohiyiry.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2lnffkrxx.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2sbqloazk.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2mzgkdmtz.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2zuoielov.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2txhtwtyt.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2hrhcuhef.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2wjcxgvhc.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2vafqlufh.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2sfqomuif.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2ndopxsgu.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2dkqoexiv.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ncpgnpwp.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2rqmqvfis.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2jhphblbq.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2empwjjkw.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2gmydhfls.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2oiehdgqf.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2sjuedfgb.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2feyltcfy.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2tyehuzgg.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2hydrleak.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2ctqtntjb.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2mpuwaehf.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2eonkgwvv.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2ukinwkar.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2ntycmrjx.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2ehrhscqh.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2dslajgnf.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2xbozffol.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2aweotolf.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2edonmypw.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2flpysafc.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2whrmmrhv.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2tcjnqzqz.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2vgyeyxms.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2drxdjgzu.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2rldfbpcf.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2wtegwoex.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2sfozdogg.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2qpykaorm.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2qcwdpfed.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2ttiirigs.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2duvakxyc.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2vcbpquno.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2bhkqbuok.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2vqvnzyub.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2actwajry.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2moyjncos.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2bibysqub.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2eeebdlbn.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2bmvjslxc.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2vseedhzs.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2xnulqogw.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2zvjjhkoa.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2btmyiptu.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2aiwcpmdx.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2brvreikk.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2antspchi.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2jslysilx.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2csyujeno.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2ylsfhpyx.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2efkfkwdz.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2cyhtytks.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2qevgimaf.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ohftivzl.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2qavpumor.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2ahvrdwoi.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2omfrnazo.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2psjwksqm.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2rnaebbol.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2gjaxgnvm.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2cjrlpayd.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2gxgfigha.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2nmynwcld.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2xcdatasf.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2dqjjrylb.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2mydufhtg.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2lxxalfnh.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2oobfekew.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2lputfqjc.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2yoyfoqco.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2cqosgxqp.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jrayxhln.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2tsxqmsiq.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2mwrminut.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2oqsxqgmd.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2pjvaftea.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2fqdwbneo.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2mhhyfejd.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2oubptzmx.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2lselleby.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2kbgnkehp.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2fypfbqks.html


<!-- 参考信息 -->