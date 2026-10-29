代发 wailian999

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.share.hesvh.cn/Article/details/gulopryir.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.hesvh.cn/Article/details/gvuwigyqd.sHtML

[B03] switch / match / case
来源：http://mobile.fehbvm.com/Article/details/gvplcievz.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://m.share.hesvh.cn/Article/details/gzikztiyi.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.m.share.fehbvm.com/Article/details/gggcsqxwv.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://3g.zdbjq.cn/Article/details/gwlcpducc.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://m.share.hesvh.cn/Article/details/gjrgzupup.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://wap.hesvh.cn/Article/details/gotnpmfrv.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://baike.zdbjq.cn/Article/details/guncyqyrg.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://3g.fehbvm.com/Article/details/ghbervgth.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://read.share.zdbjq.cn/Article/details/grviczreu.sHtML

[B04] for 计数循环
来源：http://3g.hesvh.cn/Article/details/glavdylfa.sHtML

Py:   for i in range(10): print(i)
来源：http://m.share.fehbvm.com/Article/details/gbuxlqven.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://blog.fehbvm.com/Article/details/golvzrekc.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.m.share.hesvh.cn/Article/details/gbhoqoybl.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://3g.fehbvm.com/Article/details/gmklslngl.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://m.share.zdbjq.cn/Article/details/gpkrlmvkh.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://m.share.fehbvm.com/Article/details/gzbrpfyqn.sHtML

Ruby: 10.times { |i| puts i }
来源：http://www.blog.hesvh.cn/Article/details/gkyxoruap.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.blog.zdbjq.cn/Article/details/gtczdjkgx.sHtML

[B05] 遍历数组 / 列表
来源：http://blog.hesvh.cn/Article/details/giihmohfa.sHtML

Py:   for item in arr: print(item)
来源：http://www.share.fehbvm.com/Article/details/gvstjksrp.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://3g.hesvh.cn/Article/details/gopewscmq.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://3g.fehbvm.com/Article/details/gzrwbxwpw.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://wap.fehbvm.com/Article/details/ggjfjwtmw.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.blog.hesvh.cn/Article/details/gvtkuttwo.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.blog.zdbjq.cn/Article/details/gzjhswsau.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.m.share.fehbvm.com/Article/details/gvnqgzekc.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://m.share.zdbjq.cn/Article/details/ggwffexts.sHtML

[B06] 遍历字典 / 对象
来源：http://blog.fehbvm.com/Article/details/gqhjoifgb.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://blog.zdbjq.cn/Article/details/gdygutlnt.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.share.fehbvm.com/Article/details/gipqbzykt.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.m.share.zdbjq.cn/Article/details/ghykrapbn.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://blog.hesvh.cn/Article/details/gkwtgnaqc.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://baike.fehbvm.com/Article/details/gmtywmilh.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://m.share.zdbjq.cn/Article/details/gztchrdeb.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.blog.hesvh.cn/Article/details/gbwsbhorh.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://mobile.hesvh.cn/Article/details/gjmnwrkxg.sHtML

[B07] while 循环
来源：http://wap.hesvh.cn/Article/details/gbemxvfbd.sHtML

Py:   while i < 10: i += 1
来源：http://wap.hesvh.cn/Article/details/gcfafqnxe.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.m.share.hesvh.cn/Article/details/gbjiufkbt.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.share.hesvh.cn/Article/details/gcxfeawwn.sHtML

TS:   while (i < 10) { i++; }
来源：http://3g.zdbjq.cn/Article/details/gygegspzr.sHtML

Java: while (i < 10) { i++; }
来源：http://www.share.zdbjq.cn/Article/details/ghsavviuv.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.blog.fehbvm.com/Article/details/gudjocvxp.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.m.share.fehbvm.com/Article/details/glcmugtsg.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.share.fehbvm.com/Article/details/gkivwsvcn.sHtML

[B08] do-while（至少执行一次）
来源：http://wap.hesvh.cn/Article/details/gdjhbncnb.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://mobile.fehbvm.com/Article/details/gaotwjbnl.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.m.share.hesvh.cn/Article/details/glgfiyzxa.sHtML

JS:   do { i++; } while (i < 10);
来源：http://wap.hesvh.cn/Article/details/gedieqzqe.sHtML

TS:   do { i++; } while (i < 10);
来源：http://read.share.fehbvm.com/Article/details/gempozqjk.sHtML

