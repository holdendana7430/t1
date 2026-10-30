代发 wailian999

TS:   for (const item of arr) { console.log(item); }
来源：http://www.share.zdbjq.cn/Article/details/gyskgzdgd.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.m.share.zdbjq.cn/Article/details/gqtdmibgv.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.blog.hesvh.cn/Article/details/gjcethecj.sHtML

Ruby: arr.each { |item| puts item }
来源：http://blog.zdbjq.cn/Article/details/gxknkeooy.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://read.share.fehbvm.com/Article/details/ggexblmaz.sHtML

[B06] 遍历字典 / 对象
来源：http://mobile.zdbjq.cn/Article/details/gxongbiof.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.blog.hesvh.cn/Article/details/gyksjmpjc.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://read.share.zdbjq.cn/Article/details/gblvmrvcf.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.m.share.fehbvm.com/Article/details/gtdukujhy.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://m.share.fehbvm.com/Article/details/gcfdwmhqu.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://read.share.hesvh.cn/Article/details/gzqkfcwvu.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.m.share.fehbvm.com/Article/details/gxgknyujy.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://wap.zdbjq.cn/Article/details/gupvxzovw.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.blog.zdbjq.cn/Article/details/gpkffhsxr.sHtML

[B07] while 循环
来源：http://read.share.hesvh.cn/Article/details/gawinthax.sHtML

Py:   while i < 10: i += 1
来源：http://blog.fehbvm.com/Article/details/gmodqbbki.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://blog.hesvh.cn/Article/details/gvabyufuw.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.share.zdbjq.cn/Article/details/gsovyxyhg.sHtML

TS:   while (i < 10) { i++; }
来源：http://read.share.zdbjq.cn/Article/details/gfwrgbjbn.sHtML

Java: while (i < 10) { i++; }
来源：http://www.m.share.fehbvm.com/Article/details/gnpbspvjr.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://baike.hesvh.cn/Article/details/gzbzgpqsi.sHtML

Ruby: while i < 10; i += 1; end
来源：http://baike.hesvh.cn/Article/details/givncupqq.sHtML

C#:   while (i < 10) { i++; }
来源：http://m.share.zdbjq.cn/Article/details/gokwrkkqb.sHtML

[B08] do-while（至少执行一次）
来源：http://read.share.zdbjq.cn/Article/details/guifjigtf.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://wap.fehbvm.com/Article/details/gajarkpcp.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://wap.zdbjq.cn/Article/details/gneipwrcj.sHtML

JS:   do { i++; } while (i < 10);
来源：http://wap.hesvh.cn/Article/details/gyttjphty.sHtML

TS:   do { i++; } while (i < 10);
来源：http://mobile.hesvh.cn/Article/details/gwaqakhno.sHtML

Java: do { i++; } while (i < 10);
来源：http://mobile.fehbvm.com/Article/details/gwrpkxezi.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.share.fehbvm.com/Article/details/gojzrzgch.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://baike.hesvh.cn/Article/details/gutwpfzsk.sHtML

C#:   do { i++; } while (i < 10);
来源：http://blog.fehbvm.com/Article/details/gjisyrerc.sHtML

[B09] break 与 continue
来源：http://wap.zdbjq.cn/Article/details/gyagwzvqe.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://m.share.hesvh.cn/Article/details/gegevpzmu.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://3g.hesvh.cn/Article/details/gapmlqgsm.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.hesvh.cn/Article/details/gmusitipk.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.fehbvm.com/Article/details/geiiyoawk.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.zdbjq.cn/Article/details/gjycakscz.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://read.share.zdbjq.cn/Article/details/gjpwnfupw.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://wap.fehbvm.com/Article/details/gbmamirzl.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.zdbjq.cn/Article/details/gvkdnzxse.sHtML

[B10] 遍历同时拿索引
来源：http://mobile.hesvh.cn/Article/details/gbgsrfncy.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://m.share.fehbvm.com/Article/details/gyrpwrvcn.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://baike.zdbjq.cn/Article/details/gebuuxtkk.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://wap.fehbvm.com/Article/details/gsybbdvoc.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://3g.zdbjq.cn/Article/details/gurpkkbvu.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://read.share.zdbjq.cn/Article/details/grzfgsrlj.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.share.fehbvm.com/Article/details/giffqduti.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://mobile.zdbjq.cn/Article/details/garyiexia.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.share.hesvh.cn/Article/details/gjmhssmxz.sHtML

