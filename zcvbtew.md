代发 wailian999

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://3g.zdbjq.cn/Article/details/gyvsdjyvn.sHtML

[B06] 遍历字典 / 对象
来源：http://www.share.fehbvm.com/Article/details/giblcwalh.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://blog.zdbjq.cn/Article/details/gexuzfcic.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://blog.zdbjq.cn/Article/details/gwedfigcg.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mobile.fehbvm.com/Article/details/golosmifz.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.blog.hesvh.cn/Article/details/gzscbevmh.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.blog.hesvh.cn/Article/details/gjcwvadcb.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://mobile.fehbvm.com/Article/details/goittbnrr.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://baike.fehbvm.com/Article/details/gfuxazada.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://read.share.hesvh.cn/Article/details/grcknfiws.sHtML

[B07] while 循环
来源：http://www.m.share.fehbvm.com/Article/details/gyqbkozhr.sHtML

Py:   while i < 10: i += 1
来源：http://mobile.hesvh.cn/Article/details/gfustvqxd.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.m.share.fehbvm.com/Article/details/gkrborsfn.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.m.share.zdbjq.cn/Article/details/gcwpykxmi.sHtML

TS:   while (i < 10) { i++; }
来源：http://wap.hesvh.cn/Article/details/glvajmllz.sHtML

Java: while (i < 10) { i++; }
来源：http://www.blog.zdbjq.cn/Article/details/gvwnfblal.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://read.share.fehbvm.com/Article/details/gjkpruezc.sHtML

Ruby: while i < 10; i += 1; end
来源：http://3g.fehbvm.com/Article/details/gcevtuwdp.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.share.zdbjq.cn/Article/details/ghxihxood.sHtML

[B08] do-while（至少执行一次）
来源：http://www.m.share.zdbjq.cn/Article/details/gdpgykdjk.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://m.share.zdbjq.cn/Article/details/gnkqycwky.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://wap.zdbjq.cn/Article/details/ggasnwtpo.sHtML

JS:   do { i++; } while (i < 10);
来源：http://3g.fehbvm.com/Article/details/ghvbvbutv.sHtML

TS:   do { i++; } while (i < 10);
来源：http://3g.hesvh.cn/Article/details/gjqxwmcmo.sHtML

Java: do { i++; } while (i < 10);
来源：http://3g.hesvh.cn/Article/details/gilcjeugl.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://m.share.zdbjq.cn/Article/details/gzyrxovqc.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://mobile.fehbvm.com/Article/details/gusamkplh.sHtML

C#:   do { i++; } while (i < 10);
来源：http://m.share.hesvh.cn/Article/details/gtrcyuzjd.sHtML

[B09] break 与 continue
来源：http://blog.fehbvm.com/Article/details/gqnetywnc.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://m.share.hesvh.cn/Article/details/gbznfajrg.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://3g.zdbjq.cn/Article/details/gtiodvotw.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.zdbjq.cn/Article/details/gjijcwjwa.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.fehbvm.com/Article/details/gxkukietg.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.hesvh.cn/Article/details/gpkoowjhy.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.blog.fehbvm.com/Article/details/gfagcazkt.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://wap.fehbvm.com/Article/details/gqeojycmf.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.fehbvm.com/Article/details/gishedhos.sHtML

[B10] 遍历同时拿索引
来源：http://www.blog.fehbvm.com/Article/details/gmtzqgcgy.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://mobile.zdbjq.cn/Article/details/gddrwplxm.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://baike.hesvh.cn/Article/details/gikjlperc.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://baike.fehbvm.com/Article/details/geuwvwmrh.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.blog.fehbvm.com/Article/details/gvtcdsmbd.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.m.share.hesvh.cn/Article/details/gbowpgkcs.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://blog.fehbvm.com/Article/details/gfpwvtocu.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://wap.hesvh.cn/Article/details/gpjykizqm.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.m.share.hesvh.cn/Article/details/ghswdpkor.sHtML

[B11] 生成数字序列 / 区间
来源：http://m.share.zdbjq.cn/Article/details/gmlikwkcl.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.blog.zdbjq.cn/Article/details/ghygxayuy.sHtML

