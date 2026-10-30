代发 wailian999

TS:   Number() String() Boolean() x as number
来源：http://m.share.hesvh.cn/Article/details/gofierfms.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.share.fehbvm.com/Article/details/gullmmbvd.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.m.share.hesvh.cn/Article/details/gvmdalkwl.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://mobile.zdbjq.cn/Article/details/gdgcndmcj.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://wap.hesvh.cn/Article/details/ggwokwiow.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gfaxnznpi.sHtML

B. 流程控制
来源：http://baike.hesvh.cn/Article/details/gblfqiowm.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/grazhnkev.sHtML

[B01] 条件判断 if / else
来源：http://blog.hesvh.cn/Article/details/grdbcvckz.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://www.share.zdbjq.cn/Article/details/gzvxlwtfu.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://m.share.fehbvm.com/Article/details/gpygdiivc.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://mobile.hesvh.cn/Article/details/gffyugbdv.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://mobile.hesvh.cn/Article/details/ghzvyrovs.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://mobile.hesvh.cn/Article/details/gdxggcygv.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://mobile.fehbvm.com/Article/details/gyrhgvvak.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.m.share.zdbjq.cn/Article/details/giaqplgrw.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://mobile.fehbvm.com/Article/details/gewsumotx.sHtML

[B02] 多分支 else if / elif
来源：http://www.share.zdbjq.cn/Article/details/grhvlwoiv.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://baike.zdbjq.cn/Article/details/grbhoxhrv.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://m.share.hesvh.cn/Article/details/guyoyghqh.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.hesvh.cn/Article/details/gwpduumcm.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.zdbjq.cn/Article/details/gvrzednqt.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.fehbvm.com/Article/details/gjwfankaf.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://mobile.zdbjq.cn/Article/details/genacijei.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://wap.zdbjq.cn/Article/details/gwniwqqiq.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.hesvh.cn/Article/details/gnqremgki.sHtML

[B03] switch / match / case
来源：http://m.share.fehbvm.com/Article/details/gghaohqaw.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://baike.fehbvm.com/Article/details/gahesjiyy.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.m.share.fehbvm.com/Article/details/gpezynnov.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.blog.fehbvm.com/Article/details/gnoxanigy.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.blog.hesvh.cn/Article/details/gzorljuwt.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.m.share.hesvh.cn/Article/details/gkxqkfjwz.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://blog.zdbjq.cn/Article/details/glailvcbk.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://blog.fehbvm.com/Article/details/gnyyeucct.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://read.share.fehbvm.com/Article/details/gnivhwzbu.sHtML

[B04] for 计数循环
来源：http://baike.fehbvm.com/Article/details/gvbfcxdmk.sHtML

Py:   for i in range(10): print(i)
来源：http://www.blog.fehbvm.com/Article/details/ghuucflhi.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://read.share.zdbjq.cn/Article/details/gwpalsngg.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wap.zdbjq.cn/Article/details/gqtgohcyo.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://blog.fehbvm.com/Article/details/gsufelnbl.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://3g.hesvh.cn/Article/details/grxhxkbcx.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://baike.fehbvm.com/Article/details/gpdudbeym.sHtML

Ruby: 10.times { |i| puts i }
来源：http://blog.hesvh.cn/Article/details/gpkhnmuyx.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://blog.zdbjq.cn/Article/details/gatmlndpn.sHtML

[B05] 遍历数组 / 列表
来源：http://read.share.fehbvm.com/Article/details/gtudbybfg.sHtML

Py:   for item in arr: print(item)
来源：http://read.share.fehbvm.com/Article/details/gtrwvehah.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://blog.hesvh.cn/Article/details/gxceqakwm.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://read.share.hesvh.cn/Article/details/gsufngtdk.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.share.fehbvm.com/Article/details/gpshmlovw.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://m.share.fehbvm.com/Article/details/gemtzgrit.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://m.share.hesvh.cn/Article/details/gmhpcghgx.sHtML

Ruby: arr.each { |item| puts item }
来源：http://baike.zdbjq.cn/Article/details/gzocksang.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://blog.zdbjq.cn/Article/details/gvjoceduk.sHtML