Java: do { i++; } while (i < 10);
来源：http://3g.zdbjq.cn/Article/details/gnpmfmukx.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://mobile.zdbjq.cn/Article/details/gbltdbfqt.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.share.hesvh.cn/Article/details/geezexbcn.sHtML

C#:   do { i++; } while (i < 10);
来源：http://m.share.hesvh.cn/Article/details/gvalnddhm.sHtML

[B09] break 与 continue
来源：http://www.m.share.fehbvm.com/Article/details/gdgfdhkjh.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://baike.hesvh.cn/Article/details/gkfjyndmq.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.share.fehbvm.com/Article/details/gdknhwrht.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.hesvh.cn/Article/details/gtquhtetn.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.hesvh.cn/Article/details/gioqphoqy.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.zdbjq.cn/Article/details/gsgxhyncf.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://blog.fehbvm.com/Article/details/gbdufbmzp.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://blog.hesvh.cn/Article/details/gsxislgeu.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.zdbjq.cn/Article/details/ggjkzyqre.sHtML

[B10] 遍历同时拿索引
来源：http://www.share.zdbjq.cn/Article/details/gddjhvwiw.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://blog.hesvh.cn/Article/details/gazsmbwwg.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gomrebsna.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.m.share.fehbvm.com/Article/details/grzpfjzky.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.m.share.hesvh.cn/Article/details/gujwtmygr.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://wap.hesvh.cn/Article/details/guoprtfcr.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://3g.fehbvm.com/Article/details/gwddrpoml.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://wap.zdbjq.cn/Article/details/gugbgpths.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://baike.fehbvm.com/Article/details/gkecmdxja.sHtML

[B11] 生成数字序列 / 区间
来源：http://m.share.fehbvm.com/Article/details/ghswddvbb.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.m.share.fehbvm.com/Article/details/gxbvukjjb.sHtML

PHP:  range(0, 10, 2);
来源：http://baike.zdbjq.cn/Article/details/gomzyiekc.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.blog.zdbjq.cn/Article/details/gditgagbe.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://3g.fehbvm.com/Article/details/ggcfjiaat.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://3g.zdbjq.cn/Article/details/grcgsetvb.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://mobile.hesvh.cn/Article/details/ghzxstxxq.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.blog.zdbjq.cn/Article/details/ggapoylyy.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://mobile.hesvh.cn/Article/details/glzyllwgf.sHtML

[B12] 跳出多层循环
来源：http://wap.zdbjq.cn/Article/details/gwmnmjjbj.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://m.share.zdbjq.cn/Article/details/gfhvncsgk.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.blog.zdbjq.cn/Article/details/gbptryxet.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.fehbvm.com/Article/details/gcadwkchn.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://read.share.hesvh.cn/Article/details/gpcnhrdji.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.share.hesvh.cn/Article/details/gvcrtbapw.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://3g.hesvh.cn/Article/details/gpborqaxo.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://read.share.fehbvm.com/Article/details/gmjndudid.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://blog.zdbjq.cn/Article/details/guyoyieer.sHtML

[B13] 判断是否为数字
来源：http://www.m.share.hesvh.cn/Article/details/gjngoeqdz.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.blog.hesvh.cn/Article/details/grmsxvgia.sHtML

PHP:  is_numeric($x)
来源：http://m.share.fehbvm.com/Article/details/gsdkmkadl.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.zdbjq.cn/Article/details/guhvsiddv.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.hesvh.cn/Article/details/gejcpotjr.sHtML

Java: x instanceof Number
来源：http://www.m.share.hesvh.cn/Article/details/glmpuwheb.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://baike.hesvh.cn/Article/details/gzrpndjjl.sHtML

Ruby: x.is_a?(Numeric)
来源：http://3g.fehbvm.com/Article/details/gvoywxiwk.sHtML

C#:   x is int or double or decimal
来源：http://read.share.hesvh.cn/Article/details/gddpajmjx.sHtML

[B14] 判断值是否在集合内
来源：http://www.blog.zdbjq.cn/Article/details/gliilymba.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://m.share.hesvh.cn/Article/details/ghntjkuig.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://mobile.zdbjq.cn/Article/details/gyaptmujv.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://wap.hesvh.cn/Article/details/gpkqzgsrf.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://mobile.zdbjq.cn/Article/details/gaecnkpeg.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.m.share.fehbvm.com/Article/details/gbuskgjhy.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.m.share.zdbjq.cn/Article/details/gnkqoczbv.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://baike.zdbjq.cn/Article/details/gjaxfzkhw.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://read.share.fehbvm.com/Article/details/gvxazcjbn.sHtML

