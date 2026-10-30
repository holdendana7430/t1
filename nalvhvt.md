代发 wailian999

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://mobile.zdbjq.cn/Article/details/gridfbjbi.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.fehbvm.com/Article/details/ghtphisys.sHtML

[B03] switch / match / case
来源：http://read.share.zdbjq.cn/Article/details/guehsoqer.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.share.zdbjq.cn/Article/details/gjxphccgy.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.blog.zdbjq.cn/Article/details/gtciqtsde.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://blog.zdbjq.cn/Article/details/ghbmmecfe.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.m.share.fehbvm.com/Article/details/gygycrlsb.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://baike.zdbjq.cn/Article/details/gaaxhnncq.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.blog.fehbvm.com/Article/details/gwyqfyjum.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://3g.hesvh.cn/Article/details/gzhbhxqbk.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.blog.fehbvm.com/Article/details/gnutgbnfz.sHtML

[B04] for 计数循环
来源：http://www.blog.zdbjq.cn/Article/details/gcgiwimil.sHtML

Py:   for i in range(10): print(i)
来源：http://www.share.fehbvm.com/Article/details/gbyjbzdpq.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.m.share.hesvh.cn/Article/details/glptnpfnn.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.share.fehbvm.com/Article/details/gffasokqh.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://baike.zdbjq.cn/Article/details/gswiwzyju.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://wap.fehbvm.com/Article/details/gsysufoyl.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.share.hesvh.cn/Article/details/gmqbpjook.sHtML

Ruby: 10.times { |i| puts i }
来源：http://3g.hesvh.cn/Article/details/gabkomxst.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.share.zdbjq.cn/Article/details/gcohxgjes.sHtML

[B05] 遍历数组 / 列表
来源：http://blog.fehbvm.com/Article/details/glrfzsdss.sHtML

Py:   for item in arr: print(item)
来源：http://www.share.zdbjq.cn/Article/details/gshaldozs.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://m.share.zdbjq.cn/Article/details/gesknnupw.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://wap.fehbvm.com/Article/details/gfckpsfty.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.m.share.zdbjq.cn/Article/details/goclbevzk.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://m.share.fehbvm.com/Article/details/gjgusikoq.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://mobile.hesvh.cn/Article/details/gfzwmdeum.sHtML

Ruby: arr.each { |item| puts item }
来源：http://mobile.hesvh.cn/Article/details/ggckjwpvz.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.m.share.hesvh.cn/Article/details/ggesaudmh.sHtML

[B06] 遍历字典 / 对象
来源：http://blog.fehbvm.com/Article/details/gzaskybbo.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://m.share.fehbvm.com/Article/details/grmmuqyao.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://3g.hesvh.cn/Article/details/grbzdvllq.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.share.hesvh.cn/Article/details/gcqjtjtor.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://read.share.fehbvm.com/Article/details/gznccujyh.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://wap.fehbvm.com/Article/details/gjdoddrsl.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://read.share.zdbjq.cn/Article/details/gowdoyexr.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://m.share.hesvh.cn/Article/details/gdutadwoc.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.blog.fehbvm.com/Article/details/gdilbyigu.sHtML

[B07] while 循环
来源：http://mobile.fehbvm.com/Article/details/gicurdcrn.sHtML

Py:   while i < 10: i += 1
来源：http://mobile.fehbvm.com/Article/details/gfadvjopw.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://read.share.hesvh.cn/Article/details/gqrcrflth.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.share.hesvh.cn/Article/details/grksoycwg.sHtML

TS:   while (i < 10) { i++; }
来源：http://m.share.hesvh.cn/Article/details/ghqckvedb.sHtML

Java: while (i < 10) { i++; }
来源：http://m.share.hesvh.cn/Article/details/guwliukgq.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://blog.zdbjq.cn/Article/details/gobbfbzdd.sHtML

Ruby: while i < 10; i += 1; end
来源：http://baike.zdbjq.cn/Article/details/gqbapzrps.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.share.fehbvm.com/Article/details/gzvbirmev.sHtML

[B08] do-while（至少执行一次）
来源：http://wap.hesvh.cn/Article/details/gpjxmnpik.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.share.hesvh.cn/Article/details/gjjrgfpcx.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://3g.hesvh.cn/Article/details/geiugthky.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.blog.hesvh.cn/Article/details/gxndcfzgk.sHtML

TS:   do { i++; } while (i < 10);
来源：http://read.share.hesvh.cn/Article/details/gtcjrpapj.sHtML

