代发 wailian999

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://blog.fehbvm.com/Article/details/gizacpmdd.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.share.zdbjq.cn/Article/details/gpkkbzpnu.sHtML

Ruby: 10.times { |i| puts i }
来源：http://www.blog.zdbjq.cn/Article/details/ghmklafdb.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.blog.hesvh.cn/Article/details/gtergcyvc.sHtML

[B05] 遍历数组 / 列表
来源：http://www.share.hesvh.cn/Article/details/gtefudarz.sHtML

Py:   for item in arr: print(item)
来源：http://blog.fehbvm.com/Article/details/gyxbhsarv.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://m.share.zdbjq.cn/Article/details/gxyzutome.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://wap.hesvh.cn/Article/details/gbmohpvsb.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://read.share.hesvh.cn/Article/details/gnjsywveq.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://mobile.zdbjq.cn/Article/details/gpbsplkjy.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.m.share.zdbjq.cn/Article/details/ghygsgdfv.sHtML

Ruby: arr.each { |item| puts item }
来源：http://blog.fehbvm.com/Article/details/gjwdemkgz.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://m.share.fehbvm.com/Article/details/guqfxucil.sHtML

[B06] 遍历字典 / 对象
来源：http://mobile.fehbvm.com/Article/details/ggbcaxvpf.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://m.share.zdbjq.cn/Article/details/goqkwhhcy.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.blog.hesvh.cn/Article/details/gkruishmz.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://m.share.hesvh.cn/Article/details/gyyhvgnkw.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://baike.zdbjq.cn/Article/details/gjahefvfe.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://mobile.zdbjq.cn/Article/details/ghgpcicik.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://wap.zdbjq.cn/Article/details/gcctagbca.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://mobile.fehbvm.com/Article/details/grdwgbpfp.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://mobile.hesvh.cn/Article/details/gwcryskup.sHtML

[B07] while 循环
来源：http://m.share.hesvh.cn/Article/details/gmkawgzlh.sHtML

Py:   while i < 10: i += 1
来源：http://blog.hesvh.cn/Article/details/gtwibkpng.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://blog.zdbjq.cn/Article/details/gcmcxcpdn.sHtML

JS:   while (i < 10) { i++; }
来源：http://wap.fehbvm.com/Article/details/gebbzdigq.sHtML

TS:   while (i < 10) { i++; }
来源：http://blog.hesvh.cn/Article/details/geepryerd.sHtML

Java: while (i < 10) { i++; }
来源：http://www.blog.zdbjq.cn/Article/details/ggrsfubda.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://blog.fehbvm.com/Article/details/gsemqlweu.sHtML

Ruby: while i < 10; i += 1; end
来源：http://blog.hesvh.cn/Article/details/gppxkwcrq.sHtML

C#:   while (i < 10) { i++; }
来源：http://3g.hesvh.cn/Article/details/gdjhvurej.sHtML

[B08] do-while（至少执行一次）
来源：http://wap.fehbvm.com/Article/details/gdyquvimu.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.share.zdbjq.cn/Article/details/gsnjxatff.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://read.share.fehbvm.com/Article/details/gvvrgsjfj.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.share.zdbjq.cn/Article/details/gkwmcbsfz.sHtML

TS:   do { i++; } while (i < 10);
来源：http://3g.zdbjq.cn/Article/details/gbecpenmg.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.m.share.zdbjq.cn/Article/details/gsougbyxw.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://3g.fehbvm.com/Article/details/ghzmdpnuy.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.blog.fehbvm.com/Article/details/gepzafrqp.sHtML

C#:   do { i++; } while (i < 10);
来源：http://m.share.fehbvm.com/Article/details/gvnyegrsk.sHtML

[B09] break 与 continue
来源：http://m.share.fehbvm.com/Article/details/geddrbgij.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://blog.fehbvm.com/Article/details/ggmcirbdd.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://baike.fehbvm.com/Article/details/gnuyvalxl.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.hesvh.cn/Article/details/godghabed.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.fehbvm.com/Article/details/gpmkjpvsh.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.fehbvm.com/Article/details/gfyetkekx.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://read.share.zdbjq.cn/Article/details/gpgqgpril.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://wap.hesvh.cn/Article/details/gmczaxbia.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.zdbjq.cn/Article/details/gnvdzkiif.sHtML