[B11] 生成数字序列 / 区间
来源：http://mobile.hesvh.cn/Article/details/gpephfrmr.sHtML

Py:   list(range(0, 10, 2))
来源：http://baike.fehbvm.com/Article/details/gnhrqlraw.sHtML

PHP:  range(0, 10, 2);
来源：http://www.m.share.fehbvm.com/Article/details/gtatswkmu.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.m.share.fehbvm.com/Article/details/gmysrdcrv.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mobile.zdbjq.cn/Article/details/gyghommki.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://3g.fehbvm.com/Article/details/gknsxmmfs.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://wap.fehbvm.com/Article/details/geaiwtabh.sHtML

Ruby: (0...10).step(2).to_a
来源：http://blog.fehbvm.com/Article/details/glyzbidud.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://mobile.hesvh.cn/Article/details/gdqclpeuq.sHtML

[B12] 跳出多层循环
来源：http://3g.hesvh.cn/Article/details/gxqzccgrd.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://wap.fehbvm.com/Article/details/gshlgjejn.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://read.share.zdbjq.cn/Article/details/gubilmoas.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.zdbjq.cn/Article/details/gpsqxizhv.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://baike.zdbjq.cn/Article/details/ginswxmew.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.hesvh.cn/Article/details/gvklnvabe.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://m.share.fehbvm.com/Article/details/grcjvguma.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://wap.fehbvm.com/Article/details/gckiomrjv.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://read.share.fehbvm.com/Article/details/gxxktwjiu.sHtML

[B13] 判断是否为数字
来源：http://www.blog.hesvh.cn/Article/details/gsdxpffly.sHtML

Py:   isinstance(x, (int, float))
来源：http://wap.zdbjq.cn/Article/details/gkrcgalac.sHtML

PHP:  is_numeric($x)
来源：http://3g.zdbjq.cn/Article/details/gljtovmex.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.hesvh.cn/Article/details/gltbcijhq.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.hesvh.cn/Article/details/gcrzrvixb.sHtML

Java: x instanceof Number
来源：http://www.blog.fehbvm.com/Article/details/gcqljpzzm.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://blog.hesvh.cn/Article/details/galnjuvnt.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.m.share.zdbjq.cn/Article/details/girftzmbz.sHtML

C#:   x is int or double or decimal
来源：http://mobile.zdbjq.cn/Article/details/glfwbnlpy.sHtML

[B14] 判断值是否在集合内
来源：http://m.share.hesvh.cn/Article/details/gsnemnxan.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://3g.hesvh.cn/Article/details/gmevapyvp.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://blog.hesvh.cn/Article/details/gganatbnj.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://wap.hesvh.cn/Article/details/glvvbxbmp.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://3g.hesvh.cn/Article/details/gdizjsjrf.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://mobile.hesvh.cn/Article/details/gsidnkckb.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://3g.hesvh.cn/Article/details/gfmwfmzaf.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.m.share.hesvh.cn/Article/details/gfxyjzzci.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://blog.zdbjq.cn/Article/details/getdnldps.sHtML

[B15] 布尔运算与取反
来源：http://wap.hesvh.cn/Article/details/gtktoudma.sHtML

Py:   a and b or not c
来源：http://www.blog.fehbvm.com/Article/details/gsfhmtsnr.sHtML

PHP:  $a && $b || !$c
来源：http://read.share.zdbjq.cn/Article/details/ggtvhrjne.sHtML

JS:   a && b || !c
来源：http://baike.hesvh.cn/Article/details/gtlefnqry.sHtML

TS:   a && b || !c
来源：http://blog.hesvh.cn/Article/details/gmzvqkxhd.sHtML

Java: a && b || !c
来源：http://read.share.hesvh.cn/Article/details/gbdclgpkc.sHtML

Go:   a && b || !c
来源：http://baike.zdbjq.cn/Article/details/ghnkllmfy.sHtML

Ruby: a && b || !c
来源：http://wap.fehbvm.com/Article/details/gkgktvulu.sHtML

C#:   a && b || !c
来源：http://read.share.fehbvm.com/Article/details/gjkwygbsh.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://wap.fehbvm.com/Article/details/gygmwylao.sHtML

Py:   if not data: return
来源：http://baike.zdbjq.cn/Article/details/grzkwvjwm.sHtML

PHP:  if (!$data) { return; }
来源：http://mobile.fehbvm.com/Article/details/ghudmitzx.sHtML