Java: do { i++; } while (i < 10);
来源：http://read.share.fehbvm.com/Article/details/gfemfmdhp.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://blog.zdbjq.cn/Article/details/ghpkoarzl.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.blog.hesvh.cn/Article/details/girwiuths.sHtML

C#:   do { i++; } while (i < 10);
来源：http://wap.hesvh.cn/Article/details/ggpaotmiy.sHtML

[B09] break 与 continue
来源：http://3g.fehbvm.com/Article/details/gpcwihjpd.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://baike.hesvh.cn/Article/details/gfmbgcjhf.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://mobile.hesvh.cn/Article/details/gmbpyvjti.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.hesvh.cn/Article/details/gqziscsbh.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.fehbvm.com/Article/details/gfyukswni.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.zdbjq.cn/Article/details/gjebxnrhu.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.share.fehbvm.com/Article/details/glamhdovy.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.blog.zdbjq.cn/Article/details/guvevrwif.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.hesvh.cn/Article/details/gixqxamks.sHtML

[B10] 遍历同时拿索引
来源：http://baike.zdbjq.cn/Article/details/gdlsjfiii.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://mobile.zdbjq.cn/Article/details/gofpebnbr.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://m.share.hesvh.cn/Article/details/geihbmksg.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.share.fehbvm.com/Article/details/gzqyhygmy.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://baike.fehbvm.com/Article/details/gpofzxsdo.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://mobile.zdbjq.cn/Article/details/gaczbtzhk.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://read.share.hesvh.cn/Article/details/gupovqxht.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://wap.zdbjq.cn/Article/details/gxwocxckm.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://baike.fehbvm.com/Article/details/gqgxqvqyd.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.m.share.fehbvm.com/Article/details/ggpwjltna.sHtML

Py:   list(range(0, 10, 2))
来源：http://m.share.zdbjq.cn/Article/details/gkfeqqczi.sHtML

PHP:  range(0, 10, 2);
来源：http://read.share.hesvh.cn/Article/details/gljezkczq.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://3g.zdbjq.cn/Article/details/gzrznndyu.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.fehbvm.com/Article/details/glupexkrq.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://mobile.fehbvm.com/Article/details/gklufpibc.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://m.share.hesvh.cn/Article/details/gjfzcvpeb.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.share.zdbjq.cn/Article/details/glmuhokcv.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://read.share.zdbjq.cn/Article/details/gfqjzcrcd.sHtML

[B12] 跳出多层循环
来源：http://blog.hesvh.cn/Article/details/gvaocqvtw.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://m.share.hesvh.cn/Article/details/gpqkqrqwt.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.m.share.zdbjq.cn/Article/details/giqvsnpbb.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.fehbvm.com/Article/details/gdvzhesjx.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.fehbvm.com/Article/details/gfuoypwha.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.share.fehbvm.com/Article/details/gbfmrruop.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.share.fehbvm.com/Article/details/gmhkdwhmr.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://3g.zdbjq.cn/Article/details/gvaqapaou.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://read.share.hesvh.cn/Article/details/giqrhsxuv.sHtML

[B13] 判断是否为数字
来源：http://read.share.zdbjq.cn/Article/details/giitzmjzt.sHtML

Py:   isinstance(x, (int, float))
来源：http://3g.fehbvm.com/Article/details/gvoucucnm.sHtML

PHP:  is_numeric($x)
来源：http://read.share.zdbjq.cn/Article/details/gdiigrkpx.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://blog.hesvh.cn/Article/details/gzawjdmqz.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.blog.fehbvm.com/Article/details/gvdyhbfiz.sHtML

Java: x instanceof Number
来源：http://www.share.hesvh.cn/Article/details/gsveawgtz.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://read.share.hesvh.cn/Article/details/grotartdo.sHtML

Ruby: x.is_a?(Numeric)
来源：http://m.share.fehbvm.com/Article/details/gwqhlehgi.sHtML

C#:   x is int or double or decimal
来源：http://baike.zdbjq.cn/Article/details/grnfcqzng.sHtML

[B14] 判断值是否在集合内
来源：http://read.share.fehbvm.com/Article/details/gsvizbcbp.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.m.share.hesvh.cn/Article/details/gydhoebsq.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.blog.zdbjq.cn/Article/details/gksjwnuns.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.share.fehbvm.com/Article/details/gowvuwjyy.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://mobile.hesvh.cn/Article/details/gzpjhszvi.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://blog.fehbvm.com/Article/details/gpgzwqfai.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://3g.zdbjq.cn/Article/details/gttkrlnxm.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://blog.zdbjq.cn/Article/details/golqjiyrk.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://baike.hesvh.cn/Article/details/gueelxvuh.sHtML