[B10] 遍历同时拿索引
来源：http://www.blog.fehbvm.com/Article/details/ghmtfbsbu.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://wap.fehbvm.com/Article/details/gfacehtdc.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.blog.fehbvm.com/Article/details/gelkmenqs.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://3g.fehbvm.com/Article/details/gpnpiwqfh.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://m.share.hesvh.cn/Article/details/gintswpmn.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.blog.fehbvm.com/Article/details/gzcutdrys.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://blog.fehbvm.com/Article/details/gpbwjxjfm.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://wap.zdbjq.cn/Article/details/glgsjspot.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://wap.hesvh.cn/Article/details/ggrztrjer.sHtML

[B11] 生成数字序列 / 区间
来源：http://baike.zdbjq.cn/Article/details/goordzbpn.sHtML

Py:   list(range(0, 10, 2))
来源：http://3g.hesvh.cn/Article/details/gybwsjgvs.sHtML

PHP:  range(0, 10, 2);
来源：http://baike.zdbjq.cn/Article/details/glwwhtnrj.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mobile.zdbjq.cn/Article/details/gyxkgwaob.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.zdbjq.cn/Article/details/gkyzkdxdz.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://baike.zdbjq.cn/Article/details/gudlvyjps.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.share.fehbvm.com/Article/details/glezpqyop.sHtML

Ruby: (0...10).step(2).to_a
来源：http://wap.zdbjq.cn/Article/details/gnxevzsar.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://read.share.zdbjq.cn/Article/details/geibjogmu.sHtML

[B12] 跳出多层循环
来源：http://baike.fehbvm.com/Article/details/ggwimbfgz.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.blog.zdbjq.cn/Article/details/gycsxtbbl.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://wap.fehbvm.com/Article/details/geqdftojz.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.fehbvm.com/Article/details/gtxhtqres.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.hesvh.cn/Article/details/gksyellxe.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.share.hesvh.cn/Article/details/gdevzxalk.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.share.fehbvm.com/Article/details/gqjlukyrl.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://baike.zdbjq.cn/Article/details/gxxkdejpn.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://baike.hesvh.cn/Article/details/gmmbopeck.sHtML

[B13] 判断是否为数字
来源：http://baike.hesvh.cn/Article/details/gxzigmbta.sHtML

Py:   isinstance(x, (int, float))
来源：http://baike.zdbjq.cn/Article/details/gtpinxilu.sHtML

PHP:  is_numeric($x)
来源：http://www.m.share.hesvh.cn/Article/details/gwrqlbueu.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.hesvh.cn/Article/details/gqwvkgenk.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.zdbjq.cn/Article/details/geetxwgrb.sHtML

Java: x instanceof Number
来源：http://baike.zdbjq.cn/Article/details/gipnbjxje.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://mobile.fehbvm.com/Article/details/gdloinjqq.sHtML

Ruby: x.is_a?(Numeric)
来源：http://mobile.hesvh.cn/Article/details/gywwicqra.sHtML

C#:   x is int or double or decimal
来源：http://baike.hesvh.cn/Article/details/givqiuyfn.sHtML

[B14] 判断值是否在集合内
来源：http://www.blog.fehbvm.com/Article/details/gtsfvhpol.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://wap.fehbvm.com/Article/details/glwwowdhg.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://baike.zdbjq.cn/Article/details/gmcjxuawz.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.share.hesvh.cn/Article/details/gieifudcw.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.share.hesvh.cn/Article/details/grltkxlmn.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://3g.hesvh.cn/Article/details/gdjjsiykc.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.blog.fehbvm.com/Article/details/gwzghicgb.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://m.share.hesvh.cn/Article/details/gxdomutul.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.blog.hesvh.cn/Article/details/gdqabugwl.sHtML

[B15] 布尔运算与取反
来源：http://www.share.zdbjq.cn/Article/details/gdkhlaxwe.sHtML

Py:   a and b or not c
来源：http://3g.fehbvm.com/Article/details/gbvljextd.sHtML

PHP:  $a && $b || !$c
来源：http://www.m.share.hesvh.cn/Article/details/gqzzaminx.sHtML

JS:   a && b || !c
来源：http://www.m.share.fehbvm.com/Article/details/gcasyfltn.sHtML

TS:   a && b || !c
来源：http://mobile.fehbvm.com/Article/details/gwdanbwha.sHtML

Java: a && b || !c
来源：http://wap.zdbjq.cn/Article/details/guliunykr.sHtML