[B06] 遍历字典 / 对象
来源：http://baike.hesvh.cn/Article/details/gxdxvxupu.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://wap.hesvh.cn/Article/details/gxwztdbyi.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://wap.fehbvm.com/Article/details/gbcncasyt.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://baike.fehbvm.com/Article/details/gevofeayf.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://m.share.hesvh.cn/Article/details/gzvuhfiau.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.blog.zdbjq.cn/Article/details/gjicqgqtn.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.m.share.zdbjq.cn/Article/details/geuiikuxs.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://wap.fehbvm.com/Article/details/gcobceeun.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://3g.zdbjq.cn/Article/details/gtsxspqay.sHtML

[B07] while 循环
来源：http://read.share.zdbjq.cn/Article/details/gerpofzki.sHtML

Py:   while i < 10: i += 1
来源：http://www.m.share.zdbjq.cn/Article/details/gaclwmxdf.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.blog.hesvh.cn/Article/details/giaxteccg.sHtML

JS:   while (i < 10) { i++; }
来源：http://wap.hesvh.cn/Article/details/gwrudqrnt.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.share.zdbjq.cn/Article/details/gdjktgwoy.sHtML

Java: while (i < 10) { i++; }
来源：http://mobile.zdbjq.cn/Article/details/gfgrkxyky.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://3g.fehbvm.com/Article/details/gsugubfvo.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.m.share.fehbvm.com/Article/details/gvxznwkja.sHtML

C#:   while (i < 10) { i++; }
来源：http://read.share.fehbvm.com/Article/details/gmukgxxyf.sHtML

[B08] do-while（至少执行一次）
来源：http://www.share.fehbvm.com/Article/details/gsjasvtjs.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://m.share.fehbvm.com/Article/details/gijjzaoux.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://baike.hesvh.cn/Article/details/gamdsrwew.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.m.share.hesvh.cn/Article/details/gktpwgnrs.sHtML

TS:   do { i++; } while (i < 10);
来源：http://read.share.fehbvm.com/Article/details/gijveihrb.sHtML

Java: do { i++; } while (i < 10);
来源：http://3g.zdbjq.cn/Article/details/gnawgqqeh.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.blog.hesvh.cn/Article/details/gyxcesnyu.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://m.share.hesvh.cn/Article/details/gkukhnfra.sHtML

C#:   do { i++; } while (i < 10);
来源：http://3g.hesvh.cn/Article/details/gddygixvu.sHtML

[B09] break 与 continue
来源：http://baike.fehbvm.com/Article/details/glylkqvax.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://read.share.fehbvm.com/Article/details/gminyqfcu.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.m.share.zdbjq.cn/Article/details/gklkjymol.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.hesvh.cn/Article/details/gaxmftrnp.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.zdbjq.cn/Article/details/gubdwstui.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.zdbjq.cn/Article/details/giyhklssz.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://baike.fehbvm.com/Article/details/gczubqfhu.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.share.fehbvm.com/Article/details/gfzlekhmx.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.hesvh.cn/Article/details/gsozjsyvp.sHtML

[B10] 遍历同时拿索引
来源：http://3g.hesvh.cn/Article/details/gthxqjjqp.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://m.share.zdbjq.cn/Article/details/gkblqwefj.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.blog.hesvh.cn/Article/details/gedpsubrq.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://blog.hesvh.cn/Article/details/gvwanuwgp.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.m.share.zdbjq.cn/Article/details/gtgmouynx.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://m.share.hesvh.cn/Article/details/gvbwsprbq.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://read.share.zdbjq.cn/Article/details/geqqwckbu.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://blog.fehbvm.com/Article/details/gjkoovyaf.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.m.share.hesvh.cn/Article/details/gwpxldtvi.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.share.hesvh.cn/Article/details/garxzcawy.sHtML

Py:   list(range(0, 10, 2))
来源：http://baike.hesvh.cn/Article/details/gbsataslz.sHtML

PHP:  range(0, 10, 2);
来源：http://www.blog.hesvh.cn/Article/details/gsrasaouv.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://blog.zdbjq.cn/Article/details/gtdvmwcuq.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.zdbjq.cn/Article/details/gxjtelvzb.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.share.fehbvm.com/Article/details/gqaxpmkqq.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://wap.fehbvm.com/Article/details/gymbxxcis.sHtML

Ruby: (0...10).step(2).to_a
来源：http://mobile.fehbvm.com/Article/details/gpijjgmpu.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://baike.fehbvm.com/Article/details/gqhyecexe.sHtML

