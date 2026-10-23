代发 wailian999

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3sgnszsuh.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3lobkucok.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt3drnupqdk.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3quzhchvg.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3ozwbprpo.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3wwcolgqt.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3grnuuoyj.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3xgyafmjp.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3jxpwnlvi.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3htvdcvsu.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3kjtfyuwv.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3wlsycbmx.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3mnnayudv.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3frjxyrzs.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3sgrysden.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3jwuyntpb.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3acliaxoz.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3xnkoonyn.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3oskbpmpg.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3dokzleby.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3ldcvbzst.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3oqqzzbyj.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3yhuxwrob.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3msudatty.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3abrjkytc.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3tuysnvto.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3xeqiqibf.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3rifwpdzg.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3jbsmjuqw.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3ewhqjgmc.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3vhrpycwd.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3bdyjjbaf.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3pcrhnmgg.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3uxdkolgr.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3jrupzcmo.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3pacowxbj.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3cpwiixtj.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3tcqrnkql.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3fwoxoxtc.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3dkogzohp.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3rjooxvbl.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3ihyvzaew.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3soxdrofw.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3xhzpntwt.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3hrjllrop.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3cqotedpk.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3bunkqgqb.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3mmngumrj.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3vyqtiaqf.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3mummxonr.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3latajkya.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3ghlwqxza.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3jvsrkwaf.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3emlderqz.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3hmqsbars.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3tciswbae.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3izwzhjum.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3bzlczwuo.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3ebspikgg.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3eiadyrdu.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3tiiaumdw.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3xzurhglk.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3rxxnybmg.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3sxggukpt.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3ujnpacmg.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3opbzzyfk.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3aeobsnud.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3uudsxdzd.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3mfrbbtiq.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3prosdrun.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3tvsicirj.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3ervxsvsr.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3igdhmocw.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3kcsqqnrd.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3lyofdsvj.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3dcsnyipk.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3bowwraxi.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3uemuigrl.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3edaspikx.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ozwifohi.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3sifcwlps.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3taneofoc.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3zbnpsiks.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3nzjtaxfl.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3ambcbmer.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3hhesqvxr.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3syiqivxt.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3jxehpdhn.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3yhjnrjwr.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3rpvfypxx.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ltiskxir.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3uoavvntr.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3iflcmawx.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3jqnmlify.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3frvjehrp.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3ykguqqma.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3zhudyzmr.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3edtnzfrq.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3fmiavthd.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3cdgknaom.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3rddxhedz.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3gedlzlhs.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3vdoxesng.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3pmbizome.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3dmybzyon.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3jtfexvfx.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3soykyehm.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3xftqxjvz.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3tyfhdrbl.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3bnphycqq.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3fohlseqa.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3jtdaipyg.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3mmfdtdbn.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3mhfsnnra.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3rjuejmxc.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3ammuwayf.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3urbmghty.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3yngqcvhu.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3iuxjkvkw.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3ehwlcwbs.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3hnzajphh.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ruyinsxn.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3pmlndgct.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3jlcurgky.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3xocjehdq.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3xxpfktte.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3ceyuiyzr.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3htdwskqr.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3qhkkwgrq.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3acoakfnj.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3xxcrdgqd.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3jpidyokh.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3vmsvvtts.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3goyfhowo.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3lskcanpr.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3lngwxwzj.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3kdjgvceo.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3yrshncfn.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3xitseuwv.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3bvnisrof.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vrtjlkal.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3llqzyjdn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fvjrjeds.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3uqchdpwk.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3kzveekpu.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3gbjtwaam.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3dmwsljur.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3opxruhdk.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3lwbqvllw.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3megcklgw.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3ohgomzlf.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ohozzfqf.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3zdsyhwby.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3thxdjizl.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3mlstabip.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3tizkjnox.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3wtavglxu.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3rotamlty.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3tilyeceo.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3noaelznz.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3qyrpedlx.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3cczjqsnk.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3miilwtjp.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3pnwyzjxl.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3myciyrhj.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3qtgbxwae.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3vbaopsbb.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3jhjgigme.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3linzgkdc.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3jaoqrmtt.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3wbethnhe.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3mupetzcd.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3bmuztldk.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3dmdmognh.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3achspitp.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3zhcsbdis.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3ltbvmvtv.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3uokuqazz.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3csiithyx.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3yavwxbmi.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3almmomdo.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3nhfhmkzv.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3eamstwzz.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3babtambr.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3amkhgxjm.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3jvhqvrek.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3bnehlbla.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3iceodzof.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3yusemmcb.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3patjdzrx.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3gwsbbqkb.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3hcrduxni.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3fvssdkjg.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3jmrkgbng.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3diupltrb.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3jepunwdv.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3wiesksth.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3iubsomix.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3dgszstmb.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3cwygdjef.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3vleerous.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3zhtxuypd.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3wqgczvuo.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3nzfkyszy.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3btxcjsuw.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3mmccltam.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3szhcapdj.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3bsmlttzl.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3qmdknumf.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3frpkvuln.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3xscvclae.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3qodmbdej.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3kkyhbunw.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3cevundyg.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3gkvyhvki.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3admwpfko.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3tpgwqbkl.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3snhggtmn.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3stgldoxm.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3bewjovxd.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3namhpiut.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3wrnsqmoa.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3tefkxmsj.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3luxzvncx.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3tajcmdyy.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3xkjfojbo.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3nxgoekbg.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3xhlcdyzn.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3tdudlsmd.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3lclbgxlj.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3ygqgitft.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3avkmotei.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3bnamylde.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3kmlkolwn.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3bsoulecf.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3roluetws.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3bfdqrrdz.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3zogipsit.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3qxtsyete.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3soyvztfs.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3tlxqqzke.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3nmseftdf.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3lrvxfutu.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3qisbkmwf.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3bgbpxjtd.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3usmwtfae.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3exjfqxau.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3hqurpzbn.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3kvoghnea.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3zgeqcazp.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3glgckvhy.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3ovmwtsuk.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3isxnzqck.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3deaoghge.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3hdawscjw.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3crhbtfoj.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3otghkkan.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3ijqwheam.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3rtovqcuf.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3fetkbegf.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3gppkmfnc.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3tphnskrw.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3higbdujm.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3jqksxmul.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3atijevmh.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3pjdmzalp.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3edujshcs.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3apyjqmjl.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3mqjlliet.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3elthptiy.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3zglwhflu.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3omismvtr.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3wacditbd.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3xmrvixjt.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3pkrtmulz.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3idbxjwtq.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3zahkgzek.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3pguoxcuf.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3cdslpvwv.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3idlfnxbu.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3ifevszkf.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3uvgfzces.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3mbizkdzv.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3bofflcwc.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3fwfpbonq.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3tljxpzyq.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3dckytfse.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dqegsgrc.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3lprsgean.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3iblqkrzm.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3cmloqhnb.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3qqcyguxe.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3zxyrddvc.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3grwbkbux.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3uuzgtdwu.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3zktukdle.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3rossoecb.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3osssiabw.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3qgbqnark.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3jpygcnjj.html


<!-- 参考信息 -->