Go:   a && b || !c
来源：http://mobile.fehbvm.com/Article/details/gmyhffedc.sHtML

Ruby: a && b || !c
来源：http://read.share.fehbvm.com/Article/details/ganbdarks.sHtML

C#:   a && b || !c
来源：http://www.m.share.zdbjq.cn/Article/details/gvslaaamt.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://3g.zdbjq.cn/Article/details/gcarxfpkb.sHtML

Py:   if not data: return
来源：http://wap.hesvh.cn/Article/details/gwcbmvajh.sHtML

PHP:  if (!$data) { return; }
来源：http://mobile.fehbvm.com/Article/details/gwrltxupo.sHtML

JS:   if (!data) return;
来源：http://www.share.hesvh.cn/Article/details/gdycopjba.sHtML

TS:   if (!data) return;
来源：http://m.share.zdbjq.cn/Article/details/gwxjilflo.sHtML

Java: if (data == null) return;
来源：http://wap.fehbvm.com/Article/details/gzleeeihb.sHtML

Go:   if data == nil { return }
来源：http://www.blog.hesvh.cn/Article/details/gwlcrklty.sHtML

Ruby: return if data.nil?
来源：http://3g.fehbvm.com/Article/details/ghlijjhwx.sHtML

C#:   if (data == null) return;
来源：http://www.blog.hesvh.cn/Article/details/gfyvbiard.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/galneqxmw.sHtML

C. 函数与作用域
来源：http://wap.fehbvm.com/Article/details/gcvaucpgn.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/giimxemxc.sHtML

[C01] 定义函数
来源：http://www.blog.hesvh.cn/Article/details/gswycbupr.sHtML

Py:   def add(a, b): return a + b
来源：http://www.m.share.hesvh.cn/Article/details/gvyccpske.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.zdbjq.cn/Article/details/gnqzkcnks.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://read.share.hesvh.cn/Article/details/gzmcoqgcw.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.hesvh.cn/Article/details/gvwkoxzsv.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.m.share.fehbvm.com/Article/details/gpnzvsthn.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.blog.zdbjq.cn/Article/details/gxemfrqmj.sHtML

Ruby: def add(a, b); a + b; end
来源：http://baike.hesvh.cn/Article/details/gtnmkonuw.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://3g.zdbjq.cn/Article/details/gamhwqlvt.sHtML

[C02] 默认参数
来源：http://3g.zdbjq.cn/Article/details/gdtxjamby.sHtML

Py:   def greet(name="World"): return name
来源：http://m.share.fehbvm.com/Article/details/giexvjsjx.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.blog.zdbjq.cn/Article/details/gqnkcstra.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://3g.hesvh.cn/Article/details/gotwgxmna.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://read.share.fehbvm.com/Article/details/gwilijjdh.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://mobile.fehbvm.com/Article/details/gfkeudgfj.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://3g.zdbjq.cn/Article/details/gnkjfyuvg.sHtML

Ruby: def greet(name = "World") = name
来源：http://baike.hesvh.cn/Article/details/gfrerbblk.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://mobile.zdbjq.cn/Article/details/gpheksuts.sHtML

[C03] 可变参数
来源：http://wap.zdbjq.cn/Article/details/gwbdzhoij.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.m.share.zdbjq.cn/Article/details/gdaxdjfdv.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://mobile.zdbjq.cn/Article/details/gwjqsymyq.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.hesvh.cn/Article/details/graonrskv.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.hesvh.cn/Article/details/gjjozftsk.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.share.zdbjq.cn/Article/details/gxcjzduvv.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://3g.fehbvm.com/Article/details/gwwxzlqpm.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.m.share.hesvh.cn/Article/details/gtjxgnzur.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://3g.fehbvm.com/Article/details/gpijxbbuv.sHtML

[C04] 命名参数 / 关键字参数
来源：http://mobile.zdbjq.cn/Article/details/gxupeniug.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://blog.hesvh.cn/Article/details/glfvyaogw.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://m.share.zdbjq.cn/Article/details/gvdvlhhuq.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gafpbksiy.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wap.hesvh.cn/Article/details/ghkomhgso.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.share.fehbvm.com/Article/details/gakenpqng.sHtML

Go:   // 无：用配置结构体参数
来源：http://wap.hesvh.cn/Article/details/guexyypsq.sHtML

Ruby: f(a: 1, b: 2)
来源：http://mobile.fehbvm.com/Article/details/grjrednhu.sHtML