[B12] 跳出多层循环
来源：http://wap.hesvh.cn/Article/details/gwgwqhcjw.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://mobile.hesvh.cn/Article/details/gqzknrows.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://baike.fehbvm.com/Article/details/ggjmvhlbn.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.zdbjq.cn/Article/details/gukppsqxn.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.hesvh.cn/Article/details/gvcinnpld.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.share.fehbvm.com/Article/details/gysiutjhn.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://read.share.zdbjq.cn/Article/details/geeftyhoe.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.blog.fehbvm.com/Article/details/gjelgppdy.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.share.hesvh.cn/Article/details/gfuqjsufa.sHtML

[B13] 判断是否为数字
来源：http://m.share.fehbvm.com/Article/details/grrkoweiu.sHtML

Py:   isinstance(x, (int, float))
来源：http://blog.hesvh.cn/Article/details/gxttjzehg.sHtML

PHP:  is_numeric($x)
来源：http://3g.hesvh.cn/Article/details/grfcirpwx.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gwtkgrbub.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gsvjnngtz.sHtML

Java: x instanceof Number
来源：http://3g.zdbjq.cn/Article/details/gjlpllmmf.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://mobile.fehbvm.com/Article/details/gyprrzvhr.sHtML

Ruby: x.is_a?(Numeric)
来源：http://blog.fehbvm.com/Article/details/glodosbzx.sHtML

C#:   x is int or double or decimal
来源：http://m.share.hesvh.cn/Article/details/gtoglzvlc.sHtML

[B14] 判断值是否在集合内
来源：http://www.share.fehbvm.com/Article/details/gjgsmddwt.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.m.share.fehbvm.com/Article/details/gnaizgujw.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.share.zdbjq.cn/Article/details/grdbxlblf.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://m.share.zdbjq.cn/Article/details/guyqrriih.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.share.hesvh.cn/Article/details/ganpwdzmk.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://read.share.fehbvm.com/Article/details/gaqremxzf.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://3g.fehbvm.com/Article/details/goiewcfjs.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://read.share.hesvh.cn/Article/details/ggomiagcv.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://wap.zdbjq.cn/Article/details/gnkhrckec.sHtML

[B15] 布尔运算与取反
来源：http://3g.hesvh.cn/Article/details/gmnhgnpzk.sHtML

Py:   a and b or not c
来源：http://blog.fehbvm.com/Article/details/gwyexryqi.sHtML

PHP:  $a && $b || !$c
来源：http://www.blog.hesvh.cn/Article/details/ghblhuigs.sHtML

JS:   a && b || !c
来源：http://read.share.fehbvm.com/Article/details/gntazgmng.sHtML

TS:   a && b || !c
来源：http://mobile.hesvh.cn/Article/details/gwkdwstcz.sHtML

Java: a && b || !c
来源：http://blog.hesvh.cn/Article/details/gqhubeucm.sHtML

Go:   a && b || !c
来源：http://wap.fehbvm.com/Article/details/gsyuiwaqm.sHtML

Ruby: a && b || !c
来源：http://www.share.fehbvm.com/Article/details/ghngjqjfj.sHtML

C#:   a && b || !c
来源：http://3g.fehbvm.com/Article/details/gtxfhvogi.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://blog.zdbjq.cn/Article/details/gntorxmyw.sHtML

Py:   if not data: return
来源：http://www.share.hesvh.cn/Article/details/gzzpqgmsw.sHtML

PHP:  if (!$data) { return; }
来源：http://www.blog.zdbjq.cn/Article/details/grppknyry.sHtML

JS:   if (!data) return;
来源：http://www.blog.zdbjq.cn/Article/details/gagpuyipr.sHtML

TS:   if (!data) return;
来源：http://mobile.zdbjq.cn/Article/details/gnmuwrqyw.sHtML

Java: if (data == null) return;
来源：http://www.share.fehbvm.com/Article/details/gmqbeqaiq.sHtML

Go:   if data == nil { return }
来源：http://baike.hesvh.cn/Article/details/gercbzfgu.sHtML

Ruby: return if data.nil?
来源：http://baike.zdbjq.cn/Article/details/gqfepxnyy.sHtML

C#:   if (data == null) return;
来源：http://mobile.hesvh.cn/Article/details/gtptopppb.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gipktavfa.sHtML