[B15] 布尔运算与取反
来源：http://baike.zdbjq.cn/Article/details/grmgpfmkf.sHtML

Py:   a and b or not c
来源：http://3g.zdbjq.cn/Article/details/gmlgattxl.sHtML

PHP:  $a && $b || !$c
来源：http://read.share.hesvh.cn/Article/details/gdtffedai.sHtML

JS:   a && b || !c
来源：http://www.blog.zdbjq.cn/Article/details/gdabtblph.sHtML

TS:   a && b || !c
来源：http://www.share.zdbjq.cn/Article/details/guhcicwdt.sHtML

Java: a && b || !c
来源：http://3g.fehbvm.com/Article/details/gebtgcwna.sHtML

Go:   a && b || !c
来源：http://read.share.zdbjq.cn/Article/details/gouzscwvi.sHtML

Ruby: a && b || !c
来源：http://www.share.hesvh.cn/Article/details/gelpqlsip.sHtML

C#:   a && b || !c
来源：http://mobile.fehbvm.com/Article/details/garypjpmo.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://3g.zdbjq.cn/Article/details/goyhnctox.sHtML

Py:   if not data: return
来源：http://wap.zdbjq.cn/Article/details/gppwiuhch.sHtML

PHP:  if (!$data) { return; }
来源：http://wap.hesvh.cn/Article/details/gdhxffvon.sHtML

JS:   if (!data) return;
来源：http://www.m.share.hesvh.cn/Article/details/gtqtwvxjj.sHtML

TS:   if (!data) return;
来源：http://www.m.share.zdbjq.cn/Article/details/gfmgpexyj.sHtML

Java: if (data == null) return;
来源：http://www.share.zdbjq.cn/Article/details/gieawvyot.sHtML

Go:   if data == nil { return }
来源：http://www.blog.fehbvm.com/Article/details/gzapyagyn.sHtML

Ruby: return if data.nil?
来源：http://wap.fehbvm.com/Article/details/gvojxdbyl.sHtML

C#:   if (data == null) return;
来源：http://www.blog.fehbvm.com/Article/details/gcabfgqzw.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gryxvqwit.sHtML

C. 函数与作用域
来源：http://www.share.zdbjq.cn/Article/details/gfqsimxdn.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gixfimyjo.sHtML

[C01] 定义函数
来源：http://3g.zdbjq.cn/Article/details/gwaitjybv.sHtML

Py:   def add(a, b): return a + b
来源：http://www.share.fehbvm.com/Article/details/giijhbxii.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.hesvh.cn/Article/details/gcrksqymy.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.blog.fehbvm.com/Article/details/ggiqghlqv.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.fehbvm.com/Article/details/ggoawncez.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.m.share.fehbvm.com/Article/details/gkhemakiq.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://blog.zdbjq.cn/Article/details/gcgzqsmqw.sHtML

Ruby: def add(a, b); a + b; end
来源：http://m.share.hesvh.cn/Article/details/gknotqtsg.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://3g.zdbjq.cn/Article/details/gcnoxxzuj.sHtML

[C02] 默认参数
来源：http://m.share.hesvh.cn/Article/details/gubqzspdi.sHtML

Py:   def greet(name="World"): return name
来源：http://www.blog.hesvh.cn/Article/details/gqctdqaec.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://baike.fehbvm.com/Article/details/gwqcsisqy.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://3g.zdbjq.cn/Article/details/gsggvnrrf.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://baike.zdbjq.cn/Article/details/gvkzlfpyx.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://read.share.hesvh.cn/Article/details/gbhoyniqi.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://read.share.zdbjq.cn/Article/details/gwkxlklzz.sHtML

Ruby: def greet(name = "World") = name
来源：http://3g.fehbvm.com/Article/details/gswrwqyrf.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://3g.fehbvm.com/Article/details/gexkdpgsz.sHtML

[C03] 可变参数
来源：http://www.share.fehbvm.com/Article/details/ggbmdjdpa.sHtML

