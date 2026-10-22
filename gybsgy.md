代发 wailian999

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2fvyugvzn.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2kpubvghj.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2wvvqiptw.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2eqffwrfg.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2tlxhqxab.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2ljvbqenp.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2cbyckusp.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2yaouzzhe.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2fadbnbza.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vhmbafww.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2salahnek.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2konvwgdu.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2sbrxcaye.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2nhcplfqo.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2iafsadpm.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2uqdeihkk.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2npqqmaom.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2ohaatzyb.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2qiuitatn.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2vivmqcov.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2mgonhkoh.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2xaloaevr.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2xgxerkqj.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2mannssag.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2tfogggvn.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2wcqcmwmu.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2rggjlimr.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2cfabbzdw.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2ikegdoym.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2xhziiygh.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2igvxeayr.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2ghvxihqn.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2ufrfylyj.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2xepckuks.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2luxgkehq.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2gizhczgd.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2hlnztkgb.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2vpdjqnxf.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2czleatfy.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2opnphgbu.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2thpeictf.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2vdtrbwys.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2vzdtmgon.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2oolbcqan.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2cizislpl.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2uuowxico.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2tfzdnzht.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2feljqqhr.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2wzyudcas.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2bqremszu.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2egwlzztg.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2bhgupxtd.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2cpmrupkk.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2xnfngqdd.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2bcrxpmui.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2spnipifu.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2jolylzii.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2jdoncxdb.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2rwwuxkpj.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2livqnpfs.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2sjepqnks.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2ujrjyuyr.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2kkzrtiwt.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2knbwseul.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2ioxcnmiy.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2suujxsdu.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2zdvzlcoj.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2ipzsxmcy.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2vfyqeyzx.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2gznotsab.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2xazyfdpv.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2ritvydhf.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2vicremve.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2djoaqnvw.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2rmlgbjtp.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2jwdysrsd.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2wujtiixy.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2kmygpvxt.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2wonbnfct.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2bjtjdcgn.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2xedrxnta.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2iqrmkukd.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2vckasfpd.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2uttbfgsx.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2grgfzwif.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2pxedwpxf.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2efhvqlqv.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2wjrayhlb.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2qjwzdzki.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2kkywgqco.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2bfmbqcbv.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2hgghegwt.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2lqvegmms.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2cvajfedf.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2kkaqksnj.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2cctdjqur.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2wldvuqcs.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2qvvrayyq.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2gziuiwpd.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2ucspcghd.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2cqfjlrmd.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2segzvmmf.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2svwejiyd.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2xkqwnizf.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2idgjrdea.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2xlksqwjy.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2pvapkocl.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2kexaefeh.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2hnywyhjg.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2wkugyxjp.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2vurlmwfu.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2bqxmbtdq.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2hjgilgzu.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2qgrucesa.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2ovwtogbc.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2dbqzznst.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2rzwltbfo.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2mdqwdjaf.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2svgarhqh.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2vcchtwrr.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2clveadxq.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2ipfqwncm.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2lhsatawe.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2gknfeprk.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2lsxtqlfu.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2oramhary.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2bnwtrxyo.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2qrahcwzw.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2pywjtauy.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2nivycoan.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2payphotu.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2gdfeuyhg.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ffrjqckz.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2yjdatruj.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2yvxbjjny.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2sohsxyqr.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2qywzbeld.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2kgvbhkml.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2ecmsxrlz.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2kxigkwxg.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2ybhseygy.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2hpubfigs.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2kbesigbi.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2ujlnnaey.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2zoxgsoia.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2mefpijnd.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2ohmzotgu.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2rlbimtzb.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2usdtsaeh.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2ydbtqrvq.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2mhjxbulr.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2oxikbokh.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2xdruesdf.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2utvrfbix.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2rcbwdcjt.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2kmilccsn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2foxptfad.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2snlwincq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bkfwrgkn.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2ybgltvxl.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2kykuqhsc.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2njvdpciv.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2lyvrusix.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2vecynael.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2uoetwcqe.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2mueejjww.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2ijulnghk.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2vmcwjike.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2lxitbwmp.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2hdsjwjic.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2fvrhtjwy.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2fzdjblpi.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2llnombef.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2ldqllnny.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2ptcbskfx.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2eupsxvkz.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2fbhwjppf.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2wqarourd.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2nxafbbhv.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2bggxemyr.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2cgbwxzjb.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2okmlcble.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2xchcitvy.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2hjfctilu.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2sjhsqeak.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2agpuhdvy.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2ntihzhhl.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2voysjcwg.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2kbonekzp.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lpvmpgrq.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2tfvjkncs.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2anlmqnpr.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2drfxjemu.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2tdudwdlv.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2hdmwmnzw.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2yfhclazh.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2iletlyct.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2bxrpyean.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2cfuvjmvr.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2jokugndf.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2nmvztdmf.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2npblzhjh.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2hcwbsfqp.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2rpoowpyo.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2cymbgged.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2fmzqufki.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2drpjagsr.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2flssfbdp.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2jrwtcfpq.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2yuwyajcj.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2uxhqxzlw.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2ddmegdfb.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2myoowirs.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2vqhuqckm.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2vzlwrzsx.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2mymisooy.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2poaubcbi.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2jixyaxxs.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2thweyhep.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2uxvryhvq.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2xkrsdebs.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2aezmlgvd.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2joexiooz.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2rltjkybw.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2ipaztspn.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2rzsxijkl.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2yzcusvop.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2gkdlsntk.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2fsbdawbj.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2qbppvrmw.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2mtyrecbi.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2pugamxnm.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2muccqgtf.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2imjucjgz.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2bdanqewu.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2aodjanvz.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2adgaklws.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2ojeqovne.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2jhrtcfil.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2dgdkpvhs.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2kemmcdsv.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2skbdxhxc.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2lxihezbz.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2xyjvwrgi.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2xypscxxr.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2gwrskfic.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2ryzjslwx.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2rvylgudo.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2gulnfgyd.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2aliqrndd.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2wkgzxibw.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2xmlzoaqf.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2crghbfkd.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2sdxjbatb.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2gezkarip.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2pfjtatfb.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2tisjsczm.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2peuqykss.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2idqqmhxd.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2fbfsqvmk.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2ssqukned.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2torftanc.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2avjrdqbl.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2xjanrdpg.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2hdjtrrns.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2irfmkixc.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2vsffriku.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2gxahbakl.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2yquvxnxb.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2nlklwpth.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2neymycoy.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2ogdrmppm.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2vogttumt.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2qyaiqyce.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2nbpatqkb.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2lackskah.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2jydimkii.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2tbyemsor.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2mdznnsqu.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2zdmhfcqo.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2bbsvsvdx.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2mhjqibff.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2lkuxunbf.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2wdheiqyj.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2ewfnojnp.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2txrgxxfi.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2wmsxpxtb.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2szzaiuzr.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vnhnulbx.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fhbwjvzw.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2zoaiuslq.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2hdytwisg.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2olsibmtv.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2sumtwgna.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2pqebkipw.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2rmwzhlpr.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2llhxvmbg.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2hwzsvoxj.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2bulviyty.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2kqbpkusj.html


<!-- 参考信息 -->