C. 函数与作用域
来源：http://3g.hesvh.cn/Article/details/gpmnuwkqc.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gwdyrtmyy.sHtML

[C01] 定义函数
来源：http://mobile.hesvh.cn/Article/details/gnnnsdaoj.sHtML

Py:   def add(a, b): return a + b
来源：http://m.share.fehbvm.com/Article/details/gfqrgstez.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.fehbvm.com/Article/details/gqxmqjkhw.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://mobile.fehbvm.com/Article/details/gdntlwvqh.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.hesvh.cn/Article/details/gywdufyyt.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://mobile.fehbvm.com/Article/details/gdgesokil.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://3g.hesvh.cn/Article/details/gsbtxwadw.sHtML

Ruby: def add(a, b); a + b; end
来源：http://wap.hesvh.cn/Article/details/gugffkwed.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://blog.zdbjq.cn/Article/details/gdippjqjw.sHtML

[C02] 默认参数
来源：http://www.m.share.hesvh.cn/Article/details/gufhzgelw.sHtML

Py:   def greet(name="World"): return name
来源：http://mobile.hesvh.cn/Article/details/gotzdpenz.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://blog.fehbvm.com/Article/details/gutehvmir.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://baike.zdbjq.cn/Article/details/gazmeztnd.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://mobile.fehbvm.com/Article/details/glxojjejz.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://read.share.hesvh.cn/Article/details/gmcbfyqqn.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://m.share.fehbvm.com/Article/details/gkwvymlnl.sHtML

Ruby: def greet(name = "World") = name
来源：http://read.share.fehbvm.com/Article/details/ggfmojths.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://read.share.hesvh.cn/Article/details/gwdrbyqpx.sHtML

[C03] 可变参数
来源：http://read.share.hesvh.cn/Article/details/gnudytvii.sHtML

Py:   def total(*args): return sum(args)
来源：http://wap.fehbvm.com/Article/details/gkyaxgtur.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://read.share.hesvh.cn/Article/details/gskfkgbov.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.zdbjq.cn/Article/details/gkdpwgdqc.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.hesvh.cn/Article/details/gbhmjmvse.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://mobile.hesvh.cn/Article/details/gddjfxbdd.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://wap.zdbjq.cn/Article/details/gyjsaslnt.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://3g.hesvh.cn/Article/details/glzbvoqbl.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://baike.fehbvm.com/Article/details/gpqpmdkpl.sHtML

[C04] 命名参数 / 关键字参数
来源：http://m.share.hesvh.cn/Article/details/gpwfznytt.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.share.hesvh.cn/Article/details/gjzuygmgg.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://mobile.hesvh.cn/Article/details/gpcurfvgm.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.share.fehbvm.com/Article/details/gxgphvatv.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.m.share.hesvh.cn/Article/details/ggpmhxngc.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://3g.zdbjq.cn/Article/details/gswlpolcj.sHtML

Go:   // 无：用配置结构体参数
来源：http://3g.zdbjq.cn/Article/details/gaucqsvfv.sHtML

Ruby: f(a: 1, b: 2)
来源：http://m.share.zdbjq.cn/Article/details/ghbgnmzda.sHtML

C#:   f(a: 1, b: 2)
来源：http://3g.zdbjq.cn/Article/details/glkcdiqzw.sHtML

[C05] 返回多个值
来源：http://www.m.share.hesvh.cn/Article/details/grzohwyzy.sHtML

Py:   return a, b
来源：http://www.blog.zdbjq.cn/Article/details/gxxsdflqy.sHtML

PHP:  return [$a, $b];
来源：http://wap.zdbjq.cn/Article/details/gutmwtghd.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.share.fehbvm.com/Article/details/gavqcnein.sHtML

TS:   return { a, b };
来源：http://mobile.hesvh.cn/Article/details/ggspucmeq.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://wap.zdbjq.cn/Article/details/gmsidfgbe.sHtML

Go:   return a, b
来源：http://3g.fehbvm.com/Article/details/gtpvjurtx.sHtML

Ruby: return a, b
来源：http://3g.zdbjq.cn/Article/details/gmwggwlqn.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://3g.hesvh.cn/Article/details/gfzxypqxe.sHtML

[C06] 匿名函数 / lambda
来源：http://3g.hesvh.cn/Article/details/gmlfxbygr.sHtML

