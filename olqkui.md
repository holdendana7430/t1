代发 wailian999

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3hmqwfhhm.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3tsgrktkz.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt3gnqwjiiq.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3iidnotvd.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3xffxmuhy.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3jtxiabgf.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt3peagmftp.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt3eqjtowuc.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3pvqovzps.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3omdppwqu.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3vthbvbku.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zadyofvw.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3hyukovvm.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3kvklsdkf.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3zmdaigcr.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3gxkoaxvg.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3isugyaqp.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3lsfatyji.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3vzeiryvh.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3kltdlifi.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3mwiyzuaa.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3ibumufzx.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3xmlncysa.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt3kzypzqcb.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3zhojiasa.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3vpcfmdnz.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3xgqfyurk.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3kqhmfiju.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3tcbkpekz.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3vxyggjdz.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3vksodrch.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3ixxpypor.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3puyjgfkl.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3gpvwwvid.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3ercunnoi.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3sllzsovv.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3sgyyuvkz.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3fiptpoqa.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3dsywncpp.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3nacmrugj.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3zfeqwpxm.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3eroxgmkl.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3lrxdxepe.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3yuvehceh.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3sumyzewc.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3rdfzymbi.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3aoymgonm.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3zvovpvri.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3liavohmo.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3eicmthze.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3bcysrlfv.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3rlcqhexi.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3ujrhyzrl.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3zcvgaxxl.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3ftjbpbix.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3kvejrmpf.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3toccsozm.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3bxehyjfe.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3gauylvqx.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3lipwweii.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3wvqrwlkw.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3wpwkuhzk.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3rbwflvao.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3dbrjfceq.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3hjhzoldp.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3ifadypsu.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3bqohijfy.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3rtxhurin.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3dpuzdwmj.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3rlvlojrh.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3koxtemzw.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3bvtbihbi.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3czcckezo.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3eqtbwhkz.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3wrkbvdmn.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3rabslocj.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3olmeriuk.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3nqsamdna.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3mlnmgpcy.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3srqboffz.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3rdmixsaq.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3xfgcsuus.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3chibdxiv.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3vbeqjjfp.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3dquzywlk.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3jhjmfooe.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3tabttnir.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3jvlonyfj.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3tzraloku.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3gzqchfhx.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3unwccipv.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3ttopqiqi.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3csujfnlo.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3hskmqfmc.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3jysdyshg.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3ipxvvooz.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3qmmbykou.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3wjzyxhpb.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3squjpplm.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3uvdpaozo.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3llixjijf.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3aseffbpu.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3rkkumerb.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3zdxoqcbp.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3ujkeagby.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3eiltdjjk.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3jnyernay.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3yhnrlpjt.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3xqxdvbai.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3bkpokksn.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3jotazxgo.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3jxkvdurm.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3zmpjpjvb.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3yyaibhfl.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3nifuruad.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3hfqyjuwp.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3jaamfnmd.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3bmqqeaqk.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3kmuzmxvo.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3fkyqtdmn.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3itjzbkbr.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3eyndcafd.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3pnayjuty.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3lkpntsno.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3odvxkozz.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3svxwzebd.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3vcesqsli.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3etzoqrxr.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3wekdbhof.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3lljzahor.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3bbdsqtrq.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3rlrxgnxe.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ltbgkgbx.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3sgfdytlu.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3viurgifj.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3gapcauka.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3drrezcvn.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3jvjpixkk.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3dqdsizso.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3rvptmjst.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3bunemnvw.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3jjsithuj.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3ssmbwvag.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3ugqmstdj.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3dicapppt.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3vcpmbzma.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3vazmhcem.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3lshgnknf.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3swzyjolo.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3lxgppfdn.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3afuutmhz.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3ulcjnkag.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3vncwritg.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3vrcewaag.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3gxegrnnk.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3dojnwton.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3oyotogfj.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3akgwmbes.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ktxeohwl.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3yxazitse.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3hfztvrme.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3gvvnmxbx.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3avgefqkv.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3gqrxgfrj.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3otxpyecx.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3xjnsxlpg.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3vhxzrsvq.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3zmisovjc.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3bhrobrzk.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3tsogtqah.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3mupegout.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3prwawjwi.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3ryxgsgal.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3ahteixhi.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3orwddkux.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3qopccnvx.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3dnyumbzx.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3qjxutivh.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3cwwdnjhb.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3udyuamdp.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3oemrbeqc.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3uxsjwunl.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3jgxiebgy.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3tellrbbn.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3nibbijdv.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3djsbzwfx.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3hxsckxvb.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3mshxqboa.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3psbwzalp.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3ghindrhk.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3lqlhspjb.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3ouavjbmh.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3fhudding.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3euioswrl.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3vxjbquhs.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3dvlyxdlb.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3uqixyoua.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3qcyvnxrv.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3ovrtedsq.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3sgurqpjq.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3oiuvnbbq.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3beuzxzxi.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3mpdrbzxt.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3kxwiwksq.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3nweutxwz.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3abkmehbr.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3xkmdyesa.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3phpstjjl.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3ojtocnpv.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3mhfmsztg.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3dcvgnceh.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3xjrczslp.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3cudakoid.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3ueleicsl.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3vsdftrjb.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3ywbluwqr.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3xmryydik.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3msszeqzn.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3gfcsbfhj.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3szqvxcuk.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3tvqoqazf.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3hggsxmqj.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3fcvnxjqx.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3jdpmoont.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3xujmypwf.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3fuhbqprj.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3ocfhbjzp.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3mbdoiqxd.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3igutgylf.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3hpjqnzdc.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3yizgyxtt.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3ftlvjarh.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3lxrtsyto.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3jmacvwgf.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3crucefnp.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3rukmreqm.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3jqznskfr.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3frgfqebw.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3oyberubr.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3mleyfpci.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3wehehohj.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3wqxkzthx.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3xsstojtg.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3pyjzoosf.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3wcbwsblc.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3ldobbrrc.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3llgbabyc.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3bhaknaux.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3yompqcxp.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3gcpfgpjd.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3tdxxpbwz.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3eljjpklh.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3fmvazgcv.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3tdwvrjos.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3atepjjht.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3sygdcgsx.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3vvtyktvq.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3utgxkvty.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3mrilfhsb.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3jsupwfgo.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3ttxjyidf.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3pwgmypks.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3czuqptqx.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3oohbxtjv.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3pbzzhgjg.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3gojxawge.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3upasyugl.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3evwnfwda.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3msrnxncs.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3dxrpsaba.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3ggopatkq.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3ykfwerjm.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3estptbvj.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3sjeqzeqx.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3tsnldghd.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3aimopzen.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3gdozatus.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3priusfnq.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3qntorjkt.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3lfootyzn.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3xbbymjrd.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3lwizormz.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3dxavzayp.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3noxdjqmk.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3wldzxdol.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3jurwhffo.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3nldfioiv.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3xlgsefsb.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ojlkoftt.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3sbqergjb.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3dvmyxqxk.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3gjqmsvbr.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3tkddzjkp.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3ipibtjsj.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3tnthaxjw.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3alkwwuvg.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3irzpdtir.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3aupmjdst.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3tanygdft.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qsofhdxx.html


<!-- 参考信息 -->