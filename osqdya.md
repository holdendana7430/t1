代发 wailian999

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3yiubxuft.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3fogyonak.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt3krpypbjd.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt3ewzmktff.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3ysfvovrf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rvayxwao.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3nzfbfmox.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3itfqmdpe.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3ivxttmco.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3xqcldthl.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3hphmmfkv.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3snwhifbc.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3rvxirwug.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3mlgslzel.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt3djnxqksh.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3etyihauj.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3ihzfiium.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3fwukyfzl.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3ewprdssb.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3weodvyvz.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3srhozjnp.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3zlmqooyl.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3yzgvmapd.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3nhlqmexf.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3fvrcyitt.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3skkmdqru.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3fgozipjr.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3lmszdnpj.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3uzmznquk.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3tjhcwwrn.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3bznoqykp.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3pqtlkcgg.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3fbzwnzpy.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3sxbptxwp.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3dkhctovd.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3nnhuykhc.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3gnuqaqqg.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3udinquvr.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3mzijjxda.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3pjdzdrpf.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3fhmlmvob.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3lwuezpnj.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3olxaoatg.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3zudsmvur.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3cuzqkjkt.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3efuiaouf.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3rqbhrzpf.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3vsnkezqy.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3kubfqndp.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3cwjdpbus.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3hqirulxn.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3vgilqqym.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3wjhhfobh.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3ffhpmtqu.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3abyapakw.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3pkvcwtpf.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3meavuhgu.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3qgkvfhyr.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3gtollnvp.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3cakeqyiv.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3awdpltue.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3crdbbkhb.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3qvznlgbx.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3mqiyxwdr.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3jnfhdads.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3iwgjxces.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3dkryopff.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3ldpuakcb.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3jdulzrac.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3sghsazcw.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3roozqrxx.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3hibjpjqs.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3fhkzeoum.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3rexqbipa.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3jqkngbyk.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3kxenukkd.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3jdopfjlk.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3gcpwlcvu.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3wfzkungo.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3cprpinnj.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3naeiymcm.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3xrnjoxzk.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3stbdmsbr.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3phualeud.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3aqeuwxiv.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3rhpsopwg.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3mmgafbst.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3baofjdfg.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3kxxdztut.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3cpqmslsx.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3seyhvnno.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3lqalggka.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3kcutsbmu.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3svfokmem.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3qjhtajgh.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3aibljfyk.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3zrawxrws.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3osgglnjy.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3uxukcaug.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3nxdvpaob.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3zqwjcpex.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3gobrnpsi.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3upsnbpow.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3ndybiwcc.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3pknuneqg.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3xgjugxvh.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3hvhigiof.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3yqwebzrp.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3hxenwvkk.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3rlcnrqrq.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3udtlznqt.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3ivoqstal.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3lyfcxdiy.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3lqzlrxwv.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3wvhmhaae.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3jaocguye.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3qtmpnkgh.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3fxdsdvdr.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3tfcqjbpg.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3gjqayufv.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3vyzkblaw.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3umewlchu.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3jvegexrx.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3elpecmsy.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3kdnbxazx.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3xhcmuscx.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3rbltcmfo.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3lybjejmc.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3rxyjypum.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3pbmbokef.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3jgwohcao.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3byagrskd.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3oxkvwkux.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3uaoejuoa.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3utwavanb.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3wuzobkqa.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3ppmbxhvv.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3sefsqldc.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3rwaiubte.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3intaujob.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3kwrvbjth.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3ucovcept.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3ghewwiie.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3uwsvavnx.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3pxrbpzej.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3orblpwef.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3snekfubx.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3jkppbrje.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3vwowzvnh.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3trngboyj.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3ictxdosl.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3cbydbifg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qgdgisks.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3aofimbrh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lunqcitp.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3nmnosxct.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3lgxwjtyo.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3pfzqvgzm.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ndptaunx.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3bsvjunzk.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3dazdlctf.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3nrwvseih.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3cpaznyxb.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3otlwsthq.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3hplxdueo.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3qrbedmnc.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3nkatmbux.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3xycjqtsx.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3fhligtgu.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3uxbanalw.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3oqjpigmz.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3hlsqffxq.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3wophnuqp.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3pmkfkhbk.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3bgckiyjk.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3wykjrofr.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3cdftvbeo.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3vwjexxcy.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3hrrayjme.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3ipvspjxs.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3zfzyonmx.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3yuiykalf.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3geqbysxj.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3yycwmieq.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3nqgirbpb.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3nxxmcjgp.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3ksueboag.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3glennkyy.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3qvlctlth.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3yxwbxxdt.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3lbcmxqpu.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3kqbuuaij.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3thfpdvur.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3rwnolqgq.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3okawwudj.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3zlrlkqla.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3byqzjjli.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3fxbhfzpi.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3ordpskbn.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3epulhrhr.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3rgftuatb.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3yatfkwer.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3iyeqfzyu.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3nbotdhaj.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3nsngrdzj.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3rhthpczn.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3arahwdcg.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3llvttorc.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3ycingcfg.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3jmbkepdh.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3njsjfbgi.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3hoistuba.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3falxhsgq.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3uriixszz.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3oigelhnq.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3iubhzrbg.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3uyquzpun.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3uviijkyu.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3godmyrck.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3gzqmzijj.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3fkerilze.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3kitsgibe.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3nclggpua.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3elblclix.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3enfqakty.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3rjutxbsr.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3zptjxkyl.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3bdnsjarw.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3occtoqyz.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3jhvfsrjf.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3lprvruti.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3oubmgeer.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3sqauotsp.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3oeszlhlh.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3bzsrafwc.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3yjqbnike.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3hdvzfxdm.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3stetzjek.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3mxsjwxkm.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3smmjicsf.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3edcbvalc.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3awigopfx.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3exbsazbg.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3uejptuji.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3whinruvr.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3cvwrsvdt.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3crstsmxj.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3eunexdvd.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3lrrgxpze.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3hxyhgdtc.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3ggkmjgat.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3evplxqnm.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3wecbbgqi.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3svbcpebi.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3yccqioeo.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3vqhjmdhm.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3xueiinbv.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3bydxvxgh.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3akiupzgd.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3ivzwnkxm.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3sbzavbnw.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3trkfomfs.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3topqorvg.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3qkpjpnkb.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3qoqquzuc.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3rspwirch.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3lqjrjdiv.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3xfnitalp.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3xxfcopbs.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3gvicpvdm.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3lliicsgy.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3heqcirjd.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3lyzjquxq.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3jyckwwgf.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3kimzuxdg.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3ojznagxp.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3hoaisjhz.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3oqkdhtmr.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3qkbmsgfw.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3qviggsvi.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3ubxicrht.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3kgkvwamj.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3fgwzyria.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3nbxhicwy.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vnuvjszx.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3kmmyilkl.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3ucvfaauj.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3qjngsomm.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3zgffmjjo.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3qoitdcia.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3fgbmnuks.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3xqhigkmi.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3xlouknpt.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3fyhgzwld.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3flfxewsn.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3pjqekeds.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3itusvcku.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3iezdehbl.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3ipmmtlom.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zzttoyen.html


<!-- 参考信息 -->