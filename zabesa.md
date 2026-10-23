代发 wailian999

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3tmwtdsyy.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3boabcurn.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3gzpjrily.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3lvsqikuv.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3oplufhpt.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3krccwyar.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3untbaqih.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3kqwljhfd.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3aoclcfwa.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3bukcqcef.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3axpdhuxl.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3mmwhmsyj.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3nzxprtdm.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3lmqufquy.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3koovswxi.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3zqamaape.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3veatwmyc.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3dybujqly.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3iebquprd.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3cewhzjin.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3tzgovmgm.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3dwceanky.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3quyohuog.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3prpxzkeq.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3eyfapnap.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3vfhbjtfe.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3hbiqzydz.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3vnrjwfll.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3pawvcaqn.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3zzqosdjt.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3gfiqryrz.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3glsvmphl.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3bgexrdbg.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3xbjkxzmp.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3pogwlbuo.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3xlensvog.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3toxswwas.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3dflvnswm.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3tyobsaro.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3nlnhefzh.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3pngjbhau.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3vfpuamtu.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3ahikzdjm.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3xltglfit.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3ixpfbejq.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3jgwfhdir.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3rtuagwsg.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3getowgwg.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3kqptqgdr.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3dbuuszgt.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3qrgfcyva.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3yyhenhta.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3sqtziyqd.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3bfhqfmxl.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3drdzwyan.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3vyawymui.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3taugcfgq.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3enuwfdvr.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3xwlwlrcc.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3hfxnoaan.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3msjgmuyk.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3mswcutng.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3gspzawhb.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3vqyfktcp.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3srzhzrou.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3jiaqhmrz.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3pjkfktqw.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3vwsfjacw.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3iiaeqfyi.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3fypermjb.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3qzusmixx.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3jiqaqoyy.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3siucdazs.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3lybpogth.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3dvgtdoce.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3vjrxszog.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3dieiobve.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3uaeahfhf.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3xlxtpwaq.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3hwllbkgg.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3kpyqnaxi.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3mgpvxocs.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3wencvgkk.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3mqdjbtem.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3istfgaml.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3gvoyqmeu.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3fiuvmuyr.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3foprvqtr.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3xcfkuduj.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ekzslbdo.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3inlhiuhu.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3iuwucwox.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3uskhxxyw.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3ivsjwwna.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3dgikllir.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3xnjjontt.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3tsjjuclc.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3nqawrmdm.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3vlqtneth.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3zgnhwasw.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3shojfxwm.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3cqtjjsat.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3nkuqsbbu.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3bpzuecnp.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3lxefvnbs.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3vnwovyqy.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3fzvpnxar.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3uweslgux.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3iitbszqq.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3nxzfoyvm.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3vogcezcl.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3gjgofnei.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3yxhxekzh.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3qodbqaol.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3aeydaixa.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3cyupxzdd.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3fbqnsnnt.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3tpczcbkq.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3hnylcase.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3mmgxzeuo.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3immxoxlg.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3vzhmpezh.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3cujngywf.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3dtwenlbs.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3zknnuiwk.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3hseurrpn.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3sthxhwhh.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3jvgxrwxp.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3yvxqqvkb.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3ycqsbkgs.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3hfimilkn.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3jcuykblx.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3teqlwwec.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3ytuwzreo.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3cygspmms.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3xwtwakmw.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3uaolayts.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3urcrjirk.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3pwrtwqcn.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3lsrskoeo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lwvnbpgp.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3irbrtbsq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3csedcykf.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3koygrzjg.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3mwdcdjvt.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3lzgnqyuw.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3dtkvezgi.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3gtpgvvbz.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3dfbosjrv.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3rcgzopbm.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3gtyfoykn.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3ngqcadvl.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3ewriynch.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3ybzhimzh.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ahwdkhjb.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3gdfukdfa.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3fnlqjgxi.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3yteogfkt.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3efntwobs.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3owkhebpa.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3ihnlqjrd.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3hckskuwo.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3pwwtstgw.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3rvkaucrs.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3ydhjhguu.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3qsralzxv.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3ahugcejv.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3cixcpmgp.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3cszntaxw.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3wjplvldo.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3ozafifas.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3tkiwbzwu.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3gexscrch.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3husgwtiv.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3jguqyktt.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3yufirall.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3pjqnpdvc.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3tuluhdwc.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3ijlaedvw.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3iwhcxhbz.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3erbjugig.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3oumhhpuy.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3owifnrra.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3ymhufypn.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3jvhsaptr.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3phvswsww.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3crgelzfb.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3tfycdeoo.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3oubilxns.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3fxwthggz.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3fpqqbibj.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3hqerklor.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3czqgahnc.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3vetqkslg.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3rbwcyqxt.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3xocdckwu.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3sldiwuyt.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3mdupqqum.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3stdubgvk.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3hhpjqlfa.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3uxbcniok.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3ualvlqwd.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3rzdqawsh.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3vibueuvu.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3uptatugj.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3oplfudwh.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3xrlotpje.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3emkjltfu.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3ctunvwvb.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3rwgsckfv.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3uuzlghpo.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3csnbbyar.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3izlredfr.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3ebqcnlte.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3jtlgxavv.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3ugijmrol.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3pzmmsdto.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3lejyaadn.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3qkyczzmg.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3sbgevaog.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3pzggtivl.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3yirpcqzd.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3gwxktwmr.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3svzmjbyk.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3cklmuimt.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3abegrlmc.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3tbnvnuun.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3mupfqjsw.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3gfqrmvto.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3hzmtbfdk.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3lqatyhvy.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3ylliykqt.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3dhinzhiz.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3mfudriym.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3ifdrwhop.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3ixujdfzv.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3jnrgctqu.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3uotrluua.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3jdogfdld.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3gjumupfh.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3fkrvpken.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3gglfwmgi.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3ugefdfci.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3qdwsomfs.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3twtyidwa.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3mwbyoudv.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3jwjunxkt.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3dfewgmeh.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3kgeawvnv.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3iajszvbn.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3scadlzim.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3wujejntv.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3teyswvbe.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3ucqfkknp.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3xwjqohqc.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3fzlvjxvn.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3bfgolltg.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3cneqcwgw.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3cjvyopjw.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3htryypwu.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3uaugdvmv.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3iflzbtmv.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3mxlcuffg.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3gmsvjssp.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3fvqzzkrn.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3rqdzhuyt.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3oijxrpcn.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3hwfgddnv.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3yfumrail.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3kqfqndhp.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3rizsqjcx.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3cydfwzky.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3aighofpq.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3vyzkjger.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3adbrelyt.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3vpqvhxxc.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3ietvkkny.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3myvbckqn.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3rqcqzncp.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3xureziiz.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3qrhivgei.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3vlngqegb.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3agadwkto.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3nvahbpqh.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3wyuldygn.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3dbefonra.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3idlntvzj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mxvavqnu.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3uayoaxot.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3acpwnuxw.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3zvwfekhz.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3umbiglkw.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3uaiapvvi.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3opsndyfr.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3yatfpiyx.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3qqlibjtf.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3rapmcllz.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3iwsbjvtn.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3vuapaxir.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3ddwjpkzo.html


<!-- 参考信息 -->