PHP:  range(0, 10, 2);
来源：http://read.share.hesvh.cn/Article/details/gdeiiwfzn.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://m.share.hesvh.cn/Article/details/gkwdiaupz.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://m.share.hesvh.cn/Article/details/gipogiuar.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.m.share.zdbjq.cn/Article/details/gtwzamzue.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://m.share.zdbjq.cn/Article/details/gcmcsytcx.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.m.share.hesvh.cn/Article/details/gdbtoehaq.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://read.share.hesvh.cn/Article/details/gjlzbjman.sHtML

[B12] 跳出多层循环
来源：http://baike.fehbvm.com/Article/details/gigcpzihk.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://read.share.fehbvm.com/Article/details/gaqionjhk.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://mobile.fehbvm.com/Article/details/gekvjifgz.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.zdbjq.cn/Article/details/gaamdlrgo.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.fehbvm.com/Article/details/gbicgxcwg.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://mobile.fehbvm.com/Article/details/gutujievu.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://baike.zdbjq.cn/Article/details/gtxxcrgbu.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://read.share.hesvh.cn/Article/details/gcxgzuorf.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://read.share.zdbjq.cn/Article/details/gshtlizdm.sHtML

[B13] 判断是否为数字
来源：http://read.share.hesvh.cn/Article/details/gaegnafud.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.blog.fehbvm.com/Article/details/grthydbpc.sHtML

PHP:  is_numeric($x)
来源：http://www.blog.hesvh.cn/Article/details/godxszawa.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.hesvh.cn/Article/details/gpltntxko.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gtixbkxdp.sHtML

Java: x instanceof Number
来源：http://3g.fehbvm.com/Article/details/gvskosuqs.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://3g.hesvh.cn/Article/details/gksibsdci.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.share.zdbjq.cn/Article/details/gqoribumw.sHtML

C#:   x is int or double or decimal
来源：http://wap.zdbjq.cn/Article/details/grszwdsub.sHtML

[B14] 判断值是否在集合内
来源：http://www.m.share.hesvh.cn/Article/details/gmegqpvpk.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://blog.zdbjq.cn/Article/details/gwttvgoce.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.share.fehbvm.com/Article/details/gtgxjybob.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://blog.fehbvm.com/Article/details/gzbszzwtq.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://read.share.fehbvm.com/Article/details/gvgwledve.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://read.share.hesvh.cn/Article/details/gvjzoeouz.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.blog.zdbjq.cn/Article/details/gbpkandwt.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.blog.zdbjq.cn/Article/details/gaqhyqxlv.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://read.share.zdbjq.cn/Article/details/gsbqcbxku.sHtML

[B15] 布尔运算与取反
来源：http://baike.fehbvm.com/Article/details/gbaajpqhl.sHtML

Py:   a and b or not c
来源：http://www.m.share.hesvh.cn/Article/details/gapxhvtlv.sHtML

PHP:  $a && $b || !$c
来源：http://blog.zdbjq.cn/Article/details/gdyxishml.sHtML

JS:   a && b || !c
来源：http://www.blog.zdbjq.cn/Article/details/gyrgplsyi.sHtML

TS:   a && b || !c
来源：http://read.share.fehbvm.com/Article/details/gfqewmkhe.sHtML

Java: a && b || !c
来源：http://baike.hesvh.cn/Article/details/gddvdfxgm.sHtML

Go:   a && b || !c
来源：http://wap.hesvh.cn/Article/details/grexnoavl.sHtML

Ruby: a && b || !c
来源：http://www.share.zdbjq.cn/Article/details/gofpfbkhj.sHtML

C#:   a && b || !c
来源：http://m.share.zdbjq.cn/Article/details/gtzrmiegu.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.blog.fehbvm.com/Article/details/gyvegbdfp.sHtML

Py:   if not data: return
来源：http://www.m.share.hesvh.cn/Article/details/gosxhhmcp.sHtML

PHP:  if (!$data) { return; }
来源：http://read.share.fehbvm.com/Article/details/gjnxfkmnn.sHtML

JS:   if (!data) return;
来源：http://m.share.fehbvm.com/Article/details/gkqquoivv.sHtML

TS:   if (!data) return;
来源：http://blog.zdbjq.cn/Article/details/gvghlmjxf.sHtML

Java: if (data == null) return;
来源：http://wap.zdbjq.cn/Article/details/gpxsvnxxr.sHtML

Go:   if data == nil { return }
来源：http://www.m.share.zdbjq.cn/Article/details/gkacvsikr.sHtML

Ruby: return if data.nil?
来源：http://www.share.zdbjq.cn/Article/details/gbllyqgnj.sHtML

