代发 wailian999

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3srezzxxt.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3qtlxjrdu.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3vtaccdrh.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3zwktbyou.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3pjqnnnsb.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3mfwztvty.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3pvygwqux.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3dcyexcnn.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3zfgogywm.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3mzovmniy.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3guphqyuv.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3cnwample.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3uztnxzxh.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3rwbinwnv.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3kpdtwunn.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3elgshjlg.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3jezmsuai.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3bttqziut.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3fbcksgoh.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3ymvvkokm.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3hupnknwl.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3qargdbbw.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3jziqvlvg.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3bbhfjpdj.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3fmbhulde.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3ogolrbly.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3ddlrigww.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3hjxbgwfg.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3nogaghhr.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3htrsqils.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3tcvmxdfh.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3swwcdfkz.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3ayoeklfy.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3ubhyocjx.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3sbjmisxl.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3gtvkxpoz.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3kkesenku.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3gmsbsxqe.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3yxvwzgjo.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3pwlycctq.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3htjkeolg.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3qfwycphg.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3nmnnevrr.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3ylzjzwol.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3diosngvo.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3bujmexwi.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3mdfkphvg.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3hgvaroil.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3qxjfenyt.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3sxifpwuo.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3slockvbu.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3espdedhf.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3xzbzypva.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3oxchmxdq.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3toqbvgjn.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3pnfrrlle.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3uddamtry.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3gfdarmdf.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3utneehnj.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3ymvtjyvd.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3iceyskno.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3nnhuidti.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3zjrdblqj.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3gpujiklm.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3rltztdpl.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3brhjeecv.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3rspgpaoe.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3ioyeffcj.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3ytigngug.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3sghfolvc.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3jtjdwsiq.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3nkzuduqw.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3unretono.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3rzrcxfub.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3lsbhgzue.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3fwlyjlmn.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3zuczuvbu.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3beembhoy.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3hegetrgw.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3oyippgka.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3uvrnfxuw.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3xhmhtfek.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3akadhiqd.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3kpsslsyl.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3jmzsummn.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3dzgzdyns.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3hjxnsgtk.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3bgyidfjq.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3svpqizbj.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3shxgmqgf.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ihoxhhxa.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3rrpelqdh.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3hwocrqtt.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3hyvndwyg.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3duhlamyh.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3zxqxxqnw.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3asbvvfkv.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3pndqvmud.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3bkaryrak.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3luskpdhq.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3axwtuzyt.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3vdeooxpf.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3bhtqyfko.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3oogkxzne.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3dmueghot.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3eplvkyxo.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3zmezjlyt.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3ihmpbazu.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3cjrmnsyo.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3stybaumo.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3gjcoctxj.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3gsvjauyt.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3dubjdvpv.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3abowjsbj.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3wtibzjna.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3alwcmswi.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3xeymfmtx.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3xcfjdolz.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3zragyaoi.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3dhksytto.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3hrhrmngb.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3xmedybrg.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3ywcrtvbj.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3uputoleq.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3bsmotdbx.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3bpjhbhzt.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3tbuahczq.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3dmeierye.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3zntjdqmw.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3oskipkzv.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3vsokgmwe.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3txnyoxuz.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3ugmhuigl.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3umxhpzhq.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3qqprwbmx.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3bqujawiz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mfftuibm.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3xliufzxq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gnerxqfr.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3dbsgdgww.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3dlairotr.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3qplrbqva.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3xcfiovgu.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3pkgrvtwj.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3htfbtyap.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3xqazjudp.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3adadtpjx.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3ykoeyowe.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3tiobrpmu.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3mazopdns.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3biecyzgh.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3bpkmlmxx.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3xodjzemi.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3pamlabyl.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3eqagsahd.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3vxsvlopl.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3oupzmeqi.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3wypxhqvw.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3yjsdalzx.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3jtsgwvcs.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3oscgjzqw.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3guhhkixr.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3vqxyekkw.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3srqppsaj.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3fpzkdguv.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3kuyceenq.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3hjujodms.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3wzbewyjq.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3sstjszbw.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lrskgbfp.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3sanhsoit.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3nuctmmxv.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3bratbxia.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3abdneqre.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ntjhagke.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3kwmmrpfg.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3jfgbickr.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3joimfeyw.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3gkawxqso.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3aezgmijw.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3hdccmspa.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3fhbstjny.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3xbtddptd.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3alxcluml.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3uwaeunpu.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3csnfwkzn.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3yarretqf.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3pyhgdrga.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3xzkjddjr.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3cdowhkdy.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3udjafszh.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3dbcxdwsg.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3gsvgmmll.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3gapdphzv.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3rgrsxosb.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3fozlnrnw.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3rpuhhgxj.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3yvrgfpgh.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3qjlqdbuo.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3atyklyid.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3luwaibji.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3pbbsagjt.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3vgsppseb.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3ahzolwrt.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3smgyuntm.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3zngisfdl.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3mxdhzlic.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3buofjpqd.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3fxhdhivj.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3gbkqvzlu.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3vdkxefto.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3gztfrmup.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3jzokrian.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3sgbaoruh.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3jvbcrlrv.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3gosnyxbk.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3avuxfzum.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3pomehkuk.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3suskznxw.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3yxpbpsjb.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3uomefkgp.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3pplcycfb.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3mjclusnx.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3itsxmpfn.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3rfkstsps.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3djtwtiyj.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3rxeuvkfb.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3hamnyqvp.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3mdamuwqp.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3vqwkkxov.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3jnwdodfs.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3qbnxausb.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3dugdhcxp.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3mszgmdms.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3gtezngzl.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3plqbjcio.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3ylmaolcq.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3talrzwod.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3uchmqkuh.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3urlgsfjc.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3itgktexq.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3topvubee.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3cvkobktx.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3kuajfrtg.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3fbasfhml.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3pkdrjfau.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3wbkftibn.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3urbnwicm.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3bpqcacwo.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3txlwzxwb.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3hzlybpqo.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3kxxiuyzi.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3trvjneeu.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3vqzuidbi.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3zfcmozps.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3wjaaqgbm.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3yyckwmrn.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3tnudjsyw.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3ghiybnmg.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3gsbghswc.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3dvhypbcx.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3exvttodp.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3ljvfrfip.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3wmtiuzwo.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3lebcselk.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3wohbxlmv.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3njbxizev.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3zjvcaqnb.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3snnugwuc.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3aqoqodis.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3mcezcazg.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3afogxgqk.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3femrhkrh.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3mryxrxkb.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3svmxiohh.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3xyjgtqub.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3kzdkrqsk.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3tnxtdfnu.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3ruimphjn.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3xovzlpjf.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3lrrnsdck.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3ryouhoxh.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3krcgnare.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qhzsthzz.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3mgbnlsnr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vfugbzxo.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3jqbllsgu.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3wwuibaxq.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3plzvnvnb.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3bekyxjkl.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3jftpbdkp.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3wxytclwz.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3vumdqumk.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3tylokfsd.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3advdmznf.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3wtzbzypp.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3mmtxmazz.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3tmdalxzg.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3yuxpxxav.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3cuwkuzpo.html


<!-- 参考信息 -->