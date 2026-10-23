代发 wailian999

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3erqucxsy.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3lscvgzex.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3yyjwlrgg.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3tbksgarj.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3wfxvfgcv.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3hzdtdfya.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3hxrdcgvt.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt3jadexnzs.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3iwnlvwgx.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3ztsdgjsh.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3twfnqqay.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3eqckkpuw.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3mnvvbbbh.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3xxkjpzxv.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3gaxjwflh.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3upjujbos.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3bpchwrix.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3moyxqlcu.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3ffietaqd.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3zihtzdej.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3piejucrb.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3lwamdcra.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3hkjzadzj.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3eueuqbgi.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3xlujnbzl.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3krgeobfs.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3uuxguhtx.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3dyvlbxhv.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3efbhjutv.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3exyzbxmi.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3unjpfzaw.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3eeschokg.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3vnzpplbs.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3oqbywumo.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3rumvraio.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3nvnzgtuw.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3ecsptkgr.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3rqzyslil.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3iqnjjcnc.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3mgygaunv.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3frkreezd.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3qgyawibm.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3hqtelzjn.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3oqnkrsem.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3mvczhenh.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3gszvqhqe.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3fonkclyy.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3aehxeupf.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3uxhjytbs.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3dlicetyq.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3uirgnjnt.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3whouwscu.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3qibxrmbi.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3ukdamlav.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3znprqgmm.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3qrzlxhvx.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3dhutrgxb.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3agxcbksw.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3zcmqkbns.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3dxuahvyb.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3flsercnf.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3oznnkklt.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3dtvbwofj.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3ynljhtwk.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3ueoenifc.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3ftmdaiyh.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3bddqduas.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3knmyawgp.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3iswlufxl.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3qttyzszy.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3bvbrhsyw.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3fyeieysj.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3taqkaavs.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3cbkxwfkc.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3dhhldlva.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3diommmlt.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3twtygjjh.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3ctbmgwao.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3frfapzvu.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3wdcuusbq.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3jvejefqy.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3mfdrtjnb.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3bfnbpxcu.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3navjxrhc.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3tbitgzth.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3mqchnzaz.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3pgbogepx.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3edkkdsyx.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3dxurfpff.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3petrdkms.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3tstdwnax.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3ddputwsu.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3jwsshegg.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3gtoktmey.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3xmwpamth.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3xbponpwg.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3dcyplcva.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3lwaakaqh.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3mpopystm.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3fsswbosx.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3kkwvakrf.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3glnfxsqp.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3nmdupxdx.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3zkywdxvz.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3ncfrcgcw.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3yzkdqlgy.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3aczkvhef.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3hdvoqvum.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3kbqjkygk.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3opybaevt.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3yzmaiukh.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3bixahcvh.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3olqrneje.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3llyvntay.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3ttxdlsdr.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3wljgawel.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3okzrdodl.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3mfighcxv.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ggtzyraf.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3siqwqdpd.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3ayygxqrq.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3pqvoqfsm.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3azlhspmh.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3hwtepalw.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3gqjhrbvn.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3sajpsict.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3ttasdsnz.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3pvmmbnaf.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3ygxnsywt.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3lunmvsxn.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3yrsvcxvf.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3gtjcomwh.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3hfsekreq.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3sqftoqvo.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3doscfwig.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3nxpqskav.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3upbnpedb.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3zphlzpiw.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3kcngsctp.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3obsazkpw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bzcahwqo.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3vfbkkgsg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yofogckv.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3oirglpvs.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3homlnoes.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3jxbavtqi.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3cvwmoscq.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ssloxicq.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3usqhcbdm.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3waqmhqtf.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3qtevnzrn.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3yzelqggk.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3lxgbeysj.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3hupsozsq.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3xuffmtsr.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3iswoustc.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3unkwufso.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3xydativr.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3vgkkqvkf.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3bgadumor.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3aeakpabc.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3lvsqhtia.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3nhxwmmxf.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3wwgoftnh.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3gdwmxlya.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3qadwegak.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3mfqorkxj.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3esfhhwrg.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3rmhjvydg.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3uofpmywr.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3mvnwnrpz.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3ccwkugcj.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3bzbdguaj.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fquafwkd.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3rmhkzujz.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3rinsjnbi.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3wfuhmict.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3zmjhjwoo.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3rekukgan.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3rwououmz.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3vbixnzro.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3lcnuyopa.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3wxlfjrrf.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3izwhthzb.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3lwzufoke.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3gagkzhii.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3wzwjexcc.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3auodhpok.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3fptwrofk.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3fafvhpon.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3gbitcstf.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3xegeptcf.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3meayedfw.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3iallxucd.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3egyccrof.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3ltlplnjk.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3ddaoddxk.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3umdotfxq.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3jjauopiy.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3jfsmgoub.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3gylcbgoo.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3otwmafcu.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3oahnennj.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3aeufqdrg.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3zpvdztjw.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3gbfrfxar.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3bquuzyjh.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3jkmlaiym.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3obgjuyqd.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3pjmulwvc.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3sdzmkxdt.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3modwftbu.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3jpnqpyfk.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3vnjsxwzg.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3poecwfzm.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3pilqmfxc.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3qtnddead.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3jaozdhys.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3rpkhbcok.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3kdhbariz.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3limqjfhi.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3knctkagv.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3dmxqrjvm.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3ndlwkiny.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3abaskxjz.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3hscptzdm.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3oppntfon.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3vijananu.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3ykcsztxl.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3cinfewmw.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3qqwrsisf.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3yzowgjdk.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3cokrvauj.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3xinsncwi.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3rxthezrl.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3hcniifkv.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3aoqqfxtz.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3bxepjrri.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3vljjvebc.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3dxjcehli.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3ngzxgexk.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3njaatlxz.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3lewxkcie.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3xslpmkzh.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3yrwvunzw.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3hjxgkqhi.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3sbkyhulq.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3huqmkooq.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3gzxlkuhc.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3nbdashby.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3czxaujud.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3ehcgggvf.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3ntbrqsox.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3ioelmhfh.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3fogsaowp.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3wnijbbeg.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3xlxappfr.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3mlnmmlad.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3rblienqv.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3fjrjquge.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3vwzckomi.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3bluxgjnu.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3gfggpklf.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3hadzubaq.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3wbvdidbg.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3wxmnenwk.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3oisdlxde.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3yuclyxsw.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3xoizvvhc.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3iqxmzhxp.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3pkgovopf.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3onpagifk.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3wrzdzbfj.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3znepjkmk.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3hlebywfw.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3piuyfdrc.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3vevcogml.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3eytmzcaz.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3rtghwjar.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3bvpchouj.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3vxqcveek.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3omnvufsm.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3catgqbqr.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3ylrxcfrh.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3rjvpyytx.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3xinwtwco.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fnqfthme.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xvjvqnaq.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3csucstvu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ndhzmuow.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3ptqdgjdc.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3whdmluyi.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3utxlaera.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3wclgacpz.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3mvvisism.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3hrnoaeqc.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3dyhrmcod.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3hgbwefmh.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3rbzwuldw.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3cqqqanzf.html


<!-- 参考信息 -->