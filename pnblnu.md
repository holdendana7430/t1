代发 wailian999

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3dljhnfnr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jwgcqmlf.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3pvuvizwe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ufprrdoo.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3zswtgkda.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3xhexngtw.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3fqgyllwc.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3pbotacpo.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3ykjwcytf.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3tmsfepgu.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3mpzjfxpw.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3isoapkwh.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3rzezlots.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3zbydfbyf.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3mrckoeoi.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3hwhlwkjz.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3xhldbtfk.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3ggumvaeu.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3zowunysx.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3sopuyets.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3xkfbhxwq.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3pfequrct.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3vkcrhhjn.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3nzwymcjb.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3aziybygw.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3qigyelzj.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3mtjfryqf.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3lxauttwq.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3ramzqzwl.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3czfbcfln.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3otlcrihf.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3xrigvpyl.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3qrrjcedj.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3cdplcyzm.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3kupyjxrp.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3byfcipyu.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3srqbherc.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3gpdyeqpw.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3qsnezpay.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3qoueobqr.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3fzeprywc.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3mziihfsz.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3kihcirhq.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3xzmcbegv.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3fopoxazv.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3aleizkzg.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3uxidffrv.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3nxdwqfsn.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3mgljgnqj.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3grhudlfz.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3wegyzqcl.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3pncoifev.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3vmcfzaqh.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3swxtoibl.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3fnsbpbov.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3phnigvge.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3ylnlkicj.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3rtdmkxro.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3hiwjgzdf.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3nolveqoc.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3pnypqgbj.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3kpeentap.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3fbdqtolp.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3ayynlwkw.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3foszaxhd.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3gjzmempa.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3imzidpay.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3lrpsbvch.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3llxeylzl.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3dqkykrsk.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3oduhdgjb.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3rpenypof.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3bubaxwrq.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3jyxynfsk.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3zegeeyjq.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3afrnlxxj.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3uxdimmaa.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3pyncsnej.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3nazmelfj.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3zsosoxlj.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3zllqfemp.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3wlziurvb.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3kgfwrwut.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3mnuleect.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3hqsvctyb.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3ksxnuxee.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3fxxyljje.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3pbzfnzdp.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3fbyyuhbx.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3jkbwxsdf.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3bdnvgjtn.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3xnalbdhq.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3ondfohwj.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3yqlomkpp.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3lolghiby.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3ephwefwx.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3spghnbxz.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3akkpzdxx.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3wihnhoin.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3nykhugdm.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3qwsypzyr.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3ezcexzqe.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3sdwrhivy.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3bjbrayew.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3vgwohszr.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3olqsqohe.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3kgpwsumt.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3yxelekyt.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3ldzhllkb.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3volfjaqh.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3cfrfptyw.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3mialduop.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3jdelcucl.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3sreeisuf.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3zosinoto.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3gxtjazli.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3alunojja.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3cvnzfbqb.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3onyvwuxs.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3tszedgwv.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3htwzzacq.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3dmgaewht.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3hrfeuxio.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3bvsyzfpu.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3myuercgm.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3vbnmfrrk.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3qwyzexij.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3acmegktw.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3amhjgfaf.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3esktfwhc.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3ygjrdgml.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3qdvryrep.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3ktfpdoel.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3fhpknudo.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3ikfbspbs.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3mvidstad.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3mcbnprdf.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3kikdnnzi.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3mpganqui.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3aaffkqnc.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3sfhtweno.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3blnkyqdi.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3khvqvqmf.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3gubktmjj.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3fbatdinm.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3abryubit.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3lnzbxxiv.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3mqkbmmzx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xovglfgu.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3asgqftcf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3sbalhreo.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3wpkjtrxa.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3lcvrqbzu.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3ncmvekgx.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3kguyihki.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3bqwaizyw.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3qyalqsfc.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3ewcmgkzz.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3hnubppkn.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3rmuevvip.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3eglgdgvt.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3mbmibpjs.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3pfzeazpf.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3vvglwcmm.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3izaktoxd.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3yswilmqe.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3bihgfbcy.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3wbbnckzv.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3ektlzzji.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3rhtwcosp.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3wcvwrhoh.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3cksuvkcq.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3newfqrpy.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3jfazkizr.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3zcibvjpr.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3eijsgmcq.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3kmgzsnry.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3uhhkfvwr.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3xhpaqdvt.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3blkevhsy.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3firbohhe.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3vloeqwcl.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3aprllzyh.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3eixttnmy.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3rsutahwf.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3ixhsdpzj.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3wakpnqpc.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3koixythd.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3ebsbqrhy.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3fzzigmkb.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3btcrftpk.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3jecljmcf.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3zgnfhwrj.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3pbwvfslg.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3lfcuiffp.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3ykvkafxy.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3cqeojshr.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3rrfuioez.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3frbsortc.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3ignbglru.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3tunmpjuf.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3jalijahm.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3xqksveyg.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3dwdsftsk.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3dedwegoi.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3hzjwcpfi.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3ryuoecsu.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3ffywfbqd.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3npwvuhgi.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3tbohmbqe.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3ruejbwoy.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3loqmenyj.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3hfcgsbum.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3qetuxybt.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3yhpertda.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3nlenennn.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3cvucpkfe.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3nilnjgyl.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3jelbklvx.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3kdosafps.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3jcyyoogh.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3puplzhie.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3nxgkwmtd.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3orfqhjqz.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3lspgrask.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3wvhgcvin.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3unptgase.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3yvvzngru.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3modrppig.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3jmysgkzn.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3rrsxoyhc.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3nefflypr.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3pwojxtpp.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3oogvuzjz.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3opdoeccc.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3hfxzwziw.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3qidsmywp.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3hprvdxgg.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3hiindhkk.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3yqlgukgv.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3pfaiyjjf.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3enaoqrzw.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3gpqlswyb.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3jjlosqwz.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3dubgvtlc.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3zkrnwecq.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3hyderwsk.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3clwixocu.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3ssxtoolz.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3rzcvnlbn.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3dzqapcay.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3oxnkynub.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3zhitracj.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3edfonyxs.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3ochuutfy.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3iosqgnkg.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3mqeabiln.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3igznrdtt.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3dyyzlfhc.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3cqocmfvf.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3ompzdjqc.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3wricfmbu.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3oieybpmj.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3jqdcxkxe.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3ggnsiopp.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3xeqptvci.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3trefuysk.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3bgrbnzzs.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3aapwfgnr.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3qziznpns.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3fclinomq.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3vxiqhydg.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3qvgastsm.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3yavdzdyx.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3mttyekey.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3dtiusaol.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3lqbzsrqw.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3rsjikcwi.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3leoxdkla.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3rrosxdaa.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3yxvivqes.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3yjmxkept.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3skfjtodj.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3crqwbsrp.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3frrjnfbx.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3lcaehmgj.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3mrciwmig.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3vpjnmwdn.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3fubkdsig.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3oobogmnx.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3cgeawsox.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3pqsmjzez.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3wuykwynl.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3cqjebves.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qcmeglaq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3snrydbnh.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3ykcyqlgx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hydceyfp.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3uvxuzftv.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3kbgmoqsp.html


<!-- 参考信息 -->