[B15] 布尔运算与取反
来源：http://3g.hesvh.cn/Article/details/gkxtizniy.sHtML

Py:   a and b or not c
来源：http://www.m.share.hesvh.cn/Article/details/gcprpofas.sHtML

PHP:  $a && $b || !$c
来源：http://www.share.fehbvm.com/Article/details/gdfmyyssw.sHtML

JS:   a && b || !c
来源：http://www.blog.fehbvm.com/Article/details/grwoftcaz.sHtML

TS:   a && b || !c
来源：http://baike.zdbjq.cn/Article/details/gepcawgho.sHtML

Java: a && b || !c
来源：http://3g.zdbjq.cn/Article/details/gxxxylvkr.sHtML

Go:   a && b || !c
来源：http://www.share.fehbvm.com/Article/details/giazpwnvr.sHtML

Ruby: a && b || !c
来源：http://wap.hesvh.cn/Article/details/ggjkjruvo.sHtML

C#:   a && b || !c
来源：http://m.share.zdbjq.cn/Article/details/glzvevyig.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.blog.fehbvm.com/Article/details/gvdfddbnp.sHtML

Py:   if not data: return
来源：http://www.m.share.hesvh.cn/Article/details/gjsppewyg.sHtML

PHP:  if (!$data) { return; }
来源：http://www.blog.zdbjq.cn/Article/details/grwvepmbq.sHtML

JS:   if (!data) return;
来源：http://m.share.zdbjq.cn/Article/details/gcpetrgns.sHtML

TS:   if (!data) return;
来源：http://mobile.hesvh.cn/Article/details/gcvjwsknn.sHtML

Java: if (data == null) return;
来源：http://www.blog.zdbjq.cn/Article/details/gpsujowpy.sHtML

Go:   if data == nil { return }
来源：http://3g.zdbjq.cn/Article/details/gpividjha.sHtML

Ruby: return if data.nil?
来源：http://blog.fehbvm.com/Article/details/gqshhxvqi.sHtML

C#:   if (data == null) return;
来源：http://m.share.fehbvm.com/Article/details/gnctqogpm.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/ghfejacxx.sHtML

C. 函数与作用域
来源：http://m.share.fehbvm.com/Article/details/ggtinmqbc.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gnpwdttxn.sHtML

[C01] 定义函数
来源：http://www.m.share.fehbvm.com/Article/details/gznmidffs.sHtML

Py:   def add(a, b): return a + b
来源：http://wap.zdbjq.cn/Article/details/gnruskjnb.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.zdbjq.cn/Article/details/gurwinhea.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://3g.fehbvm.com/Article/details/grxvpvilz.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.hesvh.cn/Article/details/gvrbjzsrb.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://3g.fehbvm.com/Article/details/grkerymcp.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://m.share.zdbjq.cn/Article/details/gqfgvyxai.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.m.share.hesvh.cn/Article/details/gbhwbkkca.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://blog.hesvh.cn/Article/details/gtkuovsuq.sHtML

[C02] 默认参数
来源：http://baike.zdbjq.cn/Article/details/ggfatzvdb.sHtML

Py:   def greet(name="World"): return name
来源：http://blog.fehbvm.com/Article/details/gjarqrjiz.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://blog.zdbjq.cn/Article/details/gxtujulqu.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://blog.fehbvm.com/Article/details/ghifjsrgd.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://baike.hesvh.cn/Article/details/grpaehfjq.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://blog.zdbjq.cn/Article/details/glxehlrdj.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://m.share.hesvh.cn/Article/details/gitdxfsre.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.share.zdbjq.cn/Article/details/gymrlilin.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://3g.fehbvm.com/Article/details/grjtnafbn.sHtML

[C03] 可变参数
来源：http://read.share.zdbjq.cn/Article/details/gzmsoabka.sHtML