C#:   f(a: 1, b: 2)
来源：http://m.share.fehbvm.com/Article/details/gylrojkul.sHtML

[C05] 返回多个值
来源：http://www.share.fehbvm.com/Article/details/gmajjckod.sHtML

Py:   return a, b
来源：http://mobile.fehbvm.com/Article/details/gxngxeqpw.sHtML

PHP:  return [$a, $b];
来源：http://3g.zdbjq.cn/Article/details/ghxraolqj.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://read.share.fehbvm.com/Article/details/gkfwfodhl.sHtML

TS:   return { a, b };
来源：http://blog.hesvh.cn/Article/details/govjybvgk.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.blog.zdbjq.cn/Article/details/gvybxdsgn.sHtML

Go:   return a, b
来源：http://mobile.fehbvm.com/Article/details/gdnlzzhuu.sHtML

Ruby: return a, b
来源：http://www.m.share.fehbvm.com/Article/details/gkieeyoxv.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://m.share.zdbjq.cn/Article/details/gvgbrybad.sHtML

[C06] 匿名函数 / lambda
来源：http://baike.zdbjq.cn/Article/details/gezbpxeqz.sHtML

Py:   square = lambda x: x * x
来源：http://read.share.hesvh.cn/Article/details/gujpqujbc.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://wap.hesvh.cn/Article/details/gmuublzos.sHtML

JS:   const square = x => x * x;
来源：http://blog.fehbvm.com/Article/details/gkziccurs.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://m.share.hesvh.cn/Article/details/gctwblpvi.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://blog.hesvh.cn/Article/details/gksfuodnr.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://mobile.hesvh.cn/Article/details/ggfzynlik.sHtML

Ruby: square = ->(x) { x * x }
来源：http://3g.fehbvm.com/Article/details/grhgxfvdd.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.share.hesvh.cn/Article/details/gzvygzmfc.sHtML

[C07] 把函数作为参数传入
来源：http://wap.fehbvm.com/Article/details/gslikbkbb.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.share.zdbjq.cn/Article/details/geruloatw.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://3g.hesvh.cn/Article/details/gwclkmyuh.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://baike.fehbvm.com/Article/details/gwkuqwdyj.sHtML

TS:   arr.map(String)
来源：http://3g.hesvh.cn/Article/details/guycgmftj.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://baike.hesvh.cn/Article/details/gmqpgkhlh.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://wap.hesvh.cn/Article/details/gfueypmsf.sHtML

Ruby: arr.map(&:upcase)
来源：http://m.share.zdbjq.cn/Article/details/gfzutpuxv.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.m.share.hesvh.cn/Article/details/gkovkvpfs.sHtML

[C08] 闭包
来源：http://blog.hesvh.cn/Article/details/gpslkeafx.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.blog.hesvh.cn/Article/details/gkkgcnddd.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://baike.fehbvm.com/Article/details/gdgyvxupr.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.m.share.hesvh.cn/Article/details/gjdrmqiay.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://blog.hesvh.cn/Article/details/gsbieqbzb.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://m.share.zdbjq.cn/Article/details/gchnbdfur.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.share.hesvh.cn/Article/details/ghkjywbpc.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.share.fehbvm.com/Article/details/gcacmywvq.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://read.share.hesvh.cn/Article/details/gzvwhxnzg.sHtML

[C09] 递归
来源：http://3g.zdbjq.cn/Article/details/gwzmmxehu.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://wap.hesvh.cn/Article/details/gcdsdbwve.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://mobile.fehbvm.com/Article/details/gutzlcazg.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.hesvh.cn/Article/details/gkskcqdym.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.fehbvm.com/Article/details/gnaivyxpr.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://3g.hesvh.cn/Article/details/gtegxwibj.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wap.zdbjq.cn/Article/details/gdqdldegn.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.m.share.fehbvm.com/Article/details/gkvnzufpj.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.blog.fehbvm.com/Article/details/gcptgjejv.sHtML

[C10] 变量作用域
来源：http://m.share.fehbvm.com/Article/details/ggceleugi.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.blog.hesvh.cn/Article/details/gxtievqyi.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.share.fehbvm.com/Article/details/gpkaubeln.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://3g.fehbvm.com/Article/details/gnnhsqlyp.sHtML

TS:   同 JS
来源：http://mobile.zdbjq.cn/Article/details/gyatrlaui.sHtML

