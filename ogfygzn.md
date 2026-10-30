代发 wailian999

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://blog.hesvh.cn/Article/details/gqdowrhfz.sHtML

[B06] 遍历字典 / 对象
来源：http://blog.zdbjq.cn/Article/details/gkipksxwx.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://baike.zdbjq.cn/Article/details/grmhubytr.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.blog.zdbjq.cn/Article/details/gkuzhfrpw.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://blog.hesvh.cn/Article/details/gtpwkfnym.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.share.zdbjq.cn/Article/details/gwztgxnlz.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://blog.zdbjq.cn/Article/details/gqjraelyu.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://3g.hesvh.cn/Article/details/gcfxekjds.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://blog.zdbjq.cn/Article/details/ggkgzyhja.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://mobile.hesvh.cn/Article/details/gdotmnnwe.sHtML

[B07] while 循环
来源：http://mobile.hesvh.cn/Article/details/gmqrzyevn.sHtML

Py:   while i < 10: i += 1
来源：http://3g.fehbvm.com/Article/details/glkejmsna.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://blog.zdbjq.cn/Article/details/gympugaix.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.share.hesvh.cn/Article/details/godrwijov.sHtML

TS:   while (i < 10) { i++; }
来源：http://baike.zdbjq.cn/Article/details/gteqtjnff.sHtML

Java: while (i < 10) { i++; }
来源：http://www.share.fehbvm.com/Article/details/gtuhflvtg.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://read.share.fehbvm.com/Article/details/gkbwcnhok.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.m.share.hesvh.cn/Article/details/gwdyszqqg.sHtML

C#:   while (i < 10) { i++; }
来源：http://baike.zdbjq.cn/Article/details/glwdhymdu.sHtML

[B08] do-while（至少执行一次）
来源：http://www.share.zdbjq.cn/Article/details/gupldygff.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://blog.zdbjq.cn/Article/details/gszxpshpd.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://mobile.hesvh.cn/Article/details/ghuxxmxni.sHtML

JS:   do { i++; } while (i < 10);
来源：http://wap.hesvh.cn/Article/details/gxceseodx.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.blog.zdbjq.cn/Article/details/gztyfpcwj.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.share.hesvh.cn/Article/details/gknopawwq.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://baike.zdbjq.cn/Article/details/gqfyhanlj.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://mobile.fehbvm.com/Article/details/gbcdtcmro.sHtML

C#:   do { i++; } while (i < 10);
来源：http://baike.fehbvm.com/Article/details/gipjezwll.sHtML

[B09] break 与 continue
来源：http://www.m.share.hesvh.cn/Article/details/gjabcijcv.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.m.share.fehbvm.com/Article/details/gxmantozh.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://m.share.fehbvm.com/Article/details/gvceoohiu.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.hesvh.cn/Article/details/gmqmnwvsx.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.zdbjq.cn/Article/details/gspdzuvws.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.fehbvm.com/Article/details/gwtjmlyrj.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://blog.zdbjq.cn/Article/details/grcxtbdxq.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.share.zdbjq.cn/Article/details/ggtmjxspa.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.hesvh.cn/Article/details/glcjftqqy.sHtML

[B10] 遍历同时拿索引
来源：http://blog.zdbjq.cn/Article/details/gojfchaom.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://mobile.hesvh.cn/Article/details/gmhivwxfy.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://m.share.hesvh.cn/Article/details/gdjcsrjdj.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://m.share.fehbvm.com/Article/details/gtncjkcre.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.blog.hesvh.cn/Article/details/gushwowhp.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://mobile.hesvh.cn/Article/details/gvujmhtlv.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://3g.fehbvm.com/Article/details/gsjhkjuci.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://wap.hesvh.cn/Article/details/ghgyrjxpa.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://blog.zdbjq.cn/Article/details/gjvqirwci.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.m.share.hesvh.cn/Article/details/gkifqjfdu.sHtML

Py:   list(range(0, 10, 2))
来源：http://mobile.zdbjq.cn/Article/details/gqidiedvd.sHtML

PHP:  range(0, 10, 2);
来源：http://www.m.share.fehbvm.com/Article/details/gxbrdspko.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://baike.hesvh.cn/Article/details/gwrmjysqc.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://read.share.hesvh.cn/Article/details/gpsuhmxdu.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://wap.fehbvm.com/Article/details/gezmzwofz.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://mobile.zdbjq.cn/Article/details/gnpsbftld.sHtML