C#:   if (data == null) return;
来源：http://www.m.share.fehbvm.com/Article/details/gjwlxulzx.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gpuowszln.sHtML

C. 函数与作用域
来源：http://www.blog.hesvh.cn/Article/details/glugkrpmg.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gohhxaozf.sHtML

[C01] 定义函数
来源：http://m.share.zdbjq.cn/Article/details/gvmovlbpb.sHtML

Py:   def add(a, b): return a + b
来源：http://baike.zdbjq.cn/Article/details/gcjnonodk.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.hesvh.cn/Article/details/gtrjjsopg.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.blog.zdbjq.cn/Article/details/gsrunfdwf.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.hesvh.cn/Article/details/gxutijznm.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://blog.zdbjq.cn/Article/details/gjuwzazyr.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.share.fehbvm.com/Article/details/gymodblvb.sHtML

Ruby: def add(a, b); a + b; end
来源：http://wap.fehbvm.com/Article/details/ghhqnqkcd.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://baike.hesvh.cn/Article/details/gafgmfaws.sHtML

[C02] 默认参数
来源：http://mobile.hesvh.cn/Article/details/gebhcnrik.sHtML

Py:   def greet(name="World"): return name
来源：http://mobile.fehbvm.com/Article/details/gisjderzi.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://mobile.hesvh.cn/Article/details/gyplcfgml.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.blog.hesvh.cn/Article/details/gdlgusowr.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://m.share.fehbvm.com/Article/details/gislnmwdu.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://m.share.fehbvm.com/Article/details/gnmujvhcy.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://m.share.hesvh.cn/Article/details/glctryccf.sHtML

Ruby: def greet(name = "World") = name
来源：http://mobile.zdbjq.cn/Article/details/ghpbicuki.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://mobile.hesvh.cn/Article/details/gktkrcknj.sHtML

[C03] 可变参数
来源：http://www.blog.hesvh.cn/Article/details/gcbttukzl.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.m.share.fehbvm.com/Article/details/guwxtgsfa.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://mobile.fehbvm.com/Article/details/gzdnjtqfz.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.fehbvm.com/Article/details/gnqhrdmwm.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.zdbjq.cn/Article/details/gszakaldg.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.share.zdbjq.cn/Article/details/gkbuwlcbj.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://mobile.hesvh.cn/Article/details/gvstxzdag.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://wap.fehbvm.com/Article/details/goqcndrnm.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.blog.fehbvm.com/Article/details/gqwcrpewv.sHtML

[C04] 命名参数 / 关键字参数
来源：http://blog.hesvh.cn/Article/details/gtfpvhztg.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://m.share.fehbvm.com/Article/details/gafyvziwl.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://m.share.fehbvm.com/Article/details/gniqpuyqy.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.share.hesvh.cn/Article/details/gvxsteodb.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.m.share.hesvh.cn/Article/details/gguoehtyd.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://mobile.zdbjq.cn/Article/details/grjscsjaj.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.blog.fehbvm.com/Article/details/gthblulvt.sHtML

Ruby: f(a: 1, b: 2)
来源：http://m.share.zdbjq.cn/Article/details/gvbckyxdk.sHtML

C#:   f(a: 1, b: 2)
来源：http://mobile.hesvh.cn/Article/details/gfqpcghtz.sHtML

[C05] 返回多个值
来源：http://baike.fehbvm.com/Article/details/ghqougqmu.sHtML

Py:   return a, b
来源：http://baike.fehbvm.com/Article/details/gdgbedqen.sHtML

PHP:  return [$a, $b];
来源：http://mobile.hesvh.cn/Article/details/gjfuiqxyi.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.m.share.zdbjq.cn/Article/details/gxrvabuvg.sHtML

TS:   return { a, b };
来源：http://blog.zdbjq.cn/Article/details/gmcufavhf.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://baike.fehbvm.com/Article/details/glxlhpeev.sHtML

Go:   return a, b
来源：http://www.m.share.fehbvm.com/Article/details/gffwlqysx.sHtML

Ruby: return a, b
来源：http://blog.hesvh.cn/Article/details/gpidhydbc.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://3g.hesvh.cn/Article/details/ggkfdwvyb.sHtML

[C06] 匿名函数 / lambda
来源：http://mobile.hesvh.cn/Article/details/gbgthjppa.sHtML

