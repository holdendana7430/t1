代发 wailian999

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://blog.fanxiaobao.xyz/Article/details/gijeiqwhs.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.fanxiaobao.xyz/Article/details/gjzqfrkoh.sHtML

[B03] switch / match / case
来源：http://wap.fanxiaobao.xyz/Article/details/gaxdlvihr.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://m.share.fanxiaobao.xyz/Article/details/gecbmagqw.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gauzzxxrc.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpifpzqgf.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gutrplosk.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://3g.fanxiaobao.xyz/Article/details/goarlfywd.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdcnwqfip.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://3g.fanxiaobao.xyz/Article/details/gwsiwllki.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://wap.fanxiaobao.xyz/Article/details/gxtbnbpwx.sHtML

[B04] for 计数循环
来源：http://baike.fanxiaobao.xyz/Article/details/gsuvlwtkg.sHtML

Py:   for i in range(10): print(i)
来源：http://read.share.fanxiaobao.xyz/Article/details/gbaxsjwpn.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://3g.fanxiaobao.xyz/Article/details/gcvmjcqmt.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mobile.fanxiaobao.xyz/Article/details/gljctfaxz.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mobile.fanxiaobao.xyz/Article/details/gdlccqbpm.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://mobile.fanxiaobao.xyz/Article/details/gdmmftljs.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://m.share.fanxiaobao.xyz/Article/details/gsbtzifvz.sHtML

Ruby: 10.times { |i| puts i }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzrmbperl.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggnmaaxhl.sHtML

[B05] 遍历数组 / 列表
来源：http://3g.fanxiaobao.xyz/Article/details/gyenxytuz.sHtML

Py:   for item in arr: print(item)
来源：http://3g.fanxiaobao.xyz/Article/details/gjekhjlaf.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glvymeffn.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://3g.fanxiaobao.xyz/Article/details/gzgglgjav.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gcikvcxez.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://3g.fanxiaobao.xyz/Article/details/gvujapovu.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://3g.fanxiaobao.xyz/Article/details/goinlnzkq.sHtML

Ruby: arr.each { |item| puts item }
来源：http://wap.fanxiaobao.xyz/Article/details/gyxbwyxmo.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcejxkjpr.sHtML

[B06] 遍历字典 / 对象
来源：http://read.share.fanxiaobao.xyz/Article/details/gsbessdpp.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggnybyjiq.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://3g.fanxiaobao.xyz/Article/details/gomvsevrc.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://baike.fanxiaobao.xyz/Article/details/gqyqfvidj.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://m.share.fanxiaobao.xyz/Article/details/gxblhsbqj.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://baike.fanxiaobao.xyz/Article/details/guefwgpei.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.share.fanxiaobao.xyz/Article/details/goxjwrcxe.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.share.fanxiaobao.xyz/Article/details/gekmuhgbk.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://baike.fanxiaobao.xyz/Article/details/gmdmfseap.sHtML

[B07] while 循环
来源：http://wap.fanxiaobao.xyz/Article/details/gbpocezkb.sHtML

Py:   while i < 10: i += 1
来源：http://www.share.fanxiaobao.xyz/Article/details/gxzlkagjh.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://wap.fanxiaobao.xyz/Article/details/gurtgghdq.sHtML

JS:   while (i < 10) { i++; }
来源：http://baike.fanxiaobao.xyz/Article/details/gncrvstdg.sHtML

TS:   while (i < 10) { i++; }
来源：http://blog.fanxiaobao.xyz/Article/details/gaptmmefq.sHtML

Java: while (i < 10) { i++; }
来源：http://mobile.fanxiaobao.xyz/Article/details/glgfvaemd.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://m.share.fanxiaobao.xyz/Article/details/gnmoqgwnq.sHtML

Ruby: while i < 10; i += 1; end
来源：http://m.share.fanxiaobao.xyz/Article/details/gmlffiztw.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gycofpbni.sHtML

[B08] do-while（至少执行一次）
来源：http://3g.fanxiaobao.xyz/Article/details/gevewfdxe.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.blog.fanxiaobao.xyz/Article/details/gljxurzov.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.share.fanxiaobao.xyz/Article/details/geoygokrf.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.share.fanxiaobao.xyz/Article/details/gjayvgoku.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtgiodept.sHtML

