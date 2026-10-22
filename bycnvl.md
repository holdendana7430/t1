代发 wailian999

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2wkdmehrl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zsmvpvjz.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2tjuvnlgg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yxokufxn.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2vsdvvoph.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2ltiytcka.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2bssecpza.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2bwqxqpqz.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2qixujwgu.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2ucjpwfnr.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2lnrfkezw.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2dboxbwqh.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2ldysvaro.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2fdjqxguk.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2isfiqdsr.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2glejlwmx.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2eowshroy.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2ubgnwkqq.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2vkmsmfxu.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2krvdksxb.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2vudtazzl.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2ikcyccsg.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2yjlxmdcp.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2nvnbddni.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2qwbyxegp.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2dqaydapm.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2aucimndx.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2rkxttxgo.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2ikbtopva.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2ghwpcqfq.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2cgautyyy.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2wzlvbehw.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2xukejozq.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2glfznvcm.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2pmxwoopu.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2nhvpcbjo.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2hpmnsqoz.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2ebuszkdp.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2wwvcxlat.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2srldqqfk.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2xknbkzah.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2bhbgdymb.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2tqverufi.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2fblfnuil.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2jsjaitua.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2uuesshlk.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2tindljia.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2ovlsgybl.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2owkiksav.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2svicmwag.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2rwxjmpzj.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2hbbcmsai.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2cpupadal.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2hkxdpxti.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2uxljdvns.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2tioqaoih.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2daxgqexd.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2qgwmjvdo.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2fwartweu.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2ognpvmfm.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2qlniehfg.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2joivhmtd.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2llintrnd.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2hjhmvhmj.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2wgjalkfi.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2phnydkxz.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2jiofksth.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2crbfofnx.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2lvoqygbk.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2gyprinzt.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2rfwawcyo.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2byuftevh.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2dsnctdmz.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2ietktvtl.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2rxicfubr.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2mssnglyy.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2zgekyqvj.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2nypwdrry.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2mcejqujk.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2kixaspdc.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2yhyhatdv.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2bwgygoaw.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2lzsdqktg.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2vmlmmpzv.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2bokunuqh.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2blfizday.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2pfztxogm.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2rohsxobj.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2ormkeolh.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2bgjuyyip.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2tqhjetdu.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2vnvksvyk.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2tbsfgpsa.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2wbqewhup.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2iagkuskq.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2bghmqwqx.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2mtwrggwd.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ckatxbgr.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2szvrwagf.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2kfqsrmxp.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2tdkybrcd.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2wrbaqbim.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2mmiyvtrd.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2xnjcrmjz.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2uiwfbhtx.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2bgfsduup.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2fqmlpwja.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2abqpktyh.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2yyrkbofo.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2jwjchfqa.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2llxxgzjw.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2dgicumst.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2otzmjnhu.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2jlnqpkdk.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2jcjwozit.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2vzemrnfh.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2utrwtvcv.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2ksoggygf.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2jnicqntn.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2ywgaubdh.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2nwqzcrnt.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2edsgblwf.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2grtdpwxo.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2pxqjnidh.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2azahcmia.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2gjtufayn.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2nbpcgixl.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2zlxfklwk.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2idphfxtr.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2gtqefjja.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2ojgjbzui.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2arsxkrny.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2qeiudhzw.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2fsqlpegw.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2hskdygpf.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2hddmlytv.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2bmmubabh.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2opdecbjw.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2tdcxxzpt.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2ruggeysg.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2mruslpll.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2wzrdlcfz.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2pqjsjfpq.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2oynflvbj.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2vbkchoxg.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2xqtttvmj.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2bvswakdi.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2mktunkfp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lgrglezh.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2jjxuaxhp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zhpvybrm.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2zetzifus.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2xqrwfeav.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2caoeucyj.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2hzttpzbe.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ohktjsfe.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ihjmwdhs.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2zclgfmxs.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2rkciitvd.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2vljazlug.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2lrdofuqx.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2exnmrnbk.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2dgkcyboy.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2tlqveavs.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2dsgazgqz.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2axafrmmr.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2omfkfxkl.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2xqtuumpf.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2zrjodxdf.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2qikmtivb.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2cwtxolzg.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2vwlboywg.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2ejaqaqzo.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2uymgrdaw.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2fcurrzye.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2devfhsrh.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2tcaunhpy.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2olyvvuue.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2saiiwmqz.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2pvbdnwld.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2sytlsvjg.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2ylaswwqc.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2ahtdangr.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2jveimrvl.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2mfxspyar.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2exwqwtjk.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2tgsjzaam.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2yfrsmvcq.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2krdnsneq.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2lsmylkyf.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2xyqhjdhb.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2zwhwxbxi.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2iztuhdpc.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2qzebpjve.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2phxwljgf.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2xiqxvxfv.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2rdqmjhhp.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2poxyjmym.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2upljbkim.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2jdfmuxfr.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2crskdpnz.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2pnyhyjba.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2mgcpmftc.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2wkfawrbw.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2gqlhmguu.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2elqeseft.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2xgivoogg.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2fsgqimkx.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2kdnarnhk.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2grscporx.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2uwwattqw.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2wkplpaqm.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2mekwrgnj.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2tizhudjj.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2oqlerocx.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2vwldmrja.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2byqvzrun.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2svvgzuoe.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2wvgysdwm.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2aozevoee.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2znfnhtur.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2cvshdroo.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2fbfqnuko.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2piwngxrz.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2gblkzhhn.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2uzimuyfi.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2nbudooxm.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2jvjcuofg.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2hfphbwvu.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2gdxmmksb.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2oabrklam.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2vwlpkmci.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2vfyxjkic.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2wesdcnot.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2eqrryouw.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2yyvnecjn.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2gjxoavxz.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2igjzoxyf.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2syjjlfli.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2txyylvnl.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2hwzouazg.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2xjgzjngu.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2mgevtiwq.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2ncawerhf.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2ypwzxzyg.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2wzdxfmdo.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2wexypjjm.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2qemgmvym.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2giunhirv.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2ihcfpgab.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2nzqmlvhq.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2jntpfoer.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2nwcouefl.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2nfbjqmbt.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2oonnxftf.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2spsxbwel.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2xxrrknsi.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2oxqbotgq.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2eenzdxfj.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2gftwqfjb.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2bahcogzz.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2nkelfidn.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2mmgfxrfv.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2uifzbvhg.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2uulmizdb.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2eofukinf.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2letseeck.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2bwpwwafb.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2iegtimdu.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2gszdwhtb.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2tpxoaejp.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2ymsilxzi.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2pkyaakav.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2rtdlosif.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2mdskwceu.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2mphjyzie.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2okldcfre.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2bgfiqpia.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2dcvlnrge.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2tewfczos.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2cdugjhne.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2ejuiwyzv.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2aazgvcqm.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2zufatniw.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2wvkxsmbb.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2orusmzux.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2kmkjurax.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2tekbupqx.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2ejfjgcaw.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2frclzlfe.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2swkbggfv.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2vwkgkbxs.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2xfwaqtwi.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2vyosxjkr.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2kommwsbg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qwwcznpp.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2yogisuly.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lwfqbqvy.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2mrclevwc.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2dsrpwyku.html


<!-- 参考信息 -->