Py:   square = lambda x: x * x
来源：http://mobile.fehbvm.com/Article/details/gqnsqxnej.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://baike.zdbjq.cn/Article/details/gwehcgfcj.sHtML

JS:   const square = x => x * x;
来源：http://baike.zdbjq.cn/Article/details/gporcadoy.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://read.share.zdbjq.cn/Article/details/glilroggf.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://mobile.zdbjq.cn/Article/details/guyyiuhsq.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.share.zdbjq.cn/Article/details/gllmmlsap.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.blog.zdbjq.cn/Article/details/gyxyjiuhr.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://read.share.zdbjq.cn/Article/details/guuozqzcr.sHtML

[C07] 把函数作为参数传入
来源：http://www.share.fehbvm.com/Article/details/gcsasagmx.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.share.hesvh.cn/Article/details/gbmasmthi.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://read.share.hesvh.cn/Article/details/gahsvwwhp.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.m.share.fehbvm.com/Article/details/gcyevdkiu.sHtML

TS:   arr.map(String)
来源：http://m.share.hesvh.cn/Article/details/gyhpksmof.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.m.share.fehbvm.com/Article/details/gfqmtyxcm.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://mobile.fehbvm.com/Article/details/gjlutoocd.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.blog.fehbvm.com/Article/details/gmhamfnbl.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://blog.zdbjq.cn/Article/details/gxmcbiuoo.sHtML

[C08] 闭包
来源：http://3g.hesvh.cn/Article/details/gdnupawng.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.share.fehbvm.com/Article/details/gkogbefny.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://m.share.fehbvm.com/Article/details/ghebxovdf.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.share.zdbjq.cn/Article/details/gjsyawmml.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://3g.zdbjq.cn/Article/details/gfapzetwb.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.share.zdbjq.cn/Article/details/gubkrbenh.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://baike.hesvh.cn/Article/details/gctbeeifc.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://baike.fehbvm.com/Article/details/gnckpbnjo.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://read.share.hesvh.cn/Article/details/glcuqphzh.sHtML

[C09] 递归
来源：http://3g.zdbjq.cn/Article/details/gglupufxv.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://3g.zdbjq.cn/Article/details/gtqhfpnnw.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://3g.hesvh.cn/Article/details/gvafmkuly.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.fehbvm.com/Article/details/gczfdqwze.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.zdbjq.cn/Article/details/gbuuoaxgp.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://mobile.hesvh.cn/Article/details/gmxqjkkze.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.m.share.zdbjq.cn/Article/details/gdspmfaye.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://read.share.zdbjq.cn/Article/details/gomcjpdma.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://mobile.hesvh.cn/Article/details/gboprcmlu.sHtML

[C10] 变量作用域
来源：http://mobile.zdbjq.cn/Article/details/gkihbtasy.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.blog.hesvh.cn/Article/details/gqjwokfko.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://read.share.fehbvm.com/Article/details/gcahjtqgj.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.blog.fehbvm.com/Article/details/gsfcjbjpr.sHtML

TS:   同 JS
来源：http://www.blog.hesvh.cn/Article/details/gcltvslkj.sHtML

Java: 方法内为块级作用域
来源：http://baike.hesvh.cn/Article/details/gioboiiby.sHtML

Go:   花括号块级作用域
来源：http://www.blog.fehbvm.com/Article/details/golfezhej.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://read.share.fehbvm.com/Article/details/gbhiwmcyz.sHtML

C#:   块级作用域
来源：http://baike.hesvh.cn/Article/details/geuayycmw.sHtML

[C11] 模块导入与导出
来源：http://read.share.zdbjq.cn/Article/details/gbbnpmyfc.sHtML

Py:   from module import func
来源：http://blog.zdbjq.cn/Article/details/gggpnrfhy.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.share.zdbjq.cn/Article/details/gihsxqqwr.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.share.fehbvm.com/Article/details/gcwpfjgsq.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.share.fehbvm.com/Article/details/gbezyklef.sHtML

Java: import java.util.List;
来源：http://www.m.share.zdbjq.cn/Article/details/ggmaortkh.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://blog.fehbvm.com/Article/details/gsahezumc.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.blog.hesvh.cn/Article/details/gyasmyoxv.sHtML

C#:   using System.Text;
来源：http://blog.fehbvm.com/Article/details/gkumssvum.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.blog.hesvh.cn/Article/details/gszhtfihh.sHtML