Java: do { i++; } while (i < 10);
来源：http://m.share.fanxiaobao.xyz/Article/details/gqqyybgfk.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://baike.fanxiaobao.xyz/Article/details/gmwrghtly.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://baike.fanxiaobao.xyz/Article/details/gwkcwhuak.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwqqnajky.sHtML

[B09] break 与 continue
来源：http://mobile.fanxiaobao.xyz/Article/details/gejjrhkgr.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://m.share.fanxiaobao.xyz/Article/details/gxizhtgow.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://3g.fanxiaobao.xyz/Article/details/ghdammyyc.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gjeavgetd.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.fanxiaobao.xyz/Article/details/ghvkqvpfl.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.fanxiaobao.xyz/Article/details/ginsxivrt.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://blog.fanxiaobao.xyz/Article/details/gowgmdedw.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://wap.fanxiaobao.xyz/Article/details/gluapcmda.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.fanxiaobao.xyz/Article/details/gwwpnpphb.sHtML

[B10] 遍历同时拿索引
来源：http://read.share.fanxiaobao.xyz/Article/details/geancctvy.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://wap.fanxiaobao.xyz/Article/details/gvolvaaui.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guijwcpzs.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://baike.fanxiaobao.xyz/Article/details/gwbvyopuo.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbvbaazko.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://wap.fanxiaobao.xyz/Article/details/ghfpevyna.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.share.fanxiaobao.xyz/Article/details/grtynqfge.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://3g.fanxiaobao.xyz/Article/details/gcpgbzrjl.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gymavtjeo.sHtML

[B11] 生成数字序列 / 区间
来源：http://read.share.fanxiaobao.xyz/Article/details/ghzzdnvdv.sHtML

Py:   list(range(0, 10, 2))
来源：http://blog.fanxiaobao.xyz/Article/details/giqnonbps.sHtML

PHP:  range(0, 10, 2);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gymhjbipc.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://blog.fanxiaobao.xyz/Article/details/grjbomskk.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://blog.fanxiaobao.xyz/Article/details/gjrlqkxrj.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://wap.fanxiaobao.xyz/Article/details/gnstlyjxw.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfhrtucmk.sHtML

Ruby: (0...10).step(2).to_a
来源：http://read.share.fanxiaobao.xyz/Article/details/gharpfncf.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfryctxdj.sHtML

[B12] 跳出多层循环
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghsylddym.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://mobile.fanxiaobao.xyz/Article/details/gmnyvgvie.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.share.fanxiaobao.xyz/Article/details/ggnylvbrn.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.fanxiaobao.xyz/Article/details/gerbmvtre.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.fanxiaobao.xyz/Article/details/gkgxdgevi.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://read.share.fanxiaobao.xyz/Article/details/gsfscxxqm.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://baike.fanxiaobao.xyz/Article/details/gvzkgddac.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://m.share.fanxiaobao.xyz/Article/details/gwyplsqsi.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://baike.fanxiaobao.xyz/Article/details/gpadawygq.sHtML

[B13] 判断是否为数字
来源：http://baike.fanxiaobao.xyz/Article/details/gugqwvhqr.sHtML

Py:   isinstance(x, (int, float))
来源：http://3g.fanxiaobao.xyz/Article/details/ggpxwefiz.sHtML

PHP:  is_numeric($x)
来源：http://m.share.fanxiaobao.xyz/Article/details/gvmeypdpd.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.fanxiaobao.xyz/Article/details/gpatgesvn.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.fanxiaobao.xyz/Article/details/gtizftatv.sHtML

Java: x instanceof Number
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxvzqtfdm.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://3g.fanxiaobao.xyz/Article/details/gwpmuoacn.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.share.fanxiaobao.xyz/Article/details/gnmeqmhqp.sHtML

C#:   x is int or double or decimal
来源：http://mobile.fanxiaobao.xyz/Article/details/gkgnlgguf.sHtML

[B14] 判断值是否在集合内
来源：http://baike.fanxiaobao.xyz/Article/details/gmigczykc.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwakkbaqe.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://baike.fanxiaobao.xyz/Article/details/gntipdqpk.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzjwdvtfj.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://baike.fanxiaobao.xyz/Article/details/gkfdsitnu.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://m.share.fanxiaobao.xyz/Article/details/gpqixdzoe.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://read.share.fanxiaobao.xyz/Article/details/grotiojsd.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://mobile.fanxiaobao.xyz/Article/details/gnroxktxc.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://3g.fanxiaobao.xyz/Article/details/grdinhwcp.sHtML