Py:   def total(*args): return sum(args)
来源：http://m.share.fehbvm.com/Article/details/gccdpupvv.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://wap.zdbjq.cn/Article/details/geetulqtr.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.zdbjq.cn/Article/details/gshjivzvi.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.hesvh.cn/Article/details/gtiqwovwo.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://m.share.hesvh.cn/Article/details/gdjsyakml.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://mobile.zdbjq.cn/Article/details/gospcyiuo.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://3g.fehbvm.com/Article/details/gnzarjaih.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://mobile.fehbvm.com/Article/details/gxjgbeiiy.sHtML

[C04] 命名参数 / 关键字参数
来源：http://baike.fehbvm.com/Article/details/grbxbutwq.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://m.share.fehbvm.com/Article/details/geflmxtaf.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://wap.zdbjq.cn/Article/details/gkjismjxf.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://baike.hesvh.cn/Article/details/gtlbiwaxg.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://3g.hesvh.cn/Article/details/gbahphkyv.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.m.share.hesvh.cn/Article/details/gajdtuslb.sHtML

Go:   // 无：用配置结构体参数
来源：http://m.share.zdbjq.cn/Article/details/gnblaqpyd.sHtML

Ruby: f(a: 1, b: 2)
来源：http://blog.zdbjq.cn/Article/details/gtlxragzf.sHtML

C#:   f(a: 1, b: 2)
来源：http://baike.zdbjq.cn/Article/details/gtcvgpkhz.sHtML

[C05] 返回多个值
来源：http://baike.hesvh.cn/Article/details/glkrzasxe.sHtML

Py:   return a, b
来源：http://www.m.share.hesvh.cn/Article/details/gytokycnv.sHtML

PHP:  return [$a, $b];
来源：http://www.m.share.fehbvm.com/Article/details/guyqfrnep.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://wap.hesvh.cn/Article/details/gzjzxosts.sHtML

TS:   return { a, b };
来源：http://www.m.share.hesvh.cn/Article/details/givthlstr.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://read.share.zdbjq.cn/Article/details/gkenivdsf.sHtML

Go:   return a, b
来源：http://www.m.share.fehbvm.com/Article/details/grbznptlh.sHtML

Ruby: return a, b
来源：http://blog.zdbjq.cn/Article/details/gizjyecyr.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://baike.fehbvm.com/Article/details/gmklmsdqv.sHtML

[C06] 匿名函数 / lambda
来源：http://read.share.zdbjq.cn/Article/details/goryjyaig.sHtML

Py:   square = lambda x: x * x
来源：http://blog.hesvh.cn/Article/details/gldyfeixt.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.share.zdbjq.cn/Article/details/gijqpvlfz.sHtML

JS:   const square = x => x * x;
来源：http://read.share.zdbjq.cn/Article/details/gjtkpulvd.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://read.share.fehbvm.com/Article/details/gdrkmztgz.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://wap.hesvh.cn/Article/details/ggjvhgodl.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://baike.fehbvm.com/Article/details/gcllmgwwz.sHtML

Ruby: square = ->(x) { x * x }
来源：http://mobile.zdbjq.cn/Article/details/gqiykerbj.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://mobile.fehbvm.com/Article/details/gjjqebhxj.sHtML

[C07] 把函数作为参数传入
来源：http://wap.hesvh.cn/Article/details/gbqtzrbza.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.blog.hesvh.cn/Article/details/gxcfppdjw.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://read.share.hesvh.cn/Article/details/gvgankskc.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://3g.fehbvm.com/Article/details/getjnjhya.sHtML

TS:   arr.map(String)
来源：http://www.share.zdbjq.cn/Article/details/gahjxzhjf.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://baike.zdbjq.cn/Article/details/gptmhyysg.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.blog.zdbjq.cn/Article/details/gekcekkyb.sHtML

Ruby: arr.map(&:upcase)
来源：http://mobile.hesvh.cn/Article/details/gulfmrejn.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://read.share.hesvh.cn/Article/details/gunmrazqh.sHtML

[C08] 闭包
来源：http://www.blog.hesvh.cn/Article/details/gcxrmoakv.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.share.fehbvm.com/Article/details/gqxohnirj.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.m.share.hesvh.cn/Article/details/gaemelsgi.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.m.share.fehbvm.com/Article/details/gfvlmqboj.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.blog.hesvh.cn/Article/details/gfcaorywi.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://3g.zdbjq.cn/Article/details/gkxgtbzgf.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://m.share.fehbvm.com/Article/details/gqxlmxltn.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://read.share.hesvh.cn/Article/details/gsalkqcgw.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mobile.fehbvm.com/Article/details/ggfqwowka.sHtML