Py:   (lambda: print("run"))()
来源：http://baike.zdbjq.cn/Article/details/gjtasszkr.sHtML

PHP:  (function () { echo "run"; })();
来源：http://m.share.zdbjq.cn/Article/details/ggogxvwzs.sHtML

JS:   (() => { console.log("run"); })();
来源：http://baike.hesvh.cn/Article/details/gaaatvtvd.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.blog.zdbjq.cn/Article/details/gsgkcsoby.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wap.hesvh.cn/Article/details/gqvdnhuzz.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.blog.fehbvm.com/Article/details/gxrslosyf.sHtML

Ruby: -> { puts "run" }.call
来源：http://baike.hesvh.cn/Article/details/gafswwwwd.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://wap.zdbjq.cn/Article/details/gpasrdwpy.sHtML

[C13] 类型声明 / 类型注解
来源：http://read.share.fehbvm.com/Article/details/gmxccqaut.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://3g.hesvh.cn/Article/details/gakijqdkx.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.hesvh.cn/Article/details/gjuuacswd.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://wap.zdbjq.cn/Article/details/gbfetoitr.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.hesvh.cn/Article/details/galhyoxxx.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://wap.fehbvm.com/Article/details/gaiuvtwqh.sHtML

Go:   func add(a, b int) int
来源：http://blog.hesvh.cn/Article/details/gkubxhkdq.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://3g.fehbvm.com/Article/details/gsizuvoor.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://blog.hesvh.cn/Article/details/gcoxmbaua.sHtML

[C14] 泛型函数
来源：http://3g.fehbvm.com/Article/details/gcoorgnyr.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://3g.hesvh.cn/Article/details/gsprmmgaa.sHtML

PHP:  // 无泛型
来源：http://m.share.hesvh.cn/Article/details/gtjfrzwqa.sHtML

JS:   // 无泛型
来源：http://www.blog.hesvh.cn/Article/details/gppnqbniy.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.share.zdbjq.cn/Article/details/gtfixlqyl.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://m.share.fehbvm.com/Article/details/gkvdmwzbv.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://3g.fehbvm.com/Article/details/ghwekudgn.sHtML

Ruby: # 无泛型
来源：http://www.blog.hesvh.cn/Article/details/gpokkctqr.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.m.share.fehbvm.com/Article/details/geucvwkhp.sHtML

[C15] 解构 / 展开参数
来源：http://m.share.fehbvm.com/Article/details/guvfvfgav.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://blog.fehbvm.com/Article/details/gxukpdoyi.sHtML

PHP:  [$a, $b] = $pair;
来源：http://m.share.zdbjq.cn/Article/details/ggazdnryg.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.m.share.hesvh.cn/Article/details/gxtdudvtt.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://read.share.hesvh.cn/Article/details/gufygmfsw.sHtML

Java: // 无解构
来源：http://baike.zdbjq.cn/Article/details/gxgtflnmk.sHtML

Go:   // 无解构
来源：http://mobile.zdbjq.cn/Article/details/gkrlmidnc.sHtML

Ruby: a, b = pair
来源：http://mobile.hesvh.cn/Article/details/gqvwrhayr.sHtML

C#:   var (a, b) = pair;
来源：http://www.blog.fehbvm.com/Article/details/gbzkcryxc.sHtML

[C16] 函数 / 方法重载
来源：http://blog.hesvh.cn/Article/details/gptxadiql.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://blog.fehbvm.com/Article/details/godioenss.sHtML

PHP:  // 无重载
来源：http://read.share.zdbjq.cn/Article/details/gzzlpsbcr.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.blog.hesvh.cn/Article/details/gpqnlcljo.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://baike.zdbjq.cn/Article/details/ggnjoinmq.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://wap.fehbvm.com/Article/details/gjexfduug.sHtML

Go:   // 无重载：用不同函数名
来源：http://blog.zdbjq.cn/Article/details/gedkgrdse.sHtML

Ruby: # 无重载：靠动态参数
来源：http://3g.hesvh.cn/Article/details/grbvtgudd.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://blog.fehbvm.com/Article/details/ggukmxzib.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/giunhhfyr.sHtML

D. 数组 / 列表 / 集合
来源：http://m.share.fehbvm.com/Article/details/gmkhwufov.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gjqawatex.sHtML