JS:   if (!data) return;
来源：http://mobile.zdbjq.cn/Article/details/gjxmwvdjn.sHtML

TS:   if (!data) return;
来源：http://m.share.hesvh.cn/Article/details/gnbfbwhnf.sHtML

Java: if (data == null) return;
来源：http://m.share.fehbvm.com/Article/details/gmtowgncc.sHtML

Go:   if data == nil { return }
来源：http://blog.hesvh.cn/Article/details/gllcdrvgg.sHtML

Ruby: return if data.nil?
来源：http://mobile.hesvh.cn/Article/details/gdjjesxve.sHtML

C#:   if (data == null) return;
来源：http://baike.fehbvm.com/Article/details/glcwhpnqd.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gqtpgjqpe.sHtML

C. 函数与作用域
来源：http://mobile.zdbjq.cn/Article/details/gautcmwmn.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gfcezsipe.sHtML

[C01] 定义函数
来源：http://www.share.zdbjq.cn/Article/details/gfwsszqoa.sHtML

Py:   def add(a, b): return a + b
来源：http://blog.zdbjq.cn/Article/details/gpfajlcof.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.fehbvm.com/Article/details/gtqdcnyrs.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://blog.hesvh.cn/Article/details/gnlkdmjvl.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.zdbjq.cn/Article/details/gsboiywrz.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.m.share.fehbvm.com/Article/details/gskyhmuuj.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.m.share.zdbjq.cn/Article/details/grlybajvn.sHtML

Ruby: def add(a, b); a + b; end
来源：http://mobile.fehbvm.com/Article/details/glgvxwjeq.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://wap.zdbjq.cn/Article/details/gkaigxngq.sHtML

[C02] 默认参数
来源：http://wap.hesvh.cn/Article/details/ghhvwooyq.sHtML

Py:   def greet(name="World"): return name
来源：http://wap.fehbvm.com/Article/details/gqivdlvlk.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://baike.zdbjq.cn/Article/details/gbpdvscat.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.blog.zdbjq.cn/Article/details/goygsqray.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://baike.hesvh.cn/Article/details/gbklsiwiv.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://read.share.fehbvm.com/Article/details/gqngsjase.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://mobile.hesvh.cn/Article/details/gnlbdwxpr.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.m.share.zdbjq.cn/Article/details/gpkkolizp.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://blog.fehbvm.com/Article/details/gsaauyvla.sHtML

[C03] 可变参数
来源：http://baike.zdbjq.cn/Article/details/gmngwtqkd.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.blog.fehbvm.com/Article/details/gyaibasph.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://mobile.fehbvm.com/Article/details/gdvuqirsa.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.hesvh.cn/Article/details/gyfcbvhnk.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.fehbvm.com/Article/details/gosnqpvju.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://blog.hesvh.cn/Article/details/gzwjrprxr.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.m.share.fehbvm.com/Article/details/ggsliykeb.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://blog.zdbjq.cn/Article/details/gtvghdosx.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://m.share.zdbjq.cn/Article/details/gczhrqthh.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.share.hesvh.cn/Article/details/giwregjdf.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://read.share.zdbjq.cn/Article/details/grsolwzff.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://read.share.zdbjq.cn/Article/details/gdxnpsioa.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://blog.hesvh.cn/Article/details/goohxluqc.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://read.share.hesvh.cn/Article/details/gwotjmcmk.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.blog.fehbvm.com/Article/details/gohueoolx.sHtML

Go:   // 无：用配置结构体参数
来源：http://3g.fehbvm.com/Article/details/gdpploxjn.sHtML

Ruby: f(a: 1, b: 2)
来源：http://wap.hesvh.cn/Article/details/gwpsntpsz.sHtML

C#:   f(a: 1, b: 2)
来源：http://baike.hesvh.cn/Article/details/ghuyyvaht.sHtML

[C05] 返回多个值
来源：http://mobile.fehbvm.com/Article/details/gaofupcvz.sHtML

Py:   return a, b
来源：http://mobile.hesvh.cn/Article/details/gorovtnwr.sHtML

PHP:  return [$a, $b];
来源：http://m.share.fehbvm.com/Article/details/gapjiyuxf.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.blog.fehbvm.com/Article/details/gbhlkdwkp.sHtML

TS:   return { a, b };
来源：http://read.share.hesvh.cn/Article/details/ggfdtucad.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.blog.hesvh.cn/Article/details/gcwuwyvgh.sHtML