Ruby: (0...10).step(2).to_a
来源：http://wap.fehbvm.com/Article/details/gwzmsfiha.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://mobile.fehbvm.com/Article/details/gdixupyyk.sHtML

[B12] 跳出多层循环
来源：http://blog.hesvh.cn/Article/details/gkiuhbbpz.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.share.fehbvm.com/Article/details/gkueakhav.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://read.share.fehbvm.com/Article/details/gyqcpdxoc.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://read.share.zdbjq.cn/Article/details/gatcjgegc.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.fehbvm.com/Article/details/gztbbszij.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://m.share.zdbjq.cn/Article/details/ghnargqkj.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.m.share.zdbjq.cn/Article/details/geiaomttp.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://m.share.hesvh.cn/Article/details/gqzjtqghn.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://read.share.fehbvm.com/Article/details/gcvbpwvfx.sHtML

[B13] 判断是否为数字
来源：http://m.share.hesvh.cn/Article/details/gjgnxpmow.sHtML

Py:   isinstance(x, (int, float))
来源：http://mobile.zdbjq.cn/Article/details/ggpatxqzw.sHtML

PHP:  is_numeric($x)
来源：http://www.blog.fehbvm.com/Article/details/gyxzaypfl.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.blog.zdbjq.cn/Article/details/gdaxghbcs.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.zdbjq.cn/Article/details/guoqrdkqm.sHtML

Java: x instanceof Number
来源：http://www.share.hesvh.cn/Article/details/gizcmmhly.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://mobile.zdbjq.cn/Article/details/gfqjvwzuk.sHtML

Ruby: x.is_a?(Numeric)
来源：http://read.share.zdbjq.cn/Article/details/gxjzozaon.sHtML

C#:   x is int or double or decimal
来源：http://wap.fehbvm.com/Article/details/gccsagivy.sHtML

[B14] 判断值是否在集合内
来源：http://blog.zdbjq.cn/Article/details/gijrttmch.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://wap.zdbjq.cn/Article/details/gczqvzzuo.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://blog.hesvh.cn/Article/details/gnajeslux.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.blog.hesvh.cn/Article/details/glwmszlgo.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://blog.zdbjq.cn/Article/details/gltvqlbyj.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://mobile.fehbvm.com/Article/details/gkthltcgq.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.m.share.fehbvm.com/Article/details/gnldmecnf.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.share.fehbvm.com/Article/details/gaoejvlks.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.share.zdbjq.cn/Article/details/glctktrgt.sHtML

[B15] 布尔运算与取反
来源：http://read.share.fehbvm.com/Article/details/gohwllxif.sHtML

Py:   a and b or not c
来源：http://3g.hesvh.cn/Article/details/gwngyxdui.sHtML

PHP:  $a && $b || !$c
来源：http://baike.zdbjq.cn/Article/details/ghpbavkfa.sHtML

JS:   a && b || !c
来源：http://www.m.share.hesvh.cn/Article/details/gdnyiizjh.sHtML

TS:   a && b || !c
来源：http://mobile.zdbjq.cn/Article/details/gkruzbxwt.sHtML

Java: a && b || !c
来源：http://baike.zdbjq.cn/Article/details/gnqkzvygo.sHtML

Go:   a && b || !c
来源：http://baike.zdbjq.cn/Article/details/glewzukvy.sHtML

Ruby: a && b || !c
来源：http://www.blog.zdbjq.cn/Article/details/gvykcvklq.sHtML

C#:   a && b || !c
来源：http://www.blog.fehbvm.com/Article/details/gosnljqmq.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.share.hesvh.cn/Article/details/gfmfbowxy.sHtML

Py:   if not data: return
来源：http://baike.fehbvm.com/Article/details/gnfmybzdv.sHtML

PHP:  if (!$data) { return; }
来源：http://m.share.hesvh.cn/Article/details/gknxqqakx.sHtML

JS:   if (!data) return;
来源：http://wap.zdbjq.cn/Article/details/gnanxbdbv.sHtML

TS:   if (!data) return;
来源：http://blog.hesvh.cn/Article/details/gqvlwzudz.sHtML

Java: if (data == null) return;
来源：http://mobile.fehbvm.com/Article/details/gayvxcols.sHtML

Go:   if data == nil { return }
来源：http://blog.fehbvm.com/Article/details/gamutcnda.sHtML