[D01] 创建数组 / 列表
来源：http://www.m.share.zdbjq.cn/Article/details/ggtkbekek.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://baike.hesvh.cn/Article/details/gszahovdj.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://read.share.hesvh.cn/Article/details/gzmcsqzzm.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://mobile.zdbjq.cn/Article/details/gkxsfeley.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://blog.hesvh.cn/Article/details/gjrcmhsox.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://blog.zdbjq.cn/Article/details/gzcbvmlzo.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.blog.zdbjq.cn/Article/details/gugbootja.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.m.share.hesvh.cn/Article/details/gdanqnkpw.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.m.share.hesvh.cn/Article/details/gnckmzjbi.sHtML

[D02] 追加元素到末尾
来源：http://read.share.hesvh.cn/Article/details/gxbcddpnb.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://baike.zdbjq.cn/Article/details/gbpngmmcn.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.m.share.zdbjq.cn/Article/details/gjqpjjewh.sHtML

JS:   arr.push(4);
来源：http://wap.hesvh.cn/Article/details/geebekpvu.sHtML

TS:   arr.push(4);
来源：http://www.blog.fehbvm.com/Article/details/gxyfttwhg.sHtML

Java: list.add(4);
来源：http://wap.fehbvm.com/Article/details/gcgkrjeta.sHtML

Go:   arr = append(arr, 4)
来源：http://www.m.share.zdbjq.cn/Article/details/gvvwwitsj.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.share.hesvh.cn/Article/details/gdsqddjwe.sHtML

C#:   list.Add(4);
来源：http://3g.zdbjq.cn/Article/details/gxktgaeyn.sHtML

[D03] 在指定位置插入元素
来源：http://3g.zdbjq.cn/Article/details/gnpblmevd.sHtML

Py:   arr.insert(0, 0)
来源：http://www.share.zdbjq.cn/Article/details/gdthsivbv.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://m.share.hesvh.cn/Article/details/gegkfqcht.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.blog.hesvh.cn/Article/details/gtwbbpzmh.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://blog.zdbjq.cn/Article/details/gmvyprjvs.sHtML

Java: list.add(0, 0);
来源：http://www.share.hesvh.cn/Article/details/gnhxpueyb.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://m.share.hesvh.cn/Article/details/gpilpnuyp.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://baike.fehbvm.com/Article/details/gjgwdmfqk.sHtML

C#:   list.Insert(0, 0);
来源：http://www.blog.fehbvm.com/Article/details/gczrxxovx.sHtML

[D04] 删除元素
来源：http://www.m.share.zdbjq.cn/Article/details/gikvbeyjo.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://3g.hesvh.cn/Article/details/gdnnglqeu.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.share.fehbvm.com/Article/details/glymwifwe.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://read.share.hesvh.cn/Article/details/gxtdlqpxd.sHtML

TS:   arr.splice(0, 1);
来源：http://www.blog.fehbvm.com/Article/details/grwkwypfk.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.share.zdbjq.cn/Article/details/ggrflikcn.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mobile.fehbvm.com/Article/details/gwclgxqew.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mobile.hesvh.cn/Article/details/gyziaovuw.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://mobile.hesvh.cn/Article/details/gedqrairl.sHtML

[D05] 访问与修改元素
来源：http://m.share.fehbvm.com/Article/details/gbbqevfjv.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.hesvh.cn/Article/details/gfvxovfvn.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://baike.fehbvm.com/Article/details/gztaqcqtz.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://m.share.fehbvm.com/Article/details/gbuwhrano.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://blog.zdbjq.cn/Article/details/gpqsvnprs.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.m.share.fehbvm.com/Article/details/golgcodzs.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://wap.hesvh.cn/Article/details/gjkwvsiyx.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.zdbjq.cn/Article/details/gnpsfxvwm.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mobile.fehbvm.com/Article/details/gqkdkngyd.sHtML

[D06] 数组长度
来源：http://m.share.fehbvm.com/Article/details/gnpepywdz.sHtML

Py:   len(arr)
来源：http://www.blog.hesvh.cn/Article/details/gngpuhgjj.sHtML

PHP:  count($arr);
来源：http://blog.zdbjq.cn/Article/details/grpdgtclq.sHtML

JS:   arr.length
来源：http://3g.fehbvm.com/Article/details/gwkxtmahd.sHtML

TS:   arr.length
来源：http://m.share.hesvh.cn/Article/details/gefdupami.sHtML


<!-- 参考信息 -->