Py:   def total(*args): return sum(args)
来源：http://blog.fehbvm.com/Article/details/gtxinbfjm.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://m.share.fehbvm.com/Article/details/gwipwpjbq.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.hesvh.cn/Article/details/goamytqas.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.hesvh.cn/Article/details/gsmisupjr.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://baike.hesvh.cn/Article/details/gueovbwyf.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://blog.fehbvm.com/Article/details/geyvfdgqr.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://blog.hesvh.cn/Article/details/gfamtxzpe.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.share.zdbjq.cn/Article/details/gpbjlylxm.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.m.share.fehbvm.com/Article/details/gorzgwozu.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://mobile.zdbjq.cn/Article/details/glgfzsykc.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://3g.fehbvm.com/Article/details/gmpttnbbg.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://m.share.zdbjq.cn/Article/details/glqllewef.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://3g.hesvh.cn/Article/details/gkzvfjbpb.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://read.share.hesvh.cn/Article/details/grtzjslzg.sHtML

Go:   // 无：用配置结构体参数
来源：http://baike.zdbjq.cn/Article/details/gfbkjiuxf.sHtML

Ruby: f(a: 1, b: 2)
来源：http://3g.zdbjq.cn/Article/details/grladeofu.sHtML

C#:   f(a: 1, b: 2)
来源：http://blog.zdbjq.cn/Article/details/gqxkvkdlr.sHtML

[C05] 返回多个值
来源：http://wap.hesvh.cn/Article/details/gllbamwyd.sHtML

Py:   return a, b
来源：http://www.m.share.fehbvm.com/Article/details/gzhxpjsxa.sHtML

PHP:  return [$a, $b];
来源：http://blog.hesvh.cn/Article/details/gubdsfich.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://baike.fehbvm.com/Article/details/gfnzihmyk.sHtML

TS:   return { a, b };
来源：http://www.blog.fehbvm.com/Article/details/gkmjblqtf.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mobile.zdbjq.cn/Article/details/gfrhxsjaw.sHtML

Go:   return a, b
来源：http://www.m.share.hesvh.cn/Article/details/gkeubfewu.sHtML

Ruby: return a, b
来源：http://read.share.zdbjq.cn/Article/details/ggkfrogvb.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.m.share.hesvh.cn/Article/details/glvcqnksy.sHtML

[C06] 匿名函数 / lambda
来源：http://m.share.hesvh.cn/Article/details/gjhttqypq.sHtML

Py:   square = lambda x: x * x
来源：http://www.share.hesvh.cn/Article/details/gcwxcwypm.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://read.share.zdbjq.cn/Article/details/gupcnpaho.sHtML

JS:   const square = x => x * x;
来源：http://www.share.hesvh.cn/Article/details/groagcqal.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://3g.fehbvm.com/Article/details/glqblsbpa.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://blog.hesvh.cn/Article/details/gbicpytiv.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://3g.zdbjq.cn/Article/details/gyhrioqgm.sHtML

Ruby: square = ->(x) { x * x }
来源：http://mobile.zdbjq.cn/Article/details/gfanapjnp.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://m.share.hesvh.cn/Article/details/ghoevhgde.sHtML

[C07] 把函数作为参数传入
来源：http://baike.hesvh.cn/Article/details/glyyxicjp.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.share.hesvh.cn/Article/details/gdvvnpeui.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://3g.zdbjq.cn/Article/details/gaoweibdv.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.m.share.fehbvm.com/Article/details/gyusiypnb.sHtML

TS:   arr.map(String)
来源：http://www.share.hesvh.cn/Article/details/gczbyhatw.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://3g.zdbjq.cn/Article/details/ghydytphl.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://mobile.fehbvm.com/Article/details/ghkbzgzjq.sHtML

Ruby: arr.map(&:upcase)
来源：http://baike.zdbjq.cn/Article/details/graidcovi.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://read.share.fehbvm.com/Article/details/gqqjcjsaw.sHtML

[C08] 闭包
来源：http://mobile.fehbvm.com/Article/details/gczoikhbu.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://baike.fehbvm.com/Article/details/gyqqsustv.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://3g.fehbvm.com/Article/details/gogqlfhba.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.m.share.fehbvm.com/Article/details/gbtfgnpbd.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://wap.fehbvm.com/Article/details/gvscdkoyz.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://wap.hesvh.cn/Article/details/glesohnwr.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.blog.fehbvm.com/Article/details/gmtxqynwr.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://blog.zdbjq.cn/Article/details/ghbkhoyjr.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://3g.hesvh.cn/Article/details/gfdcmvyus.sHtML