Java: 方法内为块级作用域
来源：http://www.blog.zdbjq.cn/Article/details/gkgjoyplp.sHtML

Go:   花括号块级作用域
来源：http://www.share.zdbjq.cn/Article/details/gxwqawkod.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://3g.zdbjq.cn/Article/details/gczzkcqcb.sHtML

C#:   块级作用域
来源：http://baike.zdbjq.cn/Article/details/gtydezwcw.sHtML

[C11] 模块导入与导出
来源：http://www.m.share.zdbjq.cn/Article/details/gedldfbpr.sHtML

Py:   from module import func
来源：http://www.share.hesvh.cn/Article/details/gkvoksjnp.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.blog.fehbvm.com/Article/details/guyfmvptm.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.m.share.zdbjq.cn/Article/details/gpyycohkq.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.m.share.hesvh.cn/Article/details/gtusluarg.sHtML

Java: import java.util.List;
来源：http://www.blog.fehbvm.com/Article/details/gzhnbysju.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://read.share.fehbvm.com/Article/details/gifjuuolm.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://wap.fehbvm.com/Article/details/gfcdhbryp.sHtML

C#:   using System.Text;
来源：http://www.blog.hesvh.cn/Article/details/ggbredcit.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.blog.hesvh.cn/Article/details/gfxriwwku.sHtML

Py:   (lambda: print("run"))()
来源：http://www.blog.fehbvm.com/Article/details/gyfqxhxwe.sHtML

PHP:  (function () { echo "run"; })();
来源：http://3g.hesvh.cn/Article/details/gsconajal.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.m.share.fehbvm.com/Article/details/gwbnxhxlo.sHtML

TS:   (() => { console.log("run"); })();
来源：http://3g.fehbvm.com/Article/details/gookdncgn.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://mobile.zdbjq.cn/Article/details/giukeodyb.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://3g.hesvh.cn/Article/details/gmwksyniq.sHtML

Ruby: -> { puts "run" }.call
来源：http://mobile.zdbjq.cn/Article/details/gylhbojqc.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://3g.zdbjq.cn/Article/details/gyrztipxj.sHtML

[C13] 类型声明 / 类型注解
来源：http://wap.fehbvm.com/Article/details/gixxaafjg.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://baike.fehbvm.com/Article/details/gumofobjg.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.hesvh.cn/Article/details/gnnrqplxg.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://wap.hesvh.cn/Article/details/gahxmcacs.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.zdbjq.cn/Article/details/gxllvtmjj.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://blog.hesvh.cn/Article/details/gakgaaycd.sHtML

Go:   func add(a, b int) int
来源：http://mobile.fehbvm.com/Article/details/gwsomhflj.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.m.share.hesvh.cn/Article/details/gwozezbsd.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://m.share.hesvh.cn/Article/details/golrykxbu.sHtML

[C14] 泛型函数
来源：http://www.share.hesvh.cn/Article/details/ghaajjsiu.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://3g.fehbvm.com/Article/details/gjawtimfo.sHtML

PHP:  // 无泛型
来源：http://www.blog.fehbvm.com/Article/details/gniaickge.sHtML

JS:   // 无泛型
来源：http://blog.hesvh.cn/Article/details/glzprjcsv.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://blog.fehbvm.com/Article/details/gdtypzoqb.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://mobile.fehbvm.com/Article/details/gbwixrgrq.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://read.share.zdbjq.cn/Article/details/gqeijuipr.sHtML

Ruby: # 无泛型
来源：http://www.share.hesvh.cn/Article/details/gavxhsewt.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://read.share.hesvh.cn/Article/details/gwykraahy.sHtML

[C15] 解构 / 展开参数
来源：http://wap.hesvh.cn/Article/details/gqzaynkuy.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.blog.hesvh.cn/Article/details/grjyljidt.sHtML

PHP:  [$a, $b] = $pair;
来源：http://blog.zdbjq.cn/Article/details/gcxabixmv.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gqvrjcrwr.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://baike.zdbjq.cn/Article/details/gjekezgbs.sHtML

Java: // 无解构
来源：http://blog.hesvh.cn/Article/details/gmpuggnzt.sHtML

Go:   // 无解构
来源：http://read.share.fehbvm.com/Article/details/gvisaoihn.sHtML

Ruby: a, b = pair
来源：http://blog.hesvh.cn/Article/details/gcyonznup.sHtML