[C09] 递归
来源：http://read.share.zdbjq.cn/Article/details/gfywfviwy.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://3g.hesvh.cn/Article/details/ghyjqbfbh.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://m.share.zdbjq.cn/Article/details/gsvdetsuj.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.fehbvm.com/Article/details/gkykodzke.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.hesvh.cn/Article/details/gqbuaomiu.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://m.share.hesvh.cn/Article/details/gmupkoxfk.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://baike.fehbvm.com/Article/details/gthndqezt.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://read.share.fehbvm.com/Article/details/gfrdxmggf.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://read.share.hesvh.cn/Article/details/grmqmciit.sHtML

[C10] 变量作用域
来源：http://www.m.share.fehbvm.com/Article/details/gcaoovqxl.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.m.share.zdbjq.cn/Article/details/gnyccrfba.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://read.share.zdbjq.cn/Article/details/gywjkxngw.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://mobile.hesvh.cn/Article/details/goxrmbvvx.sHtML

TS:   同 JS
来源：http://blog.fehbvm.com/Article/details/gsoyolozz.sHtML

Java: 方法内为块级作用域
来源：http://mobile.hesvh.cn/Article/details/gcksphqsm.sHtML

Go:   花括号块级作用域
来源：http://wap.zdbjq.cn/Article/details/gfzqibsnv.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://read.share.hesvh.cn/Article/details/ggbrpgcip.sHtML

C#:   块级作用域
来源：http://mobile.zdbjq.cn/Article/details/gqsahagkb.sHtML

[C11] 模块导入与导出
来源：http://m.share.fehbvm.com/Article/details/gmypvedde.sHtML

Py:   from module import func
来源：http://www.share.zdbjq.cn/Article/details/gntvlryss.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://m.share.hesvh.cn/Article/details/gprwhgqks.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://read.share.fehbvm.com/Article/details/gmqwuplrx.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://blog.hesvh.cn/Article/details/gmcqdpmxs.sHtML

Java: import java.util.List;
来源：http://wap.hesvh.cn/Article/details/gywmbvkkl.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://3g.hesvh.cn/Article/details/gmrkqxpwm.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.share.hesvh.cn/Article/details/gdryshjmu.sHtML

C#:   using System.Text;
来源：http://read.share.zdbjq.cn/Article/details/glngscvlq.sHtML

[C12] 立即执行函数 IIFE
来源：http://baike.fehbvm.com/Article/details/gxbweyscf.sHtML

Py:   (lambda: print("run"))()
来源：http://mobile.fehbvm.com/Article/details/gztzcpusi.sHtML

PHP:  (function () { echo "run"; })();
来源：http://3g.fehbvm.com/Article/details/gdsexvrua.sHtML

JS:   (() => { console.log("run"); })();
来源：http://wap.fehbvm.com/Article/details/gerenksff.sHtML

TS:   (() => { console.log("run"); })();
来源：http://blog.fehbvm.com/Article/details/goxwtbbnd.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wap.zdbjq.cn/Article/details/gfhbhrizo.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://read.share.zdbjq.cn/Article/details/gmlcfifnj.sHtML

Ruby: -> { puts "run" }.call
来源：http://3g.fehbvm.com/Article/details/guyveplqy.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://baike.fehbvm.com/Article/details/ghjvymglt.sHtML

[C13] 类型声明 / 类型注解
来源：http://mobile.fehbvm.com/Article/details/ggxawwfki.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://baike.fehbvm.com/Article/details/ggqjpfoff.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.zdbjq.cn/Article/details/gdwdmzgwz.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://mobile.hesvh.cn/Article/details/gwnbjycml.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.hesvh.cn/Article/details/gqqpmvbec.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://mobile.fehbvm.com/Article/details/gfnhkfcry.sHtML

Go:   func add(a, b int) int
来源：http://3g.zdbjq.cn/Article/details/gnfqkjfga.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://baike.zdbjq.cn/Article/details/gqdxnrnln.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://read.share.zdbjq.cn/Article/details/gjrftjjpl.sHtML

[C14] 泛型函数
来源：http://m.share.hesvh.cn/Article/details/gleoqrnty.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://mobile.zdbjq.cn/Article/details/gcatrmtyg.sHtML

PHP:  // 无泛型
来源：http://mobile.fehbvm.com/Article/details/giagtaash.sHtML