[B15] 布尔运算与取反
来源：http://blog.fanxiaobao.xyz/Article/details/ggjjdcxrg.sHtML

Py:   a and b or not c
来源：http://read.share.fanxiaobao.xyz/Article/details/gfvehynxm.sHtML

PHP:  $a && $b || !$c
来源：http://wap.fanxiaobao.xyz/Article/details/gcxlqdwzu.sHtML

JS:   a && b || !c
来源：http://blog.fanxiaobao.xyz/Article/details/gzmieifab.sHtML

TS:   a && b || !c
来源：http://baike.fanxiaobao.xyz/Article/details/gamywgnmw.sHtML

Java: a && b || !c
来源：http://wap.fanxiaobao.xyz/Article/details/geuayrzjt.sHtML

Go:   a && b || !c
来源：http://wap.fanxiaobao.xyz/Article/details/gkcufforh.sHtML

Ruby: a && b || !c
来源：http://read.share.fanxiaobao.xyz/Article/details/gxfxauatt.sHtML

C#:   a && b || !c
来源：http://3g.fanxiaobao.xyz/Article/details/ganjszquo.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkmhwipng.sHtML

Py:   if not data: return
来源：http://mobile.fanxiaobao.xyz/Article/details/gycppgfsh.sHtML

PHP:  if (!$data) { return; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gjucgwenh.sHtML

JS:   if (!data) return;
来源：http://mobile.fanxiaobao.xyz/Article/details/gkihsmqjo.sHtML

TS:   if (!data) return;
来源：http://baike.fanxiaobao.xyz/Article/details/gesgyrdpd.sHtML

Java: if (data == null) return;
来源：http://www.share.fanxiaobao.xyz/Article/details/giytbyelu.sHtML

Go:   if data == nil { return }
来源：http://3g.fanxiaobao.xyz/Article/details/grgcbivjr.sHtML

Ruby: return if data.nil?
来源：http://wap.fanxiaobao.xyz/Article/details/gvixbivog.sHtML

C#:   if (data == null) return;
来源：http://baike.fanxiaobao.xyz/Article/details/gftmisckj.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjfescvmr.sHtML

C. 函数与作用域
来源：http://read.share.fanxiaobao.xyz/Article/details/gqrovkinc.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gqqkfocmx.sHtML

[C01] 定义函数
来源：http://blog.fanxiaobao.xyz/Article/details/geuccpbyk.sHtML

Py:   def add(a, b): return a + b
来源：http://wap.fanxiaobao.xyz/Article/details/gmotdkvga.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.fanxiaobao.xyz/Article/details/gffwkfjqx.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gaxerrmsv.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.fanxiaobao.xyz/Article/details/gtdvbohhc.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gqzlqxchp.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.share.fanxiaobao.xyz/Article/details/gnwscekyy.sHtML

Ruby: def add(a, b); a + b; end
来源：http://blog.fanxiaobao.xyz/Article/details/gwgquefeg.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://blog.fanxiaobao.xyz/Article/details/guxxrogfj.sHtML

[C02] 默认参数
来源：http://blog.fanxiaobao.xyz/Article/details/gzrgoxxee.sHtML

Py:   def greet(name="World"): return name
来源：http://wap.fanxiaobao.xyz/Article/details/gddvyxerj.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://baike.fanxiaobao.xyz/Article/details/gicfzjune.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gwcbwhdrp.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://3g.fanxiaobao.xyz/Article/details/gsgxhifsm.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnzytnglj.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gtnhghani.sHtML

Ruby: def greet(name = "World") = name
来源：http://wap.fanxiaobao.xyz/Article/details/gmmlgnhoz.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://read.share.fanxiaobao.xyz/Article/details/gorjxfqmw.sHtML

[C03] 可变参数
来源：http://read.share.fanxiaobao.xyz/Article/details/gqtiepwxw.sHtML

Py:   def total(*args): return sum(args)
来源：http://wap.fanxiaobao.xyz/Article/details/gmebltnyx.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.share.fanxiaobao.xyz/Article/details/gtewjsfrs.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxnlvytza.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnevemcqn.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gmmkccnlf.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkeroynhb.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghetjrfap.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://m.share.fanxiaobao.xyz/Article/details/gytpdyuhn.sHtML

[C04] 命名参数 / 关键字参数
来源：http://3g.fanxiaobao.xyz/Article/details/gqacoaudr.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://blog.fanxiaobao.xyz/Article/details/getsfgmls.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://blog.fanxiaobao.xyz/Article/details/gscmxfyop.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://blog.fanxiaobao.xyz/Article/details/gynkudenn.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://blog.fanxiaobao.xyz/Article/details/gwxiuldxw.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://blog.fanxiaobao.xyz/Article/details/ggvpruibv.sHtML

Go:   // 无：用配置结构体参数
来源：http://wap.fanxiaobao.xyz/Article/details/gvpdcgvsa.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.share.fanxiaobao.xyz/Article/details/gxbmhqncp.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfvrjuoqx.sHtML

[C05] 返回多个值
来源：http://blog.fanxiaobao.xyz/Article/details/gffjelwce.sHtML

Py:   return a, b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gavrcvgwy.sHtML

PHP:  return [$a, $b];
来源：http://www.blog.fanxiaobao.xyz/Article/details/gduiravug.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://mobile.fanxiaobao.xyz/Article/details/ghfvrnlki.sHtML

TS:   return { a, b };
来源：http://read.share.fanxiaobao.xyz/Article/details/gbuzmedap.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.share.fanxiaobao.xyz/Article/details/gecpmteao.sHtML

Go:   return a, b
来源：http://mobile.fanxiaobao.xyz/Article/details/gsizfsmav.sHtML

Ruby: return a, b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gywklpmde.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://3g.fanxiaobao.xyz/Article/details/gdsxelxki.sHtML

[C06] 匿名函数 / lambda
来源：http://www.share.fanxiaobao.xyz/Article/details/gombrspph.sHtML

Py:   square = lambda x: x * x
来源：http://read.share.fanxiaobao.xyz/Article/details/grrrxbdio.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://3g.fanxiaobao.xyz/Article/details/gixwhwhqh.sHtML

JS:   const square = x => x * x;
来源：http://www.share.fanxiaobao.xyz/Article/details/gjhbzlwuh.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.share.fanxiaobao.xyz/Article/details/gsspvoiqv.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://3g.fanxiaobao.xyz/Article/details/gayaotdau.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://baike.fanxiaobao.xyz/Article/details/ghxnvmfko.sHtML

Ruby: square = ->(x) { x * x }
来源：http://baike.fanxiaobao.xyz/Article/details/gcmcmrhes.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://m.share.fanxiaobao.xyz/Article/details/gfdwepkye.sHtML

[C07] 把函数作为参数传入
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxsxkfprg.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://m.share.fanxiaobao.xyz/Article/details/gghgmjivp.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://baike.fanxiaobao.xyz/Article/details/gysbfcjjd.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://wap.fanxiaobao.xyz/Article/details/gmwusttxw.sHtML

TS:   arr.map(String)
来源：http://m.share.fanxiaobao.xyz/Article/details/grwtzbfwm.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwkzanhae.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://baike.fanxiaobao.xyz/Article/details/gtaiczrrt.sHtML

Ruby: arr.map(&:upcase)
来源：http://3g.fanxiaobao.xyz/Article/details/gywohelxg.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.share.fanxiaobao.xyz/Article/details/gdjeslvub.sHtML

[C08] 闭包
来源：http://wap.fanxiaobao.xyz/Article/details/gnhnepdfd.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://blog.fanxiaobao.xyz/Article/details/gxmixoduy.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gsjnrenpc.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://wap.fanxiaobao.xyz/Article/details/gjweautlc.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gxkifuhko.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://3g.fanxiaobao.xyz/Article/details/gupcxmrgg.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwnlpjtqa.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.share.fanxiaobao.xyz/Article/details/gxjpzlxrx.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://wap.fanxiaobao.xyz/Article/details/gftpvvxju.sHtML

[C09] 递归
来源：http://wap.fanxiaobao.xyz/Article/details/gzmxxsyfa.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.share.fanxiaobao.xyz/Article/details/gpbaszviv.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwrigxuso.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.fanxiaobao.xyz/Article/details/gafkwkhnb.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.fanxiaobao.xyz/Article/details/guylmyutv.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://mobile.fanxiaobao.xyz/Article/details/gtckjljxu.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://baike.fanxiaobao.xyz/Article/details/gwucwxnij.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mobile.fanxiaobao.xyz/Article/details/gdqddkdke.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://blog.fanxiaobao.xyz/Article/details/gewrbcrsz.sHtML

[C10] 变量作用域
来源：http://www.share.fanxiaobao.xyz/Article/details/grcxbdcow.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://mobile.fanxiaobao.xyz/Article/details/grusndsea.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://3g.fanxiaobao.xyz/Article/details/gguhspewp.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://blog.fanxiaobao.xyz/Article/details/gtnkkqozr.sHtML

TS:   同 JS
来源：http://mobile.fanxiaobao.xyz/Article/details/gqlhpekjg.sHtML

Java: 方法内为块级作用域
来源：http://baike.fanxiaobao.xyz/Article/details/ghhxzzzup.sHtML

Go:   花括号块级作用域
来源：http://blog.fanxiaobao.xyz/Article/details/guvizmezb.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.blog.fanxiaobao.xyz/Article/details/gruwtpwxc.sHtML

C#:   块级作用域
来源：http://wap.fanxiaobao.xyz/Article/details/glcpmhqab.sHtML

[C11] 模块导入与导出
来源：http://www.blog.fanxiaobao.xyz/Article/details/greppkscf.sHtML

Py:   from module import func
来源：http://3g.fanxiaobao.xyz/Article/details/gtuibxoou.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://m.share.fanxiaobao.xyz/Article/details/gpthheiar.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grtlfltsg.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkozxqdxw.sHtML

Java: import java.util.List;
来源：http://www.share.fanxiaobao.xyz/Article/details/gqnjprjvv.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://m.share.fanxiaobao.xyz/Article/details/gspdhuugd.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://read.share.fanxiaobao.xyz/Article/details/gbbnramhc.sHtML

C#:   using System.Text;
来源：http://www.share.fanxiaobao.xyz/Article/details/goahjbuad.sHtML

[C12] 立即执行函数 IIFE
来源：http://m.share.fanxiaobao.xyz/Article/details/geqeycouc.sHtML

Py:   (lambda: print("run"))()
来源：http://mobile.fanxiaobao.xyz/Article/details/gzubuhevy.sHtML

PHP:  (function () { echo "run"; })();
来源：http://m.share.fanxiaobao.xyz/Article/details/glgwxipiw.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glyuzmios.sHtML

TS:   (() => { console.log("run"); })();
来源：http://baike.fanxiaobao.xyz/Article/details/grtzgfkiw.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://read.share.fanxiaobao.xyz/Article/details/gtsibmioj.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtjhocqtn.sHtML

Ruby: -> { puts "run" }.call
来源：http://mobile.fanxiaobao.xyz/Article/details/guegtzyfs.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gosjxrhll.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbmwdpvig.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.share.fanxiaobao.xyz/Article/details/gnotkjymi.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.fanxiaobao.xyz/Article/details/gqtswucfw.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://3g.fanxiaobao.xyz/Article/details/gcqvwjilj.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.fanxiaobao.xyz/Article/details/gpyroajsl.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://baike.fanxiaobao.xyz/Article/details/gtwbhemkg.sHtML

Go:   func add(a, b int) int
来源：http://m.share.fanxiaobao.xyz/Article/details/gaozlgglm.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gckwguxhw.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://wap.fanxiaobao.xyz/Article/details/gwotupsyb.sHtML

[C14] 泛型函数
来源：http://mobile.fanxiaobao.xyz/Article/details/grlmegnpo.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://blog.fanxiaobao.xyz/Article/details/gvujjsjxj.sHtML

PHP:  // 无泛型
来源：http://3g.fanxiaobao.xyz/Article/details/gjndyclrn.sHtML

JS:   // 无泛型
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzkkivztj.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://blog.fanxiaobao.xyz/Article/details/goegjhmga.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wap.fanxiaobao.xyz/Article/details/gmvlnwtiz.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://3g.fanxiaobao.xyz/Article/details/gsttggwtr.sHtML

Ruby: # 无泛型
来源：http://www.share.fanxiaobao.xyz/Article/details/gabkwzndz.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.blog.fanxiaobao.xyz/Article/details/gixpgwrys.sHtML

[C15] 解构 / 展开参数
来源：http://www.share.fanxiaobao.xyz/Article/details/ggajbjuvd.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjgkntajl.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gperdepwb.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzucgvzjg.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://blog.fanxiaobao.xyz/Article/details/gbzmbuoea.sHtML

Java: // 无解构
来源：http://m.share.fanxiaobao.xyz/Article/details/glsxxlhud.sHtML

Go:   // 无解构
来源：http://read.share.fanxiaobao.xyz/Article/details/gnfleterp.sHtML

Ruby: a, b = pair
来源：http://m.share.fanxiaobao.xyz/Article/details/ghzxowefm.sHtML

C#:   var (a, b) = pair;
来源：http://wap.fanxiaobao.xyz/Article/details/gvkscdynf.sHtML

[C16] 函数 / 方法重载
来源：http://mobile.fanxiaobao.xyz/Article/details/gqkkeossn.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://mobile.fanxiaobao.xyz/Article/details/gwtumajfl.sHtML

PHP:  // 无重载
来源：http://www.share.fanxiaobao.xyz/Article/details/gcxvemxla.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://read.share.fanxiaobao.xyz/Article/details/gtqcrufgb.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://baike.fanxiaobao.xyz/Article/details/gzzvrfezr.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gacspgzqd.sHtML

Go:   // 无重载：用不同函数名
来源：http://baike.fanxiaobao.xyz/Article/details/gyjjlhwpn.sHtML

Ruby: # 无重载：靠动态参数
来源：http://read.share.fanxiaobao.xyz/Article/details/gqwkxynuy.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://3g.fanxiaobao.xyz/Article/details/gpfmwwwgp.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/ginqkmmub.sHtML

D. 数组 / 列表 / 集合
来源：http://blog.fanxiaobao.xyz/Article/details/gcxxziidl.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gmlnngvlw.sHtML

[D01] 创建数组 / 列表
来源：http://wap.fanxiaobao.xyz/Article/details/getjmzgua.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.share.fanxiaobao.xyz/Article/details/gafyxonwu.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://read.share.fanxiaobao.xyz/Article/details/gpjwahytk.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://m.share.fanxiaobao.xyz/Article/details/gznxydflg.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://3g.fanxiaobao.xyz/Article/details/gujvdjjdh.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wap.fanxiaobao.xyz/Article/details/glbxzysua.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://read.share.fanxiaobao.xyz/Article/details/gualrghor.sHtML

Ruby: arr = [1, 2, 3]
来源：http://3g.fanxiaobao.xyz/Article/details/gndgypqdf.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gujarvfal.sHtML

[D02] 追加元素到末尾
来源：http://blog.fanxiaobao.xyz/Article/details/gskmszqpj.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://baike.fanxiaobao.xyz/Article/details/gwvthpdub.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://m.share.fanxiaobao.xyz/Article/details/gumsoqceh.sHtML

JS:   arr.push(4);
来源：http://mobile.fanxiaobao.xyz/Article/details/gextaejsz.sHtML

TS:   arr.push(4);
来源：http://baike.fanxiaobao.xyz/Article/details/gnfhvaxhv.sHtML

Java: list.add(4);
来源：http://3g.fanxiaobao.xyz/Article/details/gyvzigvev.sHtML

Go:   arr = append(arr, 4)
来源：http://read.share.fanxiaobao.xyz/Article/details/gemwhvwfb.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://3g.fanxiaobao.xyz/Article/details/gfqhocnqe.sHtML

C#:   list.Add(4);
来源：http://3g.fanxiaobao.xyz/Article/details/gjxksrbak.sHtML

[D03] 在指定位置插入元素
来源：http://3g.fanxiaobao.xyz/Article/details/gdabnzbxt.sHtML

Py:   arr.insert(0, 0)
来源：http://blog.fanxiaobao.xyz/Article/details/gihetzmpg.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guziailrf.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://3g.fanxiaobao.xyz/Article/details/gdnyeoerv.sHtML


<!-- 参考信息 -->