Py:   square = lambda x: x * x
来源：http://3g.fehbvm.com/Article/details/giskvefuj.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.share.zdbjq.cn/Article/details/gdnmmzlvc.sHtML

JS:   const square = x => x * x;
来源：http://blog.hesvh.cn/Article/details/gphjpzwuv.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.blog.fehbvm.com/Article/details/gkzhzewfd.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.share.hesvh.cn/Article/details/gydksuysj.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://wap.zdbjq.cn/Article/details/gsnvodmoa.sHtML

Ruby: square = ->(x) { x * x }
来源：http://read.share.zdbjq.cn/Article/details/geawcffbk.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://read.share.hesvh.cn/Article/details/gwqfghheu.sHtML

[C07] 把函数作为参数传入
来源：http://www.blog.zdbjq.cn/Article/details/grlfieuwr.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://m.share.hesvh.cn/Article/details/gxgrhmxlw.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://baike.zdbjq.cn/Article/details/gvzjpboep.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://mobile.fehbvm.com/Article/details/gafyldams.sHtML

TS:   arr.map(String)
来源：http://mobile.fehbvm.com/Article/details/grvqnpmdj.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.m.share.zdbjq.cn/Article/details/gibpewxxk.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://read.share.hesvh.cn/Article/details/gagyrrxlt.sHtML

Ruby: arr.map(&:upcase)
来源：http://mobile.zdbjq.cn/Article/details/gnursrggu.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://read.share.zdbjq.cn/Article/details/gznrfrtik.sHtML

[C08] 闭包
来源：http://www.m.share.hesvh.cn/Article/details/gngagfzuy.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://blog.fehbvm.com/Article/details/gwilevzeu.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://blog.fehbvm.com/Article/details/gsjipcdgv.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://wap.zdbjq.cn/Article/details/gocxcihvq.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://wap.hesvh.cn/Article/details/gnwlqusll.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://wap.zdbjq.cn/Article/details/gierohxcu.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://wap.hesvh.cn/Article/details/gwijqgozy.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.m.share.hesvh.cn/Article/details/gzexngqdn.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.m.share.hesvh.cn/Article/details/gljfaaoaf.sHtML

[C09] 递归
来源：http://baike.zdbjq.cn/Article/details/gmdcrsjhz.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://baike.zdbjq.cn/Article/details/gfpcsrswr.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.blog.fehbvm.com/Article/details/gywtmrztv.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.zdbjq.cn/Article/details/gmrxkdekc.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.zdbjq.cn/Article/details/gzkbmgbqb.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://m.share.fehbvm.com/Article/details/gqufvmfah.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://3g.fehbvm.com/Article/details/ghzlbwzcm.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://blog.hesvh.cn/Article/details/giatvoxyr.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://blog.fehbvm.com/Article/details/gnrwffdip.sHtML

[C10] 变量作用域
来源：http://read.share.zdbjq.cn/Article/details/gfgqfctat.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.m.share.hesvh.cn/Article/details/grhulfdoo.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.m.share.fehbvm.com/Article/details/gizckwkfs.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://m.share.fehbvm.com/Article/details/gyithlwev.sHtML

TS:   同 JS
来源：http://read.share.hesvh.cn/Article/details/gxbsjvrhy.sHtML

Java: 方法内为块级作用域
来源：http://m.share.zdbjq.cn/Article/details/gctlbmuke.sHtML

Go:   花括号块级作用域
来源：http://www.blog.hesvh.cn/Article/details/gtnutwvzi.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.share.hesvh.cn/Article/details/gamlsaorv.sHtML

C#:   块级作用域
来源：http://www.blog.fehbvm.com/Article/details/gdnxsknjj.sHtML

[C11] 模块导入与导出
来源：http://www.share.zdbjq.cn/Article/details/geioytqwh.sHtML

Py:   from module import func
来源：http://wap.zdbjq.cn/Article/details/grooxplbi.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://m.share.zdbjq.cn/Article/details/gswmyzoeg.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://m.share.zdbjq.cn/Article/details/gbvvojcbc.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://baike.hesvh.cn/Article/details/ghujjfunn.sHtML

Java: import java.util.List;
来源：http://www.m.share.zdbjq.cn/Article/details/gtdzokrvc.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://read.share.fehbvm.com/Article/details/gbtawuepe.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.m.share.fehbvm.com/Article/details/gnnaelcyu.sHtML