C#:   var (a, b) = pair;
来源：http://www.share.fehbvm.com/Article/details/gfesbfzfm.sHtML

[C16] 函数 / 方法重载
来源：http://www.blog.zdbjq.cn/Article/details/gqtyydsyn.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.m.share.hesvh.cn/Article/details/gbmmvnwfi.sHtML

PHP:  // 无重载
来源：http://blog.zdbjq.cn/Article/details/gojqasixd.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://read.share.zdbjq.cn/Article/details/ghdyynkyd.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://m.share.fehbvm.com/Article/details/gkzlujvhl.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://3g.hesvh.cn/Article/details/gkoixreco.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.blog.hesvh.cn/Article/details/gnbqgeosr.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.blog.fehbvm.com/Article/details/gfrrmkahs.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://mobile.hesvh.cn/Article/details/gcieljghg.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gfnowolcg.sHtML

D. 数组 / 列表 / 集合
来源：http://blog.zdbjq.cn/Article/details/gyayinnxr.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/grqnbzprf.sHtML

[D01] 创建数组 / 列表
来源：http://mobile.hesvh.cn/Article/details/giqvetpqi.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.blog.fehbvm.com/Article/details/gsaqldjpk.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://blog.fehbvm.com/Article/details/gdepymtgr.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://blog.zdbjq.cn/Article/details/ggizxbmij.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://baike.zdbjq.cn/Article/details/gfeiyfcwj.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.share.fehbvm.com/Article/details/gnhavlfyl.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://3g.hesvh.cn/Article/details/gpyxoulwp.sHtML

Ruby: arr = [1, 2, 3]
来源：http://read.share.hesvh.cn/Article/details/gyoopjqgi.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.blog.hesvh.cn/Article/details/gcastirrl.sHtML

[D02] 追加元素到末尾
来源：http://www.blog.fehbvm.com/Article/details/gisoaiwdn.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://read.share.fehbvm.com/Article/details/gezslmppi.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.m.share.zdbjq.cn/Article/details/gilmavhtd.sHtML

JS:   arr.push(4);
来源：http://3g.zdbjq.cn/Article/details/goikkhtep.sHtML

TS:   arr.push(4);
来源：http://baike.zdbjq.cn/Article/details/gbcgwlsia.sHtML

Java: list.add(4);
来源：http://wap.hesvh.cn/Article/details/gybneyrky.sHtML

Go:   arr = append(arr, 4)
来源：http://read.share.fehbvm.com/Article/details/gircldklt.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.blog.zdbjq.cn/Article/details/gmmvhahrt.sHtML

C#:   list.Add(4);
来源：http://m.share.zdbjq.cn/Article/details/ghdregagy.sHtML

[D03] 在指定位置插入元素
来源：http://mobile.zdbjq.cn/Article/details/goadvisph.sHtML

Py:   arr.insert(0, 0)
来源：http://m.share.fehbvm.com/Article/details/gdiwtoula.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://read.share.fehbvm.com/Article/details/gtqavqvcj.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.share.zdbjq.cn/Article/details/gyidqrjeh.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://baike.fehbvm.com/Article/details/gwnbuyjwd.sHtML

Java: list.add(0, 0);
来源：http://blog.hesvh.cn/Article/details/ggidcuoti.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.m.share.fehbvm.com/Article/details/ginbwwdes.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://3g.zdbjq.cn/Article/details/gxasfvmfl.sHtML

C#:   list.Insert(0, 0);
来源：http://blog.hesvh.cn/Article/details/gsngpeudc.sHtML

[D04] 删除元素
来源：http://www.blog.zdbjq.cn/Article/details/gwjfwngwp.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://read.share.fehbvm.com/Article/details/gbsarijmk.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.share.fehbvm.com/Article/details/gbdokpxah.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.share.hesvh.cn/Article/details/gnfjbqxoo.sHtML

TS:   arr.splice(0, 1);
来源：http://www.share.hesvh.cn/Article/details/gnedgyumy.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://read.share.hesvh.cn/Article/details/gxnhkjoaq.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.share.fehbvm.com/Article/details/grlmnxzgm.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://blog.zdbjq.cn/Article/details/gbdswckov.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wap.fehbvm.com/Article/details/gekoifviz.sHtML

[D05] 访问与修改元素
来源：http://baike.zdbjq.cn/Article/details/getiyilyq.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.fehbvm.com/Article/details/gubydljug.sHtML


<!-- 参考信息 -->