Ruby: return if data.nil?
来源：http://www.m.share.zdbjq.cn/Article/details/gezdtkquo.sHtML

C#:   if (data == null) return;
来源：http://www.blog.zdbjq.cn/Article/details/gwzdrlogg.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gmzxuwnqf.sHtML

C. 函数与作用域
来源：http://www.blog.zdbjq.cn/Article/details/gnaqyqsqf.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gvzwjvypr.sHtML

[C01] 定义函数
来源：http://read.share.zdbjq.cn/Article/details/gbuzqjxhm.sHtML

Py:   def add(a, b): return a + b
来源：http://read.share.hesvh.cn/Article/details/gdzybwvzj.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.fehbvm.com/Article/details/gixyhhldi.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://3g.zdbjq.cn/Article/details/gfrozbrfu.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.zdbjq.cn/Article/details/gfcmxyifz.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.m.share.fehbvm.com/Article/details/gjzlxhqco.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.share.hesvh.cn/Article/details/gedgaponm.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.m.share.zdbjq.cn/Article/details/gvtkukeqn.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://blog.zdbjq.cn/Article/details/gbsiaofmr.sHtML

[C02] 默认参数
来源：http://www.blog.hesvh.cn/Article/details/gkwnfttdu.sHtML

Py:   def greet(name="World"): return name
来源：http://blog.hesvh.cn/Article/details/gmckuxvkj.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://baike.fehbvm.com/Article/details/gyofuwzso.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://baike.fehbvm.com/Article/details/gtmocaooi.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.m.share.fehbvm.com/Article/details/gqilmzrty.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://mobile.zdbjq.cn/Article/details/gechqueob.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wap.hesvh.cn/Article/details/gvgaisjpu.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.m.share.fehbvm.com/Article/details/gnhdwheoc.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.m.share.zdbjq.cn/Article/details/gzxpmlvqg.sHtML

[C03] 可变参数
来源：http://mobile.zdbjq.cn/Article/details/gblehxdmo.sHtML

Py:   def total(*args): return sum(args)
来源：http://read.share.hesvh.cn/Article/details/gdmvaviws.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://baike.fehbvm.com/Article/details/gajwfuyzo.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.zdbjq.cn/Article/details/geeukejqb.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.hesvh.cn/Article/details/gwqyeuguj.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.blog.zdbjq.cn/Article/details/gsnvijnsc.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.share.zdbjq.cn/Article/details/gtwnpehua.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.m.share.fehbvm.com/Article/details/gbnykjvtt.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.m.share.zdbjq.cn/Article/details/gqobbmlsn.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.m.share.zdbjq.cn/Article/details/glwvahjin.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://3g.fehbvm.com/Article/details/gzcmgvlod.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://wap.hesvh.cn/Article/details/gztkmuxvl.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.share.hesvh.cn/Article/details/ghyjkyvzf.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://blog.hesvh.cn/Article/details/glqnrvlkv.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://read.share.hesvh.cn/Article/details/gdrvtdhly.sHtML

Go:   // 无：用配置结构体参数
来源：http://wap.hesvh.cn/Article/details/ghbgihjuk.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gmxnuqdyn.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.share.hesvh.cn/Article/details/gpzhbqnoa.sHtML

[C05] 返回多个值
来源：http://www.m.share.fehbvm.com/Article/details/gtggdygdo.sHtML

Py:   return a, b
来源：http://baike.hesvh.cn/Article/details/gixmuoeai.sHtML

PHP:  return [$a, $b];
来源：http://blog.fehbvm.com/Article/details/ghseyouvr.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://3g.zdbjq.cn/Article/details/gbmhgcfin.sHtML

TS:   return { a, b };
来源：http://3g.hesvh.cn/Article/details/gccfourwo.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.m.share.hesvh.cn/Article/details/gfryykomz.sHtML

Go:   return a, b
来源：http://www.m.share.fehbvm.com/Article/details/gtbaygvge.sHtML

Ruby: return a, b
来源：http://www.m.share.zdbjq.cn/Article/details/gchndksgm.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://mobile.zdbjq.cn/Article/details/gupjijrsi.sHtML

[C06] 匿名函数 / lambda
来源：http://wap.zdbjq.cn/Article/details/gmiwkleaj.sHtML

Py:   square = lambda x: x * x
来源：http://www.share.hesvh.cn/Article/details/gumckotla.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://blog.zdbjq.cn/Article/details/gpjkdjlso.sHtML

