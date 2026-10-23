代发 wailian999

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt3gtojczil.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3izcyvyub.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt3dvfcdqfw.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt3zdxosblt.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3buvsolhb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xftiwpem.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt3jcprgspa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ijkyhqji.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3rbayccyw.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3wkwsawef.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3jvrfmvrq.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3immhzrpf.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3eskmnqeu.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3awinwfmr.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3vjeytfta.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3gpkglhjx.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3kfrxpmeb.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3vsuwtgfa.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3odgehsid.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt3aaotovqe.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3uanfdbcv.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3anrhfgil.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3qrtzgzso.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3cckuummy.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3sookzxfd.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3oetkyoby.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3ddwmqiqn.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3hnausmko.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3algyinee.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3jtfydvqm.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3srlqxapi.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ynhxkqxb.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3vjeblkyd.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3loyppxso.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3yepjhzjd.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3rquzerhi.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3xgbvqqhi.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3eseuvexn.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3nhmeerjb.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3agmttpky.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3jjqahivw.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3ddmdkjxz.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3brnwgeor.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3hhadnhid.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3zbkocnsc.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3cgaahpbk.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3xlsoatcy.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3bpqyfuqs.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3ekycakwu.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3rkattppl.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3qdvsgoat.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3wlfgtsxj.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3fywiekwv.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3ycenhlpi.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3sqkplycp.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3prbpgbkb.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3irlzefpq.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3ingmrfgb.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3ggunjnxa.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3ielxiege.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3mvdgcqev.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3mscgmcnt.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3xsbtbsha.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3bipkimei.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3fbjkryje.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3zfkfwoxz.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3pqdrazus.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3zchzxjzb.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3pigktjju.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3vjlxrihh.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3tbegskhj.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3lyghpyzj.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3mzyijmjo.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3txuilxtj.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3ipaljdcw.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3tuqcthte.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3kcqleqsp.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3ajyinhvg.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3jbudvuri.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3dojufzjh.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3lhodcimq.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3ftuxsiul.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3bjzuuyyj.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3uygsixur.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3tcbsxvwf.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3myxwghrv.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3nuzbzqoy.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3udyntmho.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3yzpgiodj.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3gbfzzihr.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3tekeooox.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3abkylkxh.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3hgnqjofs.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3tyluqluf.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3njexpeuq.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3wxflfife.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3brepsgdu.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3ewpmniff.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3uasldpzi.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3snamqytt.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3dzbhvtsm.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3lykftnfy.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3yjuebktc.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3fpwumuft.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3gscblygl.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3yqvgpzvv.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3gghhliwj.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3mtqmvpny.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3noqhuaij.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3iniwjcqf.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3ocpfvodj.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3vsyzqfoq.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3eowbzcwh.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3qpsvplvq.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3jygddtmo.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3nlqjtdbt.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3lznxdkmb.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3grhvxgnz.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3ustiuszq.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3tqjidlyn.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3pgwucpcs.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3rltsxazm.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3dkkpnygr.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3hymvhgmi.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3dieyikfd.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3tvrwfckf.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3txtrystp.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3cthydvaq.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3zvijxwtb.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3tmcpqxts.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3jvuivdaa.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3hjpzwnyp.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3zhiispoa.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3wggwgqjg.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3fxdlrdsl.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3ktmgutkl.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3tcuizmro.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3awgvfcir.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3fobmexxb.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3ofndtinl.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3giogipnq.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3rkyiljbv.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3xphqvytq.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3wawabycc.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3mmsrekra.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3vtqnqblh.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3uetqdtsa.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3uxsvstev.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3piurzsmr.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3gdeltiac.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3fefkyiki.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3zifywzxb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tkkapnho.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3udgdiayc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cuicakcx.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3pblsatsi.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3ixjtewzp.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3hrrhkeab.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3eqlseqlh.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3chzwjfpb.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3xgkmcbms.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3sohqmztl.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3vlnrkkpa.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3ttffrlsr.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3yorpbbzt.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3oiouxvez.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3wiwmfnvf.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3hnmfxhhm.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3cyhaokgg.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3ydkegcyj.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3ysbvutqb.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3rcfrsqsd.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3hojatnlm.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3okngxqft.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3wslebblm.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3fencdvfo.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3bpkfncgn.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3yeivdrkv.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3ednglaat.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3kqvzdyir.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3hxaeezjd.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3wjwjzguz.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3egoscxlp.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3cbflpuhm.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3aiapztru.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3pilqwkxb.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3cevzodde.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3daradbyk.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3jclifitz.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3yvargrym.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3nkonhvhy.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3mduglyxp.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3hmtftetm.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3zfxbflec.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3iqhoxiby.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3xpzbxpqk.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3ygkrtnaz.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3blmdfrum.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3bnkcowtb.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3lukolhnr.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3sodffofi.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3xpessfif.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3bpakbogd.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3lezkksis.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3swbyarar.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3xadsxjuv.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3mpsivofg.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3uecwihqr.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3uqmtkmyi.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3vwprdsil.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3pfxcnbnq.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3rmvbrxkt.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3aqxbypgp.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3okcougxg.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3jmcsqsir.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3ffwqhnyi.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3wjiecxnq.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3rwmyngpu.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3ivbwaeou.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3lgsfgneb.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3wzfilzam.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3waucyisi.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3qqoooaeb.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3xlvrdwgd.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3rknmqavi.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3cpgmpmjq.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3smmlaovx.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3ezykpvdk.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3ckrrtpih.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3msyemgvd.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3ecqaswvh.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3selpmpbq.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3cguuccff.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3grqabtqy.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3tslnbtop.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3zydgzdfb.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3kbkfnwtz.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3thxaznnl.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3jeoaivtm.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3ysxmuedt.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3atzmzfhu.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3exfwudhs.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3ownjplcw.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3shxayaop.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3btlpeezo.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3hufqooev.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3cidgzkcg.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3flwkwkca.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3pbsjeemq.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3eolpxqan.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3tuinsbvg.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3qmiyjtmk.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3bnctejxq.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3xjytmtet.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3fpmlenzb.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3bsubqwcp.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3ajfboasy.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3lwveniyp.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3ngwbhiye.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3nvjdatpm.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3ncfdizzj.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3ewflihgs.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3rzpwpmvx.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3meuizpww.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3bvfzyigm.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3tfygvwbh.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3omsowyca.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3gzmvnbyx.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3vlqtxqyl.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3vkiaedwp.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3mginrshf.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3ayheddtc.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3zckmwekl.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3txrxkyas.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3vhidztlt.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3rajaknht.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3dyhrynjk.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3acxxsguj.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3zpbuennc.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3dvxyftpx.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3rzxiogho.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3jxyargvs.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3bvchtdfw.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3npbhzgby.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3ztzmiqfa.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3diqanovu.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3cthwniei.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3furxcugm.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3qzegjszf.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3iewyplug.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3eaufnxnx.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3mwibdphi.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3itbhfgbn.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3toijuupb.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3cwfeqgcp.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gfqhonos.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3rasnqmkj.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3qsfzenxu.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jtlvgtyt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3plhxfnzp.html


<!-- 参考信息 -->