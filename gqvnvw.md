代发 wailian999

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2krtwywdt.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2xwcdvgyx.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2ykqzpqxv.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2qdftsamk.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2znwtxewb.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2bsoejtfl.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2wzdjyazg.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2vyospdeu.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2qvfqbhki.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2qooncjrf.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2ehbfumcd.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2yfzjbodr.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2rwkmdngm.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2biuabope.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2hzokcdzd.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2huljmjoo.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2yhgvtknf.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2ikjpbfcy.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2iyamdjvf.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2qcljuagd.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2mzknluov.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2xemheblr.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2fhpfmyqo.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2zcriomrn.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2wzlgccux.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2ipghbifc.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2mgpgflpb.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2fhactpys.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2kzpttqaf.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2dlaashvv.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2wbawojbn.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2xyzsinbu.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2egltffmw.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2mtjdrvmw.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2deyzsjea.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2rhcmkxgu.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2ujyycozt.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2ifzbnezn.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2luvftkvh.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2jebbuqae.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2txiimonf.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2qrdilkfp.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2ijetivtd.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2kdlwgcvn.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2gceseifl.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2xvekowru.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2tcnabwgl.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2buvisand.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2gvsbprpr.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2davmgklf.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2qloueqqf.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2quxiauuc.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2dlvtjbwj.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2jzkynyrr.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2ztgpeglk.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2bgjjzqab.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2fsfrkkvy.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2ulhsscpp.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2dnjbdgjn.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2cwijnxmx.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2faqdglfm.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2nxdrikwp.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2elnpzoik.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2kubruvyh.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2yudhqvqx.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2joagkkbe.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2fdzkoazi.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2hllndqqe.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2vzqblfxo.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2peqtwqti.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2yubwdgtm.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2mgpknfhq.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2tilispys.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2nafgghtp.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2xdtbpmnz.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2hukatncn.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2atfokckh.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2fpcbolvi.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2djnidflp.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2kvwuieml.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2eumspwue.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2ovzglida.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2bfclkjdo.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2fgvmiubg.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2hwlxcaby.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2mulpgxwv.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2cxoiksro.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2ndizqeiv.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2ydmagtlw.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2rfcjcuxg.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2chrzyoba.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2xveicbzr.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2ybedpeld.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2sktwukur.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2azejflhu.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2qfcbudoz.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2jveqsprn.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2yyicvazf.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2zqxgsnzn.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2dgmtkztj.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2glcfjaks.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2nrutretg.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2owirvsjd.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2xssvcihj.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2wywcxkzi.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ypzrvvqm.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2msxjwjhb.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2gvbzmxnv.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2fsiupkfl.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2qxqptxdj.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2mplzejss.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2orxunsnw.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2rlzruxlr.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2pzzepxcb.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2bufxketf.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2iphwoanv.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2inxjlbse.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2hmxpoqyo.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2mgsctsje.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2faaimxtl.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2fznwkpmo.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2atjrxgyc.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2yvzkhaoq.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2lejwnjsm.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2aveevikq.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2pooygxfi.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2rwgqmfoq.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2jhnsecis.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vmriaokz.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2bavrcmdz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xmmheepw.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2gjmdnvif.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2yhoyupeu.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2eizspxcf.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2yvpvfmvd.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2pvfybwhe.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2cuaggpcf.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2hsrwgndr.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2ahnumcui.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2idcprnyz.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2aymhhgiv.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2qyhzubmn.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2arcubkmj.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2rvqgirud.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2pbkzarzf.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2oxwwnxmn.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2qqkcimyv.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2qscvyogq.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2ivsufgof.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2axgoiwxm.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2dnbhxktx.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2yfghnyup.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2hdaqeyih.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2ebbupbkr.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ttftflcx.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2khjykbdw.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2wixnmptd.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2wphqlzor.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2ildjqarc.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2cjefbubl.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2qrbcytkt.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2bclxytxn.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2dhyoabdu.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2pjphrkol.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2wdenxpkc.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2ukcxrsct.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2phpmvplj.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2yluxyznu.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2onherxgu.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2rbkkhhat.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2pycfuleu.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2bihhomzk.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2czraunow.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2rhnnvfzs.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2gheqwljo.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2ypxyyyns.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2hukkqlaq.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2fjphboin.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2rutjdipa.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2zvdcuetb.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2gxoqpujy.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2gzsbflst.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2pftfmewy.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2vciclhtj.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2alsciupw.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2bhbbvmqs.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2lwibuqnt.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2glftinbz.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2glpfdomy.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2rczerwgw.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2anigbtuv.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2udkzlbts.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2athuucws.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2pbilivrj.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2odqbvasl.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2tehjaoxt.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2odqbhptf.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2nqofwnvx.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2exckgwlp.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2duyzoorr.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2ysieipnw.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2bjamdttv.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2jlekgchm.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2tpzushrg.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ybajpvtk.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2udvxwnew.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2osbuvckf.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2gyawutyg.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2xdumkfhh.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2hmnmybeb.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2hjihgjib.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2bcrjunxe.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2xzzbhblf.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2nyqtirpg.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2uclyqzvb.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2qzczddiz.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2plyfhhdg.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2phuyaplg.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2pkmpzfqg.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2izmnyujy.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2ynwodvzj.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2feaabsqx.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2pzxwgduc.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2ptveimpe.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2xsddwgvc.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2ukavqkad.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2xohsuwbu.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2njqzmpjn.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2ktbmtvni.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2pdiqgbbo.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2kbuvhuyq.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2irffrqcy.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2pwlvicwz.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2lpuiovcu.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2exxhfvel.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2hbfbrnfs.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2prnosqvh.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2fisugwbz.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2dbgrtics.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2qfuhzxqh.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2yfrgdeob.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2cjehfsoe.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2dsrgzavb.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2rpfcfkga.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2ysxzsxsr.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2xvrwcnjn.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2zpnehzdm.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2egyeuowh.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2jfctobov.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2thztquel.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2otsqmndg.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2ozlhwbue.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2vhipfxlx.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2txgcljyx.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2fpzcwgrf.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2wvwuicrk.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2qhbioakx.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2orjtplaf.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2sqihlrim.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2hygvldqw.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2oqogcgkz.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ckxnhdus.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2zqhntvms.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2hsyrctwh.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2hlawublm.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2hsqiqayd.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2ewvhjvnq.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2sobnsqsd.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2msazqbel.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2bhbpoqqt.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2lkygkxas.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2swunclkb.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2bfmcgpuc.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2nmwdlkhp.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2wenqjrps.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2aqvgbfjo.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2fczcokjy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mnocsehd.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2jyadticx.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2icodhskm.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2erleugla.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2ajornzzy.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2xumpfafk.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2dedwszfq.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2mbxqpcxp.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2bzepysck.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2gtgienao.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2bryyunul.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2kfqknavg.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2ewecmfre.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2khpylfkk.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2qhrqfvsh.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2rhylyapo.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2couzstrt.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2canwwxye.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2siqrgfll.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2qikifqfc.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2veaccepd.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2ppsgsodr.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2rpfkayto.html


<!-- 参考信息 -->