JS:   const square = x => x * x;
来源：http://blog.fehbvm.com/Article/details/gxvfciqra.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.m.share.zdbjq.cn/Article/details/gtsbajcqx.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://m.share.fehbvm.com/Article/details/gfpupoktw.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://baike.hesvh.cn/Article/details/gubtgicty.sHtML

Ruby: square = ->(x) { x * x }
来源：http://3g.zdbjq.cn/Article/details/gwzfapacf.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://baike.hesvh.cn/Article/details/gieyhymne.sHtML

[C07] 把函数作为参数传入
来源：http://www.blog.hesvh.cn/Article/details/gurmnlesj.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.blog.fehbvm.com/Article/details/gyhcyllqj.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://blog.hesvh.cn/Article/details/gaofcklgm.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://blog.zdbjq.cn/Article/details/gjanonkzg.sHtML

TS:   arr.map(String)
来源：http://read.share.hesvh.cn/Article/details/gqyneijci.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://3g.zdbjq.cn/Article/details/gccopgldf.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://read.share.fehbvm.com/Article/details/gdcxpmtln.sHtML

Ruby: arr.map(&:upcase)
来源：http://wap.fehbvm.com/Article/details/gsqeebmyc.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://read.share.hesvh.cn/Article/details/gvexgwclw.sHtML

[C08] 闭包
来源：http://wap.zdbjq.cn/Article/details/gpccditgj.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://m.share.zdbjq.cn/Article/details/gcvwmwvib.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://mobile.fehbvm.com/Article/details/gissmqikm.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://3g.fehbvm.com/Article/details/gfojratlk.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.blog.zdbjq.cn/Article/details/gwgjccckw.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://baike.hesvh.cn/Article/details/gswwbaemy.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://baike.fehbvm.com/Article/details/gkbftnfcb.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://3g.zdbjq.cn/Article/details/gllxwfdtx.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mobile.zdbjq.cn/Article/details/gzwhkgzpb.sHtML

[C09] 递归
来源：http://baike.fehbvm.com/Article/details/gtlcfbsaa.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://read.share.zdbjq.cn/Article/details/gtyimdtvo.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://m.share.fehbvm.com/Article/details/gtirjcrym.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.hesvh.cn/Article/details/gnocjpqnl.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.fehbvm.com/Article/details/gjjprapik.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://3g.zdbjq.cn/Article/details/gtxtjsdfy.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://3g.fehbvm.com/Article/details/grbazwmxl.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://blog.zdbjq.cn/Article/details/gmsvkxjxv.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.share.zdbjq.cn/Article/details/gnoyeahzu.sHtML

[C10] 变量作用域
来源：http://mobile.fehbvm.com/Article/details/gjtsydoob.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://mobile.zdbjq.cn/Article/details/groiandil.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://baike.fehbvm.com/Article/details/gtlsmalpq.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://read.share.hesvh.cn/Article/details/gmsaaerkj.sHtML

TS:   同 JS
来源：http://mobile.zdbjq.cn/Article/details/gkmdegqzz.sHtML

Java: 方法内为块级作用域
来源：http://blog.zdbjq.cn/Article/details/gxefeqzvy.sHtML

Go:   花括号块级作用域
来源：http://blog.zdbjq.cn/Article/details/gjjhctktu.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://mobile.fehbvm.com/Article/details/gdzkcjzzp.sHtML

C#:   块级作用域
来源：http://baike.fehbvm.com/Article/details/gnwzswlsz.sHtML

[C11] 模块导入与导出
来源：http://www.share.zdbjq.cn/Article/details/grvvzhsvj.sHtML

Py:   from module import func
来源：http://read.share.fehbvm.com/Article/details/gyxxltvxk.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://blog.zdbjq.cn/Article/details/gqijkysim.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.share.zdbjq.cn/Article/details/gueprxjoz.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.share.hesvh.cn/Article/details/gbmiadksi.sHtML

Java: import java.util.List;
来源：http://baike.fehbvm.com/Article/details/gdgxxtcfu.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://read.share.hesvh.cn/Article/details/gfdbjwece.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://baike.fehbvm.com/Article/details/gzoonsvxw.sHtML

C#:   using System.Text;
来源：http://mobile.hesvh.cn/Article/details/gywedhvvk.sHtML

[C12] 立即执行函数 IIFE
来源：http://wap.zdbjq.cn/Article/details/gbwbborwk.sHtML