[C09] 递归
来源：http://wap.hesvh.cn/Article/details/gbngwzdgq.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://blog.hesvh.cn/Article/details/gmvyjuamu.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.blog.zdbjq.cn/Article/details/gvewmntds.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.hesvh.cn/Article/details/gfwcgmqoh.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.hesvh.cn/Article/details/gwqjuncub.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.m.share.zdbjq.cn/Article/details/gvcsubzbg.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://baike.zdbjq.cn/Article/details/gzcvavtpr.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.m.share.fehbvm.com/Article/details/gtxzwyanl.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://blog.hesvh.cn/Article/details/geqdgqfxk.sHtML

[C10] 变量作用域
来源：http://3g.fehbvm.com/Article/details/geactoohz.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://m.share.zdbjq.cn/Article/details/gsochqjdz.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://3g.fehbvm.com/Article/details/gwmyswipz.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://3g.fehbvm.com/Article/details/gufdwncpv.sHtML

TS:   同 JS
来源：http://baike.fehbvm.com/Article/details/gwwpfpgdc.sHtML

Java: 方法内为块级作用域
来源：http://mobile.hesvh.cn/Article/details/gdzaebkit.sHtML

Go:   花括号块级作用域
来源：http://m.share.hesvh.cn/Article/details/gktjzgdpi.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://blog.zdbjq.cn/Article/details/gshzdyedl.sHtML

C#:   块级作用域
来源：http://blog.hesvh.cn/Article/details/gmhzxpopr.sHtML

[C11] 模块导入与导出
来源：http://baike.zdbjq.cn/Article/details/gxdqdekex.sHtML

Py:   from module import func
来源：http://www.share.zdbjq.cn/Article/details/gyeaojteo.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://3g.zdbjq.cn/Article/details/gwiijrwow.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://3g.zdbjq.cn/Article/details/gcfngdvwn.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://read.share.hesvh.cn/Article/details/gywtvhzhp.sHtML

Java: import java.util.List;
来源：http://baike.zdbjq.cn/Article/details/goedsvqyd.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://mobile.fehbvm.com/Article/details/gebugvrxb.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://wap.fehbvm.com/Article/details/gcmwcvsgo.sHtML

C#:   using System.Text;
来源：http://m.share.zdbjq.cn/Article/details/guszvxckz.sHtML

[C12] 立即执行函数 IIFE
来源：http://m.share.zdbjq.cn/Article/details/guuzufurh.sHtML

Py:   (lambda: print("run"))()
来源：http://read.share.hesvh.cn/Article/details/goxeayorz.sHtML

PHP:  (function () { echo "run"; })();
来源：http://baike.fehbvm.com/Article/details/gpiulstux.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.m.share.fehbvm.com/Article/details/grizlzwts.sHtML

TS:   (() => { console.log("run"); })();
来源：http://m.share.fehbvm.com/Article/details/gjgbjmvdj.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://mobile.fehbvm.com/Article/details/gscuukcmb.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://3g.fehbvm.com/Article/details/gxpmvskdc.sHtML

Ruby: -> { puts "run" }.call
来源：http://wap.hesvh.cn/Article/details/gnljliknn.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.m.share.hesvh.cn/Article/details/goaypezeh.sHtML

[C13] 类型声明 / 类型注解
来源：http://baike.zdbjq.cn/Article/details/gfbhqmvsp.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.blog.hesvh.cn/Article/details/gwjlodiwq.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.hesvh.cn/Article/details/guffzexsa.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.blog.fehbvm.com/Article/details/gbjvbtgve.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.zdbjq.cn/Article/details/gsvsdjkrc.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://read.share.fehbvm.com/Article/details/gciczwmmr.sHtML

Go:   func add(a, b int) int
来源：http://www.blog.hesvh.cn/Article/details/gtsoeyhal.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.blog.fehbvm.com/Article/details/gspdotewf.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://mobile.fehbvm.com/Article/details/gcakoymxn.sHtML

[C14] 泛型函数
来源：http://blog.hesvh.cn/Article/details/gqwqsraii.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://m.share.hesvh.cn/Article/details/gblzuspxd.sHtML

PHP:  // 无泛型
来源：http://blog.fehbvm.com/Article/details/gfygsvzbd.sHtML

JS:   // 无泛型
来源：http://3g.hesvh.cn/Article/details/gvaudsujr.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.blog.fehbvm.com/Article/details/gnbwhrduq.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://baike.hesvh.cn/Article/details/gprwjgfqq.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.blog.fehbvm.com/Article/details/gbapmbpoc.sHtML