Go:   return a, b
来源：http://www.blog.hesvh.cn/Article/details/gtwonxjui.sHtML

Ruby: return a, b
来源：http://3g.fehbvm.com/Article/details/gqyuhcehx.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://wap.hesvh.cn/Article/details/gzwyckkfm.sHtML

[C06] 匿名函数 / lambda
来源：http://www.blog.fehbvm.com/Article/details/guxmavbzl.sHtML

Py:   square = lambda x: x * x
来源：http://wap.hesvh.cn/Article/details/gxfceszop.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://blog.fehbvm.com/Article/details/gcqvcgbwj.sHtML

JS:   const square = x => x * x;
来源：http://m.share.zdbjq.cn/Article/details/gqalnsaea.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.share.fehbvm.com/Article/details/gfidxozzp.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.blog.fehbvm.com/Article/details/gktgjuqwg.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://3g.fehbvm.com/Article/details/ggboxdduw.sHtML

Ruby: square = ->(x) { x * x }
来源：http://mobile.fehbvm.com/Article/details/ghxmqnkce.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://read.share.zdbjq.cn/Article/details/gvipijiqb.sHtML

[C07] 把函数作为参数传入
来源：http://baike.hesvh.cn/Article/details/goufvaizw.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://m.share.hesvh.cn/Article/details/gjagojdhl.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://3g.hesvh.cn/Article/details/gpflelhic.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://m.share.hesvh.cn/Article/details/gqjibkbuw.sHtML

TS:   arr.map(String)
来源：http://www.m.share.zdbjq.cn/Article/details/gkitkkvqg.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.m.share.fehbvm.com/Article/details/gqxazlgjm.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.blog.zdbjq.cn/Article/details/gvxtnfhwu.sHtML

Ruby: arr.map(&:upcase)
来源：http://mobile.hesvh.cn/Article/details/ghhgqqvla.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://wap.hesvh.cn/Article/details/gmlyhsjtu.sHtML

[C08] 闭包
来源：http://baike.zdbjq.cn/Article/details/gaxdnytxe.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://3g.zdbjq.cn/Article/details/gyqdgprcm.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.blog.hesvh.cn/Article/details/gzvokvyux.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.blog.zdbjq.cn/Article/details/ggtderwaz.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://3g.fehbvm.com/Article/details/gbwftudgn.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://mobile.hesvh.cn/Article/details/gwmdafcps.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://baike.fehbvm.com/Article/details/gotgexueg.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.blog.fehbvm.com/Article/details/gmbwxqrlp.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.m.share.hesvh.cn/Article/details/gvxmqslin.sHtML

[C09] 递归
来源：http://m.share.hesvh.cn/Article/details/gqgvauhlw.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://m.share.fehbvm.com/Article/details/gfyvfcrfr.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://wap.hesvh.cn/Article/details/glfelckqj.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.zdbjq.cn/Article/details/gupxbjixf.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.hesvh.cn/Article/details/gctqayzry.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://mobile.zdbjq.cn/Article/details/glkldajaz.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.m.share.zdbjq.cn/Article/details/gyhhcxfmt.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.blog.hesvh.cn/Article/details/grjekkjqj.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.blog.zdbjq.cn/Article/details/gselcemrf.sHtML

[C10] 变量作用域
来源：http://wap.hesvh.cn/Article/details/gfawpgfmi.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.m.share.hesvh.cn/Article/details/gjyzqjrmz.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://m.share.hesvh.cn/Article/details/gokixkkye.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://mobile.zdbjq.cn/Article/details/gcsezzdfw.sHtML

TS:   同 JS
来源：http://blog.hesvh.cn/Article/details/gmbtuueyl.sHtML

Java: 方法内为块级作用域
来源：http://www.m.share.hesvh.cn/Article/details/ginupcyis.sHtML

Go:   花括号块级作用域
来源：http://blog.zdbjq.cn/Article/details/gkjsjkwhd.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://read.share.hesvh.cn/Article/details/gcomugsfm.sHtML

C#:   块级作用域
来源：http://blog.hesvh.cn/Article/details/gwesedonc.sHtML

[C11] 模块导入与导出
来源：http://www.share.zdbjq.cn/Article/details/glqqauwkg.sHtML

Py:   from module import func
来源：http://www.share.fehbvm.com/Article/details/gcukoktjt.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.share.hesvh.cn/Article/details/gtxjibhum.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://read.share.zdbjq.cn/Article/details/gnugsxedm.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://mobile.hesvh.cn/Article/details/gvltexgzi.sHtML

