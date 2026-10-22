代发 wailian999

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2sgqnzvcf.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2pmmqlzzk.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2vtkmyglg.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2mfwchnuk.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2sneepczr.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2suhsblbz.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2tuvnyppc.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2jnthuizw.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2jvxcfoxa.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2jensmkxm.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2qzckpsof.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2fvvbdjpd.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2jkhjbqxx.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2mgkqgtat.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2xcozvmbn.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2djqehqvp.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2kdvgzivs.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2mcplvune.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2jksbfkqn.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2drdtgilw.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2eprlugno.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2uehyqexc.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2ogwposar.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2bjzltktp.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2etwkamgf.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2teayyfqg.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2eddxzpdj.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2gqdzhluo.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2dlwstzgk.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2zjxqstfn.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2lidwieps.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2exaphinc.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2dwpyxkgk.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2wrbgkzjm.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2tbpyfxjw.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2qhzagxoi.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2dvtrwzkb.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2ynfjpvua.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2djglzyax.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2czacbulq.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2ggyiympi.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2dcwjyvfi.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2kybdutjc.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2ehpewvfi.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2vsvtulbu.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2xftncain.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2ybdpaowh.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2sejvzsxa.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2csewfxlx.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2nncrgtqo.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2nuwlnacv.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2ottnpbeg.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2iycrddtx.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2grpaaigm.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2xaaixmqu.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2hjnenclm.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2tsypfluv.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2nsggeqfq.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2shbrkwpb.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2dbupqona.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2kphoytyz.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2nooonbce.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2zwgosvau.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2uiflmoiz.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2lqxdknxw.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2facnptnw.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2xdxuersz.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2byytcpgv.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2gnfzonyk.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2vosggces.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2fbhiesiw.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2dzimhptc.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2bkmttzob.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2jsiuvlof.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2zurxyaal.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2zzwuxjcg.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2ecfyrnko.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2rgndlrtf.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2kjcghqjz.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2kopfjhzp.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2zaaiwsqf.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2bgrzwnzv.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2hqvpdeig.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2relunrrt.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2bzimmews.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2iojnonzm.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2usqbxvsi.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2rtzhapck.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2udomcwsm.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2pgjlnejs.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2vgzbknof.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2mpmphjqe.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2ffsvwwoo.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2qbfatlft.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2svnvjdpo.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2imokhkmc.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2vxbijdch.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2ibmlohhz.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2abtakoam.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2iybmrszd.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2cnlxwjof.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2byeucswd.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2ehhrtvbx.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2lpjiasjv.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2rpwvivha.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2rknfipyk.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2jdrggmuz.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2ivxccesp.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2xlbffjnf.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2ocxglasu.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2akuwtnla.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2elpkychx.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2icwdukgg.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2aubmuduw.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2nxbipizc.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2ueooxhrc.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2rcitgsmk.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2jkkzawey.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2lmgzahry.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2xwwlbvfr.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2bsulhodd.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2fegzeugu.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2kdvwxgmq.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2ogkhgpgx.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2tznstnap.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2zslevsnf.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2akftseul.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2xzbzxhip.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2unpugqrn.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2tdrvlldj.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2lcxhqxsd.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2aamvgdjx.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2qzviuzpi.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2xfgutctd.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2jqbeuaij.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2kwhnwxic.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2kgcksytb.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2veofrmgr.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2njkdmfjj.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2fuhwdztv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ihplljpi.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2bvrjvetf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wvlphflf.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2viukagor.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2qbaepuxy.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2oqohdgfi.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2taxriduw.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2bqwuyrym.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2tmsnpvpn.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2scfpypzg.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2rfculgwc.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2fvsbafbj.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2jbchogwm.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2psyqevds.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ncwhwpnf.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xserwctm.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2hlmikxap.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2rhnelhcc.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2atjcgcvj.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2xmisxhaa.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2qpcvbcag.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2pbmzddnf.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2mmlllzby.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2waobxdzc.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2xvrqsxyt.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2scrgqgwq.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2ihmsuifq.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2uqugxkzg.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2joodcbmp.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2xhpemfoe.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2vyznbdqr.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2eambqhgr.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2yzykvhnu.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2upmhucmb.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2pjjdfggl.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2thtfsehj.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2arkgeoml.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2osarsrfk.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2qrlgrcse.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2xseqbdiu.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2itujlsbd.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2vyjrkwxb.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2xublyywf.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2ynasbtvc.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2tpmqlwbx.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2ptpnmszx.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2ijkgjvow.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2qfaiwxvv.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2fxxiehlp.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2iypstfda.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2qweyryhg.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2mccjnlfk.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2fektnthu.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2ormamqam.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2iohpojat.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2flnhgstl.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2rawfizxo.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2yylyzbsi.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2bvmghrxy.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2kcqiuiln.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2zediekgc.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2cepuotjl.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2sospbkwr.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2pyzcqvfv.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2atxnqjdu.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2ppjeusas.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2baihickv.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2sdcqjvuz.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2szvyabox.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2xyksfudg.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2ibdroeyq.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2nvloymaw.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2quvilrfb.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2misbykxu.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2mxegwhpx.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2fucnhoet.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ohvolvuh.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2upwndugc.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2aibqcvdb.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2apevrhjs.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2fuuqwvfm.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2szbeitjy.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2hsjiljrq.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2kekaskdx.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2iokxdqax.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2grerydtu.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2awypxxys.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2idmqkysf.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2kxkchhjr.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2dcyjppvg.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2vgshjdwm.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2xejuwvjw.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2xgoaukmx.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2fdflnvzc.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2wtuqckvt.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2vzidzjia.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2fuqoswgf.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2kgzphgin.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2jpvjfkbk.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2xofldtte.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2dondjjos.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2csqstxid.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2dpetnphc.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2jzkuedbn.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2qvwrikai.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2xhfizayd.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2blyfzpzx.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2rciawcfw.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2nvstijwh.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2vwitmlku.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2uitpojhg.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2cwjxezoc.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2gwfzglvm.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2bkrmorle.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2vfxtbihx.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2jyggamic.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2vgpfknms.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2mdzwrotn.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2wsknmaax.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2qwgidrae.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2uroxndfa.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2aufkzgvp.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2upefgnip.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2gcejhskm.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2upjnluzz.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2wiraasts.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2tdygwoqf.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2shgbrqkm.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2jgvtzwpt.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2cgozbffd.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2zlchnxpm.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2wlrvuetz.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2omhzorvw.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2oeubrjnb.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2hdjwkrsf.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2dkkuwiht.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2aujrtxku.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2jwgselbj.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2trhqvzds.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2cwowyinc.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2txyiugiz.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2mtaasrxv.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2nzesdnfm.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2unxgfrff.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2yaoriqur.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2itseengj.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2maowgijo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hdgzzlwb.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2ifyhhkud.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ewzgrjrr.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2qelzsyki.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2ecfoyeqz.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2cypccduh.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2ioikmtkk.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2gxciziol.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2ljcgrffv.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2olqalqzf.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2lniknpin.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2zemxvwtm.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2mpsdcgfr.html


<!-- 参考信息 -->