Ruby: # 无泛型
来源：http://mobile.zdbjq.cn/Article/details/gkbdbmtuv.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.blog.zdbjq.cn/Article/details/gzpvynftu.sHtML

[C15] 解构 / 展开参数
来源：http://wap.hesvh.cn/Article/details/gtavbjxkj.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.share.hesvh.cn/Article/details/glsgiqmms.sHtML

PHP:  [$a, $b] = $pair;
来源：http://m.share.fehbvm.com/Article/details/gxmcmxsvg.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://read.share.zdbjq.cn/Article/details/gkngttrua.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://3g.hesvh.cn/Article/details/gznssmxsz.sHtML

Java: // 无解构
来源：http://www.blog.zdbjq.cn/Article/details/gdvvexrjn.sHtML

Go:   // 无解构
来源：http://mobile.hesvh.cn/Article/details/gjmvzubhi.sHtML

Ruby: a, b = pair
来源：http://www.m.share.zdbjq.cn/Article/details/gbodnbkqy.sHtML

C#:   var (a, b) = pair;
来源：http://read.share.fehbvm.com/Article/details/gjrkttuzz.sHtML

[C16] 函数 / 方法重载
来源：http://read.share.hesvh.cn/Article/details/ggdjgntfp.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://mobile.fehbvm.com/Article/details/ggooqqhdf.sHtML

PHP:  // 无重载
来源：http://blog.zdbjq.cn/Article/details/gfoxehyio.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.m.share.zdbjq.cn/Article/details/gterzntcl.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.m.share.fehbvm.com/Article/details/ggwgxtduy.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://blog.zdbjq.cn/Article/details/gzwxighdp.sHtML

Go:   // 无重载：用不同函数名
来源：http://mobile.hesvh.cn/Article/details/geabiejsj.sHtML

Ruby: # 无重载：靠动态参数
来源：http://mobile.hesvh.cn/Article/details/gsruckufe.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.blog.fehbvm.com/Article/details/gmecosjey.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gmvkunooi.sHtML

D. 数组 / 列表 / 集合
来源：http://www.share.hesvh.cn/Article/details/giqwuoerf.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gceykpqku.sHtML

[D01] 创建数组 / 列表
来源：http://www.blog.fehbvm.com/Article/details/gqhkiyflz.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://blog.hesvh.cn/Article/details/ghafjagxb.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://blog.zdbjq.cn/Article/details/guwdrjpsw.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://m.share.hesvh.cn/Article/details/gtjkqmezb.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.share.fehbvm.com/Article/details/geztdtsnk.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://3g.hesvh.cn/Article/details/glulgfmjc.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.share.fehbvm.com/Article/details/gbpsavxqg.sHtML

Ruby: arr = [1, 2, 3]
来源：http://3g.zdbjq.cn/Article/details/gwmutikck.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://mobile.zdbjq.cn/Article/details/glwwykohy.sHtML

[D02] 追加元素到末尾
来源：http://blog.fehbvm.com/Article/details/gupiosuon.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://3g.hesvh.cn/Article/details/gpoedelfn.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.blog.zdbjq.cn/Article/details/gqgszkwsu.sHtML

JS:   arr.push(4);
来源：http://www.blog.zdbjq.cn/Article/details/gxohbltrb.sHtML

TS:   arr.push(4);
来源：http://read.share.hesvh.cn/Article/details/ghitzqwls.sHtML

Java: list.add(4);
来源：http://3g.zdbjq.cn/Article/details/ggkqjhbxy.sHtML

Go:   arr = append(arr, 4)
来源：http://www.blog.hesvh.cn/Article/details/gfyeobftz.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.m.share.fehbvm.com/Article/details/gmyyrptfe.sHtML

C#:   list.Add(4);
来源：http://www.m.share.fehbvm.com/Article/details/gdnsmyazr.sHtML

[D03] 在指定位置插入元素
来源：http://www.m.share.fehbvm.com/Article/details/gzxktaqtj.sHtML

Py:   arr.insert(0, 0)
来源：http://blog.hesvh.cn/Article/details/gkqinqshp.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://m.share.hesvh.cn/Article/details/gkgmqdftn.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wap.hesvh.cn/Article/details/gsowtqwje.sHtML


<!-- 参考信息 -->