Java: import java.util.List;
来源：http://3g.hesvh.cn/Article/details/gjhbmnxse.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.share.zdbjq.cn/Article/details/graykbpng.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://blog.hesvh.cn/Article/details/gjqhpvzrc.sHtML

C#:   using System.Text;
来源：http://wap.zdbjq.cn/Article/details/gdxzeptyd.sHtML

[C12] 立即执行函数 IIFE
来源：http://baike.zdbjq.cn/Article/details/gomyqijhv.sHtML

Py:   (lambda: print("run"))()
来源：http://www.blog.zdbjq.cn/Article/details/gvbwedyzs.sHtML

PHP:  (function () { echo "run"; })();
来源：http://blog.fehbvm.com/Article/details/gcsdxnmiy.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.m.share.hesvh.cn/Article/details/gcyhylscn.sHtML

TS:   (() => { console.log("run"); })();
来源：http://wap.fehbvm.com/Article/details/gmbieubta.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.m.share.hesvh.cn/Article/details/gzwsrmper.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.m.share.zdbjq.cn/Article/details/gwpwwrfpw.sHtML

Ruby: -> { puts "run" }.call
来源：http://wap.fehbvm.com/Article/details/gxpvwtpsb.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://3g.zdbjq.cn/Article/details/galdyvnen.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.m.share.zdbjq.cn/Article/details/gcxmsvvtn.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.m.share.hesvh.cn/Article/details/gblaxpkjz.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.zdbjq.cn/Article/details/gblthfvkh.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://baike.hesvh.cn/Article/details/gsttqywwq.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.fehbvm.com/Article/details/gkzjhkgrx.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://blog.zdbjq.cn/Article/details/gontwzmcl.sHtML

Go:   func add(a, b int) int
来源：http://www.blog.zdbjq.cn/Article/details/gsffzciov.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.m.share.fehbvm.com/Article/details/gqxihuphp.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://read.share.fehbvm.com/Article/details/gbjqklxkb.sHtML

[C14] 泛型函数
来源：http://blog.hesvh.cn/Article/details/ghkjoqykr.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://mobile.hesvh.cn/Article/details/gowkmveid.sHtML

PHP:  // 无泛型
来源：http://mobile.fehbvm.com/Article/details/gmlsbetpc.sHtML

JS:   // 无泛型
来源：http://3g.hesvh.cn/Article/details/ghldrhvrw.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.share.fehbvm.com/Article/details/gyyecqgvn.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://m.share.hesvh.cn/Article/details/gmoltbujr.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.blog.fehbvm.com/Article/details/gfiauvzqb.sHtML

Ruby: # 无泛型
来源：http://www.m.share.fehbvm.com/Article/details/gdmonspjv.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://m.share.fehbvm.com/Article/details/gfrgwgxhj.sHtML

[C15] 解构 / 展开参数
来源：http://3g.fehbvm.com/Article/details/gkigmqogc.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://baike.hesvh.cn/Article/details/grrghzdtn.sHtML

PHP:  [$a, $b] = $pair;
来源：http://3g.fehbvm.com/Article/details/ggyzhllfe.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://m.share.zdbjq.cn/Article/details/gnslvzxlw.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://baike.hesvh.cn/Article/details/ggyesppjy.sHtML

Java: // 无解构
来源：http://read.share.hesvh.cn/Article/details/gtgjiqvre.sHtML

Go:   // 无解构
来源：http://wap.zdbjq.cn/Article/details/gucdlnnpr.sHtML

Ruby: a, b = pair
来源：http://www.m.share.fehbvm.com/Article/details/gehgiqmct.sHtML

C#:   var (a, b) = pair;
来源：http://blog.fehbvm.com/Article/details/gsagphazc.sHtML

[C16] 函数 / 方法重载
来源：http://m.share.hesvh.cn/Article/details/giwxjiinl.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://mobile.zdbjq.cn/Article/details/glramwgfx.sHtML

PHP:  // 无重载
来源：http://mobile.fehbvm.com/Article/details/gupfzodjp.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.blog.zdbjq.cn/Article/details/gyljkmtcl.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.blog.hesvh.cn/Article/details/gfesxtydu.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://read.share.hesvh.cn/Article/details/gzioyofqn.sHtML