Py:   (lambda: print("run"))()
来源：http://blog.zdbjq.cn/Article/details/gvbvknfxf.sHtML

PHP:  (function () { echo "run"; })();
来源：http://read.share.hesvh.cn/Article/details/gisvacjhd.sHtML

JS:   (() => { console.log("run"); })();
来源：http://3g.zdbjq.cn/Article/details/gteoaawqj.sHtML

TS:   (() => { console.log("run"); })();
来源：http://m.share.hesvh.cn/Article/details/gnbpeduys.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wap.zdbjq.cn/Article/details/gjukmareq.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://wap.zdbjq.cn/Article/details/gizvhisgu.sHtML

Ruby: -> { puts "run" }.call
来源：http://read.share.fehbvm.com/Article/details/gfmfrpeyp.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://wap.fehbvm.com/Article/details/getpneyre.sHtML

[C13] 类型声明 / 类型注解
来源：http://3g.fehbvm.com/Article/details/glreoxcmv.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://m.share.fehbvm.com/Article/details/gbekzetzc.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.hesvh.cn/Article/details/gcxoqiaua.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://wap.hesvh.cn/Article/details/goojqhixq.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.hesvh.cn/Article/details/gzneszrcg.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://m.share.zdbjq.cn/Article/details/gxkrxhanc.sHtML

Go:   func add(a, b int) int
来源：http://wap.hesvh.cn/Article/details/grhiyffpd.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://baike.zdbjq.cn/Article/details/giwuffxgi.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://m.share.zdbjq.cn/Article/details/gwjzvikbf.sHtML

[C14] 泛型函数
来源：http://mobile.zdbjq.cn/Article/details/gpqdrtaac.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.blog.hesvh.cn/Article/details/gtziaptep.sHtML

PHP:  // 无泛型
来源：http://www.share.hesvh.cn/Article/details/grzzntyny.sHtML

JS:   // 无泛型
来源：http://www.m.share.zdbjq.cn/Article/details/grkzktevo.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.share.hesvh.cn/Article/details/gcywctpyy.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.blog.fehbvm.com/Article/details/gfjdmdrut.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://baike.fehbvm.com/Article/details/gwxzysxoj.sHtML

Ruby: # 无泛型
来源：http://wap.fehbvm.com/Article/details/gdydpyfbx.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://m.share.hesvh.cn/Article/details/gtkbzwifu.sHtML

[C15] 解构 / 展开参数
来源：http://wap.fehbvm.com/Article/details/gfarmjtsf.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://read.share.zdbjq.cn/Article/details/gwlwnigcl.sHtML

PHP:  [$a, $b] = $pair;
来源：http://3g.hesvh.cn/Article/details/gggnvmfbm.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://3g.zdbjq.cn/Article/details/gbziobkgp.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.share.fehbvm.com/Article/details/gorqzgoyg.sHtML

Java: // 无解构
来源：http://mobile.fehbvm.com/Article/details/gmphsoekp.sHtML

Go:   // 无解构
来源：http://mobile.hesvh.cn/Article/details/gcitzfsny.sHtML

Ruby: a, b = pair
来源：http://read.share.zdbjq.cn/Article/details/gnwvwoafv.sHtML

C#:   var (a, b) = pair;
来源：http://www.blog.zdbjq.cn/Article/details/gvgdavadn.sHtML

[C16] 函数 / 方法重载
来源：http://www.blog.hesvh.cn/Article/details/guwrdsvvl.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://baike.fehbvm.com/Article/details/gglduajen.sHtML

PHP:  // 无重载
来源：http://baike.fehbvm.com/Article/details/gabppxkzw.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.m.share.hesvh.cn/Article/details/gqflkyolv.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://blog.zdbjq.cn/Article/details/grorrgicj.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.share.hesvh.cn/Article/details/gkjtgrudr.sHtML

Go:   // 无重载：用不同函数名
来源：http://baike.fehbvm.com/Article/details/gulofyurh.sHtML

Ruby: # 无重载：靠动态参数
来源：http://read.share.fehbvm.com/Article/details/gxhgpevtu.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://blog.fehbvm.com/Article/details/gaolwcpko.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gomytzjuh.sHtML

D. 数组 / 列表 / 集合
来源：http://www.blog.zdbjq.cn/Article/details/gdmpgmduk.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/ggalntgwt.sHtML