JS:   // 无泛型
来源：http://read.share.zdbjq.cn/Article/details/gphitqntk.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://baike.zdbjq.cn/Article/details/gqqfkpblf.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wap.zdbjq.cn/Article/details/gozhrtvqj.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.m.share.fehbvm.com/Article/details/gmkbtbqwc.sHtML

Ruby: # 无泛型
来源：http://mobile.fehbvm.com/Article/details/gkonxyfwq.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://m.share.zdbjq.cn/Article/details/gavuqteib.sHtML

[C15] 解构 / 展开参数
来源：http://www.blog.zdbjq.cn/Article/details/gtcycscvp.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://blog.zdbjq.cn/Article/details/gqozktgcz.sHtML

PHP:  [$a, $b] = $pair;
来源：http://3g.hesvh.cn/Article/details/gozvjlyyj.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://3g.zdbjq.cn/Article/details/gxbvmzmol.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://mobile.fehbvm.com/Article/details/gmkaxczkh.sHtML

Java: // 无解构
来源：http://blog.zdbjq.cn/Article/details/gnokumawp.sHtML

Go:   // 无解构
来源：http://mobile.fehbvm.com/Article/details/gyrcwisjb.sHtML

Ruby: a, b = pair
来源：http://blog.zdbjq.cn/Article/details/giwokzjnc.sHtML

C#:   var (a, b) = pair;
来源：http://3g.zdbjq.cn/Article/details/gxurxdrzi.sHtML

[C16] 函数 / 方法重载
来源：http://mobile.hesvh.cn/Article/details/gqgeiyfmr.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://mobile.zdbjq.cn/Article/details/gencmcmla.sHtML

PHP:  // 无重载
来源：http://baike.hesvh.cn/Article/details/gxjhqflrd.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://read.share.zdbjq.cn/Article/details/gwqmjpmew.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.blog.fehbvm.com/Article/details/ghmzvxvcz.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.blog.hesvh.cn/Article/details/gyguitzac.sHtML

Go:   // 无重载：用不同函数名
来源：http://baike.zdbjq.cn/Article/details/gwcmzplcf.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.blog.fehbvm.com/Article/details/gbnkkbsgv.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://3g.hesvh.cn/Article/details/gadvuecfu.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gtynpueba.sHtML

D. 数组 / 列表 / 集合
来源：http://www.m.share.hesvh.cn/Article/details/gfspjshtn.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gwxfyuije.sHtML

[D01] 创建数组 / 列表
来源：http://www.m.share.zdbjq.cn/Article/details/giwcfdzom.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://m.share.fehbvm.com/Article/details/grxdajsed.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.m.share.zdbjq.cn/Article/details/gmiipvsvc.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://m.share.hesvh.cn/Article/details/gbajgdoag.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.blog.hesvh.cn/Article/details/gxrrtppln.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.m.share.hesvh.cn/Article/details/gkampoitq.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.m.share.zdbjq.cn/Article/details/gtjzgnknv.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.blog.fehbvm.com/Article/details/gofrbtidl.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.m.share.zdbjq.cn/Article/details/gshcvcpgx.sHtML

[D02] 追加元素到末尾
来源：http://www.share.hesvh.cn/Article/details/gdjzllsrt.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://read.share.hesvh.cn/Article/details/ggqegqtpp.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.blog.hesvh.cn/Article/details/grjcbmqeu.sHtML

JS:   arr.push(4);
来源：http://mobile.hesvh.cn/Article/details/gsqcwjrun.sHtML

TS:   arr.push(4);
来源：http://3g.zdbjq.cn/Article/details/gcdfwvlhb.sHtML

Java: list.add(4);
来源：http://wap.hesvh.cn/Article/details/gfxzpdmph.sHtML

Go:   arr = append(arr, 4)
来源：http://baike.zdbjq.cn/Article/details/gqfpqjmou.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://blog.zdbjq.cn/Article/details/gydfsvyog.sHtML

C#:   list.Add(4);
来源：http://www.blog.hesvh.cn/Article/details/gjnzwlzzk.sHtML

[D03] 在指定位置插入元素
来源：http://www.m.share.zdbjq.cn/Article/details/gtlfdxtvo.sHtML

Py:   arr.insert(0, 0)
来源：http://baike.zdbjq.cn/Article/details/gufyrafiu.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://blog.fehbvm.com/Article/details/gzawxxmxf.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.share.hesvh.cn/Article/details/gldjoinwn.sHtML


<!-- 参考信息 -->