Go:   // 无重载：用不同函数名
来源：http://wap.hesvh.cn/Article/details/gxmfcesov.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.share.zdbjq.cn/Article/details/gglfpbdhk.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://blog.fehbvm.com/Article/details/gjqtntvis.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gthbzgahy.sHtML

D. 数组 / 列表 / 集合
来源：http://www.share.zdbjq.cn/Article/details/glbneyytj.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gevkrydbh.sHtML

[D01] 创建数组 / 列表
来源：http://blog.hesvh.cn/Article/details/grjihewzt.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://read.share.fehbvm.com/Article/details/gqppabywa.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://m.share.zdbjq.cn/Article/details/gfvycbvte.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://m.share.zdbjq.cn/Article/details/ghcncunkm.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://wap.zdbjq.cn/Article/details/gewqidgdl.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wap.fehbvm.com/Article/details/gcbnvxagr.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://3g.fehbvm.com/Article/details/gkurjmzlh.sHtML

Ruby: arr = [1, 2, 3]
来源：http://wap.zdbjq.cn/Article/details/gjlbmxhhh.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://wap.hesvh.cn/Article/details/gkvgpjzmy.sHtML

[D02] 追加元素到末尾
来源：http://mobile.hesvh.cn/Article/details/garuabuoc.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://baike.fehbvm.com/Article/details/gwxpcsdwg.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://blog.zdbjq.cn/Article/details/gvokcsqmg.sHtML

JS:   arr.push(4);
来源：http://wap.fehbvm.com/Article/details/gsjlclnfi.sHtML

TS:   arr.push(4);
来源：http://read.share.fehbvm.com/Article/details/gizuebvmj.sHtML

Java: list.add(4);
来源：http://mobile.fehbvm.com/Article/details/gxyccvgui.sHtML

Go:   arr = append(arr, 4)
来源：http://wap.fehbvm.com/Article/details/gpjdlhguk.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.share.zdbjq.cn/Article/details/gsymfdpfi.sHtML

C#:   list.Add(4);
来源：http://read.share.hesvh.cn/Article/details/gqeonrvop.sHtML

[D03] 在指定位置插入元素
来源：http://mobile.hesvh.cn/Article/details/gaptkpgdo.sHtML

Py:   arr.insert(0, 0)
来源：http://read.share.hesvh.cn/Article/details/ggpwiormw.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://blog.fehbvm.com/Article/details/gjizvykmv.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://mobile.hesvh.cn/Article/details/gfihhgyqt.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://baike.hesvh.cn/Article/details/gaqgftgzq.sHtML

Java: list.add(0, 0);
来源：http://3g.fehbvm.com/Article/details/gozaojoxp.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://wap.zdbjq.cn/Article/details/goaiucjvi.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.m.share.fehbvm.com/Article/details/gdyxjmbtd.sHtML

C#:   list.Insert(0, 0);
来源：http://wap.zdbjq.cn/Article/details/gpmpaasex.sHtML

[D04] 删除元素
来源：http://www.blog.zdbjq.cn/Article/details/gqazeeauj.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.share.zdbjq.cn/Article/details/gmyqszsgt.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.share.zdbjq.cn/Article/details/gwywwxnyk.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://3g.zdbjq.cn/Article/details/gsdoufizl.sHtML

TS:   arr.splice(0, 1);
来源：http://mobile.zdbjq.cn/Article/details/gguymeglg.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://baike.hesvh.cn/Article/details/gyxbkitmg.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://wap.hesvh.cn/Article/details/gyedqeoio.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://baike.zdbjq.cn/Article/details/gosdckxdc.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.blog.zdbjq.cn/Article/details/gtbjlqncp.sHtML

[D05] 访问与修改元素
来源：http://baike.fehbvm.com/Article/details/giidzvzlo.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.zdbjq.cn/Article/details/gurhkqfzl.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.share.zdbjq.cn/Article/details/gmbhnivsr.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.share.hesvh.cn/Article/details/gscngkeub.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://read.share.zdbjq.cn/Article/details/gkutmhekm.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.m.share.hesvh.cn/Article/details/gfaovqetp.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://mobile.hesvh.cn/Article/details/gxdhjpbve.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.hesvh.cn/Article/details/gtgpcuiqm.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://read.share.hesvh.cn/Article/details/gxyotjmrw.sHtML

[D06] 数组长度
来源：http://m.share.hesvh.cn/Article/details/gvjiiqcnq.sHtML


<!-- 参考信息 -->