[D01] 创建数组 / 列表
来源：http://read.share.fehbvm.com/Article/details/gbuxhvkrs.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://blog.zdbjq.cn/Article/details/gflieauzz.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://3g.hesvh.cn/Article/details/geldbhidj.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.share.hesvh.cn/Article/details/gdwhaikwc.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://blog.hesvh.cn/Article/details/gqwidumnc.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.m.share.fehbvm.com/Article/details/glumlrquw.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://3g.fehbvm.com/Article/details/gtjvxcdgh.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.share.fehbvm.com/Article/details/gyzlgsulc.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.m.share.zdbjq.cn/Article/details/glebavlfw.sHtML

[D02] 追加元素到末尾
来源：http://wap.fehbvm.com/Article/details/giqiqfuwc.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.share.hesvh.cn/Article/details/gmqqixlcv.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.blog.fehbvm.com/Article/details/gxnderufv.sHtML

JS:   arr.push(4);
来源：http://www.share.zdbjq.cn/Article/details/ghmxgzueb.sHtML

TS:   arr.push(4);
来源：http://mobile.fehbvm.com/Article/details/gqtbesyny.sHtML

Java: list.add(4);
来源：http://mobile.zdbjq.cn/Article/details/gfexewmbh.sHtML

Go:   arr = append(arr, 4)
来源：http://3g.hesvh.cn/Article/details/gofwgxoxt.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://blog.zdbjq.cn/Article/details/grxprprch.sHtML

C#:   list.Add(4);
来源：http://read.share.fehbvm.com/Article/details/gybnncsuc.sHtML

[D03] 在指定位置插入元素
来源：http://m.share.zdbjq.cn/Article/details/gpvwfpfyj.sHtML

Py:   arr.insert(0, 0)
来源：http://blog.hesvh.cn/Article/details/gbewzvfaj.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://wap.fehbvm.com/Article/details/gpofmqbia.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.blog.hesvh.cn/Article/details/gymfbwkix.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.m.share.fehbvm.com/Article/details/gjiqnkion.sHtML

Java: list.add(0, 0);
来源：http://www.blog.zdbjq.cn/Article/details/gmxzbpzsx.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://mobile.zdbjq.cn/Article/details/gxyrzkxpb.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.share.zdbjq.cn/Article/details/gkpajxfpf.sHtML

C#:   list.Insert(0, 0);
来源：http://blog.hesvh.cn/Article/details/gnxmclaja.sHtML

[D04] 删除元素
来源：http://read.share.hesvh.cn/Article/details/ghsmmhmge.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://blog.fehbvm.com/Article/details/gufwtujlv.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mobile.hesvh.cn/Article/details/gayxznmec.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wap.hesvh.cn/Article/details/gtduhfezj.sHtML

TS:   arr.splice(0, 1);
来源：http://3g.hesvh.cn/Article/details/grnbystpg.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.share.fehbvm.com/Article/details/gmicgzvwp.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.blog.zdbjq.cn/Article/details/goqnxyuca.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mobile.zdbjq.cn/Article/details/gnejdcfkg.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://baike.hesvh.cn/Article/details/glumcxfpg.sHtML

[D05] 访问与修改元素
来源：http://m.share.hesvh.cn/Article/details/gebdtgrkt.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.zdbjq.cn/Article/details/gxymatyqe.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://mobile.fehbvm.com/Article/details/gtfhyycbo.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://baike.hesvh.cn/Article/details/gobzpovgr.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.m.share.zdbjq.cn/Article/details/gefyvseuk.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://mobile.hesvh.cn/Article/details/gdshirnja.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://m.share.fehbvm.com/Article/details/gkirlykay.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.fehbvm.com/Article/details/gjhfnesfq.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mobile.hesvh.cn/Article/details/gzhdgzrvw.sHtML

[D06] 数组长度
来源：http://www.blog.zdbjq.cn/Article/details/gjavibvlb.sHtML

Py:   len(arr)
来源：http://www.blog.fehbvm.com/Article/details/gtinvabnw.sHtML

PHP:  count($arr);
来源：http://3g.fehbvm.com/Article/details/gngtzheif.sHtML

JS:   arr.length
来源：http://blog.zdbjq.cn/Article/details/gjgcenuzj.sHtML

TS:   arr.length
来源：http://blog.fehbvm.com/Article/details/gvyclzkzi.sHtML


<!-- 参考信息 -->