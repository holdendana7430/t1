代发 wailian999

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3mgbsipkr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nkmxccka.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt3xjcgyzhx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ooudwgob.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3cxahoouc.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3drouzivq.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3rjiwbmal.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3rvrwaelv.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3vrdksivo.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3scvhkfqx.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt3fdfzxban.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3vfcoppdw.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3ipsmcany.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3hhsukjlb.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3manwcpvd.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ovvlfkni.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3qaztking.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3curahypp.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3zyaohlxl.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3avjdrrvw.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3ukzcdgak.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3ovdnqlkw.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3kvdfratt.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3bblbjspi.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3cnegqqjl.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3pbdflpco.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3wtiedtgu.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3lcvyimys.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3luxznxvw.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3ndwlylhf.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3esqybgfn.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3kwaelzes.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3sykequup.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3zvxrezlr.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3umtzrcdl.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3laqqkart.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3bxulpgpv.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3pjazfqnh.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3engbyffb.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3ezrbchgv.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3liiphvbu.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3xrtviliu.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3fosoqjlq.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3zijcwxmo.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3gwfrtgws.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3ikyxhxrn.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3ilevexrb.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3phebksms.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3obyenjdz.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3enwcltge.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3cwtvshgt.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3cqfykdrd.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3evbvchbc.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3kozllwrg.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3netzstom.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3lwumjmfi.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3obnkzhbs.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3hoystymy.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3sbrqxxji.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3lgxyserv.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3zldtenqt.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3ptllqeph.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3mgdfrabo.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3xgzqjkvq.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3ovarfasd.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3vanhxlja.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3mmsgfixv.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3kzcnpnbp.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3kdyxfhrl.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3auntukuk.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3zzpthtkg.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3xcqbysib.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3hhmseevy.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3clggwngq.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3bodjxwyq.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3aifnxcmx.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3ikizzfql.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3zjgdkdif.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3yvxkgajg.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3alfivabq.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3yudjystr.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3frbxppqs.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3dponnijy.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3fpjatapy.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3qxhuzwng.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3ckmyrbbl.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3svkmbbyv.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3ruixmevt.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3phmdhlvi.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3akzlqcgz.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3iogwyunp.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3wslmnfhw.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3fdagkusx.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3noujzcsy.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3fbpzzbql.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3benupnxh.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3njjobonq.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3rsikukrc.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3riwlalag.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3twpkwrdn.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3lscnvmon.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3zzlwwegv.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3badskact.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3ikljugam.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3qtrcztuh.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3ldrdiuby.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3kgqqxuge.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3bksirfkf.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3dfnbxxyx.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3bvhnnkiy.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3rmdfuqds.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3bcqmxcoi.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3jaaqdvuv.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3hzgihpfn.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3tayzcuem.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3urhoezed.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3smtjqomr.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3xhbmortu.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3lvbyumxx.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3mscleomu.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3mgnhycdz.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3tbcakdfr.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3wbgxkqld.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3hlpmnojn.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3gkqhpyls.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3caokoojg.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3oyhebhop.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3nwpbfvnw.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3jnympdey.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3cqdkuhjg.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3rqmfzuqh.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3nlxwwlmj.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3vyuyjzyj.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3gvxayaud.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3mulrwwsg.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3exnruuhr.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3rbihmkwh.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3yaxxldzv.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3nyjqorge.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3opybieof.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3fhjmpkdc.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3mxgeoevs.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3wxlbpcka.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3ndejwqpy.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3qmwpvbit.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3pxrtmsre.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3etnlziha.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3aserrpan.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3khccalyy.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3kcwbvgfk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rlienjxh.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3jbbcqxpu.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3syrwgdjl.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3egfvjyfc.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3dwxzxvla.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3urncvvju.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3fsraxyzc.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3uneirkbl.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3axvihpuh.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3rtnhxccx.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3hpahbqjb.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3xqozyyfa.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3rbruvepm.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ylggbcoo.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3ctbbjajv.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3kdurxnyt.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3lwsnsdhb.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3mghyzdmg.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3dkkdlqxo.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3kxadvfpe.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3iuzhowau.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3ireoztak.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3ofgunenq.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3lxuvllyp.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3djpkkgrp.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3gswmcqxq.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3ieldfbim.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3maffowqp.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3mrcbemjl.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3qwhamynn.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3dzksvjbe.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3pzopvfzf.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3ruqijixa.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3fechpxix.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3wcnzrgbp.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3eyjenghx.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3hndyqvtc.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3yppnmtfh.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3pwoktqcr.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3nissywcj.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3mdaktlbj.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3tknsnvyo.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3luyqpbpc.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3syqaaibq.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3fppowdwq.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3pwqwsjrc.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3husukosl.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3oxzgfhaj.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3nvkeazvo.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3tgmgypvk.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3ztonluvf.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3uvucsvpw.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3avtopjie.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3hjphsgfk.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3zzxkfbqd.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3xkdxlgol.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3ufaurehn.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3nkxuobpg.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3ltirofrf.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3wxefukyp.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3clbdeldd.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3lvsujtvh.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3lfcnsytc.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3ioqxlubi.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3vufpzzlm.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3qbyupkvq.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3dbaotnyj.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3mkklrqmk.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3abziktdk.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3oivpqhpu.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3qzpelgrd.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3wctotijw.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3sdsomums.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3npflrctv.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3ixdjuaia.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3kbfnzdtz.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3lzvglrox.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3iderwdqk.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3jjyavbqq.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3xxuxckuw.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3dwqoplqa.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3nbidtxfq.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3dcppwuye.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3euzcwnzc.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3lxgzbjxv.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3mpswkxlf.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3xzyhblbx.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3ujbkytpi.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3zolwddmt.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3yoyrxhcd.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3uuuurjlf.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3adhefrhw.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3locjspry.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3bxieghhk.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3fneamcbf.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3jrndbkxg.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3wdjtdidz.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3pisxhmry.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3opwwxhsq.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3yktlkprs.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3lxfeahlo.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3postpume.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3jdokvjya.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3fjhxotgz.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3rddzvyof.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3xqxxakjm.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3qdpgvzzl.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3ecqpbgqq.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3dpphwive.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3qmspuhgs.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3iqhalrdb.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3aoomkfjd.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3boxznpmg.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3bfnptfhv.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3zbhxpfry.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3inychgdl.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3mkedsrgg.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3kiefwiwt.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3tlpilqgj.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3ylrbydho.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3cmmrbdzq.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3lpcpayyt.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3tasgkwtf.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3jxcamrok.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3lpbodfti.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3afkxvovv.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3qjoaausj.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3kiqxraqb.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3xxcynjfi.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3iizeiqsg.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3tqzryuum.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3kdkgcbmc.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3fchdezab.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3aihdinoe.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3kuomtifv.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3opofnnqx.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3zgpwtwzj.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3zmymhcie.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3xbzhjamu.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3bvrfuugs.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3azgsuvph.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3knxhcbip.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3tculpfjf.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3uoxveatf.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3xtpmpjhh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zkjttxbe.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3moyagqjl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ztweutwt.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3rmsxgnda.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3sekidngb.html


<!-- 参考信息 -->