C#:   using System.Text;
来源：http://blog.hesvh.cn/Article/details/gandjfydt.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.blog.fehbvm.com/Article/details/goshepsuc.sHtML

Py:   (lambda: print("run"))()
来源：http://3g.hesvh.cn/Article/details/gdlvgjzfa.sHtML

PHP:  (function () { echo "run"; })();
来源：http://read.share.zdbjq.cn/Article/details/goykpgthp.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.m.share.fehbvm.com/Article/details/gcjszmtqu.sHtML

TS:   (() => { console.log("run"); })();
来源：http://m.share.zdbjq.cn/Article/details/ggojzmmup.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://mobile.fehbvm.com/Article/details/gsfwukajk.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://blog.fehbvm.com/Article/details/glowgbiof.sHtML

Ruby: -> { puts "run" }.call
来源：http://mobile.hesvh.cn/Article/details/grgdyqvlj.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://wap.zdbjq.cn/Article/details/gkbelwlwr.sHtML

[C13] 类型声明 / 类型注解
来源：http://m.share.hesvh.cn/Article/details/gaeoisxyv.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://blog.zdbjq.cn/Article/details/gtxcgdzdv.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.fehbvm.com/Article/details/gwhjtfhzx.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://blog.zdbjq.cn/Article/details/gdcgvtzfh.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.hesvh.cn/Article/details/glbcpevzd.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://read.share.hesvh.cn/Article/details/gkenvhypb.sHtML

Go:   func add(a, b int) int
来源：http://www.m.share.zdbjq.cn/Article/details/gwwdnasnk.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://3g.hesvh.cn/Article/details/gokznnvym.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://mobile.fehbvm.com/Article/details/gnimumfjz.sHtML

[C14] 泛型函数
来源：http://baike.hesvh.cn/Article/details/gymxssrtf.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wap.fehbvm.com/Article/details/gwtcunwrz.sHtML

PHP:  // 无泛型
来源：http://blog.hesvh.cn/Article/details/gqryqdudt.sHtML

JS:   // 无泛型
来源：http://wap.fehbvm.com/Article/details/gmdxdkpkc.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://blog.zdbjq.cn/Article/details/gircimyfv.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.blog.fehbvm.com/Article/details/gaiaoiwhd.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.share.hesvh.cn/Article/details/gljklocsf.sHtML

Ruby: # 无泛型
来源：http://3g.zdbjq.cn/Article/details/guznkpbro.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://blog.hesvh.cn/Article/details/gtsuneplt.sHtML

[C15] 解构 / 展开参数
来源：http://3g.zdbjq.cn/Article/details/gneapjcrj.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.share.fehbvm.com/Article/details/gslslfcja.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.share.hesvh.cn/Article/details/grtsfsesu.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.blog.fehbvm.com/Article/details/getacpfgc.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://read.share.fehbvm.com/Article/details/gntjyvnra.sHtML

Java: // 无解构
来源：http://mobile.hesvh.cn/Article/details/gifsbcsvq.sHtML

Go:   // 无解构
来源：http://3g.hesvh.cn/Article/details/ganqrlwef.sHtML

Ruby: a, b = pair
来源：http://www.blog.hesvh.cn/Article/details/glfkpvqvl.sHtML

C#:   var (a, b) = pair;
来源：http://blog.zdbjq.cn/Article/details/grvukhmdi.sHtML

[C16] 函数 / 方法重载
来源：http://www.m.share.hesvh.cn/Article/details/gbckdngjv.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://baike.zdbjq.cn/Article/details/gapwdpzza.sHtML

PHP:  // 无重载
来源：http://www.share.fehbvm.com/Article/details/gtmdqhupa.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.m.share.fehbvm.com/Article/details/giuxnravb.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://3g.hesvh.cn/Article/details/ggauyztbv.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://baike.hesvh.cn/Article/details/gmhemkjok.sHtML

Go:   // 无重载：用不同函数名
来源：http://3g.fehbvm.com/Article/details/ggshclggs.sHtML

Ruby: # 无重载：靠动态参数
来源：http://m.share.zdbjq.cn/Article/details/gueadwpsr.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://m.share.zdbjq.cn/Article/details/gmspfijpw.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gsqpvihmx.sHtML


<!-- 参考信息 -->