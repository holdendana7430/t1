代发 wailian999

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://blog.fanxiaobao.xyz/Article/details/gwajkqhjz.sHtML

[B06] 遍历字典 / 对象
来源：http://www.blog.fanxiaobao.xyz/Article/details/gteuisonz.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://baike.fanxiaobao.xyz/Article/details/gkpfkfgfu.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gxwmgkytt.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wap.fanxiaobao.xyz/Article/details/glgmahnpq.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.share.fanxiaobao.xyz/Article/details/gscixofpd.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwzzcouis.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://mobile.fanxiaobao.xyz/Article/details/gguyykzcz.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.blog.fanxiaobao.xyz/Article/details/grjnbmttw.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://3g.fanxiaobao.xyz/Article/details/gvzgoddpt.sHtML

[B07] while 循环
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gocjmdtld.sHtML

Py:   while i < 10: i += 1
来源：http://read.share.fanxiaobao.xyz/Article/details/grqpxwthz.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gkaxhdvmd.sHtML

JS:   while (i < 10) { i++; }
来源：http://baike.fanxiaobao.xyz/Article/details/gwdkghilr.sHtML

TS:   while (i < 10) { i++; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gtbztjvtf.sHtML

Java: while (i < 10) { i++; }
来源：http://m.share.fanxiaobao.xyz/Article/details/glpnqxzov.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://read.share.fanxiaobao.xyz/Article/details/gojbymxyy.sHtML

Ruby: while i < 10; i += 1; end
来源：http://mobile.fanxiaobao.xyz/Article/details/gjqcmqqzd.sHtML

C#:   while (i < 10) { i++; }
来源：http://3g.fanxiaobao.xyz/Article/details/gmmwjdmjx.sHtML

[B08] do-while（至少执行一次）
来源：http://blog.fanxiaobao.xyz/Article/details/guluhwlpj.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.blog.fanxiaobao.xyz/Article/details/guecbpxse.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://m.share.fanxiaobao.xyz/Article/details/gvgxdcase.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.share.fanxiaobao.xyz/Article/details/glpjiqjhc.sHtML

TS:   do { i++; } while (i < 10);
来源：http://read.share.fanxiaobao.xyz/Article/details/gpitlbuyh.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.share.fanxiaobao.xyz/Article/details/gxfodpncr.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://3g.fanxiaobao.xyz/Article/details/gbgwbprim.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://baike.fanxiaobao.xyz/Article/details/gguyjubea.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gokxekybw.sHtML

[B09] break 与 continue
来源：http://www.share.fanxiaobao.xyz/Article/details/gdlflpnwa.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://baike.fanxiaobao.xyz/Article/details/gleqwubgn.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://read.share.fanxiaobao.xyz/Article/details/giapvlhcj.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.fanxiaobao.xyz/Article/details/geoamghek.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gbbnsoojz.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.fanxiaobao.xyz/Article/details/goovpsuob.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gezpbxsor.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://read.share.fanxiaobao.xyz/Article/details/gnrvtfgzh.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.fanxiaobao.xyz/Article/details/gvcrydgtu.sHtML

[B10] 遍历同时拿索引
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpdwbuzaw.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxxdeawfn.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gwmntanqm.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grmdmyaqr.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://wap.fanxiaobao.xyz/Article/details/gflzjsvck.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://wap.fanxiaobao.xyz/Article/details/gotuodafl.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://m.share.fanxiaobao.xyz/Article/details/glipyeyjs.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxdwvasbd.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gvbwvnjey.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzlgzcozh.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.share.fanxiaobao.xyz/Article/details/gbzczozex.sHtML

PHP:  range(0, 10, 2);
来源：http://3g.fanxiaobao.xyz/Article/details/grrqttaqb.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://baike.fanxiaobao.xyz/Article/details/ggkovlwoi.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.fanxiaobao.xyz/Article/details/gwncevtqi.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://baike.fanxiaobao.xyz/Article/details/gahefmvwe.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grcooqdac.sHtML

Ruby: (0...10).step(2).to_a
来源：http://wap.fanxiaobao.xyz/Article/details/gkbyvlbcs.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://mobile.fanxiaobao.xyz/Article/details/gzcegejnp.sHtML

[B12] 跳出多层循环
来源：http://baike.fanxiaobao.xyz/Article/details/gfustxcoh.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://mobile.fanxiaobao.xyz/Article/details/gzqgbmvtz.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://baike.fanxiaobao.xyz/Article/details/gvktgxytd.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://mobile.fanxiaobao.xyz/Article/details/gbgozybqb.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geqrvqxar.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://wap.fanxiaobao.xyz/Article/details/gwhmalpmo.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gtmybowzx.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://m.share.fanxiaobao.xyz/Article/details/gruyduoig.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://mobile.fanxiaobao.xyz/Article/details/gnmwoogbe.sHtML

[B13] 判断是否为数字
来源：http://baike.fanxiaobao.xyz/Article/details/gglktecgl.sHtML

Py:   isinstance(x, (int, float))
来源：http://read.share.fanxiaobao.xyz/Article/details/gmsruqwhk.sHtML

PHP:  is_numeric($x)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gulanajnk.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.fanxiaobao.xyz/Article/details/gbxbvyqhh.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.fanxiaobao.xyz/Article/details/gyuvntpgf.sHtML

Java: x instanceof Number
来源：http://wap.fanxiaobao.xyz/Article/details/gklovxltz.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geafhokzt.sHtML

Ruby: x.is_a?(Numeric)
来源：http://m.share.fanxiaobao.xyz/Article/details/gzkqwbahf.sHtML

C#:   x is int or double or decimal
来源：http://baike.fanxiaobao.xyz/Article/details/gyngnijzj.sHtML

[B14] 判断值是否在集合内
来源：http://m.share.fanxiaobao.xyz/Article/details/gcthldesw.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://mobile.fanxiaobao.xyz/Article/details/gggmeqeqf.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gspyuybjf.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://m.share.fanxiaobao.xyz/Article/details/gfookfvzj.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtfldfjqa.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://baike.fanxiaobao.xyz/Article/details/gdxqqoonv.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvjmnkuzv.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://3g.fanxiaobao.xyz/Article/details/geeljjine.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://mobile.fanxiaobao.xyz/Article/details/gozaukrli.sHtML

[B15] 布尔运算与取反
来源：http://www.share.fanxiaobao.xyz/Article/details/gevrzzecc.sHtML

Py:   a and b or not c
来源：http://baike.fanxiaobao.xyz/Article/details/gzusiuget.sHtML

PHP:  $a && $b || !$c
来源：http://read.share.fanxiaobao.xyz/Article/details/gocnbohrr.sHtML

JS:   a && b || !c
来源：http://mobile.fanxiaobao.xyz/Article/details/ggimbdqef.sHtML

TS:   a && b || !c
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjhwkdtna.sHtML

Java: a && b || !c
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goxivplhf.sHtML

Go:   a && b || !c
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghefchhxz.sHtML

Ruby: a && b || !c
来源：http://www.blog.fanxiaobao.xyz/Article/details/gprxbxdzi.sHtML

C#:   a && b || !c
来源：http://wap.fanxiaobao.xyz/Article/details/gpxgucsey.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://wap.fanxiaobao.xyz/Article/details/giwsstkjt.sHtML

Py:   if not data: return
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpfcgdtds.sHtML

PHP:  if (!$data) { return; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnxjgotly.sHtML

JS:   if (!data) return;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggwdxwvfd.sHtML

TS:   if (!data) return;
来源：http://blog.fanxiaobao.xyz/Article/details/gyzoflenk.sHtML

Java: if (data == null) return;
来源：http://3g.fanxiaobao.xyz/Article/details/gzxkzjzef.sHtML

Go:   if data == nil { return }
来源：http://m.share.fanxiaobao.xyz/Article/details/gqjzvygam.sHtML

Ruby: return if data.nil?
来源：http://wap.fanxiaobao.xyz/Article/details/gedeahhpn.sHtML

C#:   if (data == null) return;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gemcufzkg.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/grdbfekdy.sHtML

C. 函数与作用域
来源：http://www.share.fanxiaobao.xyz/Article/details/gszyrwbks.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gfpraxftl.sHtML

[C01] 定义函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gasjiclbs.sHtML

Py:   def add(a, b): return a + b
来源：http://www.share.fanxiaobao.xyz/Article/details/gslzpfljd.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbpzsalie.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmrcgirjm.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.fanxiaobao.xyz/Article/details/gyxfmhnjz.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://baike.fanxiaobao.xyz/Article/details/gkquqowti.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.share.fanxiaobao.xyz/Article/details/grfmkaqlm.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ganmczpwd.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://mobile.fanxiaobao.xyz/Article/details/guezqvlcv.sHtML

[C02] 默认参数
来源：http://blog.fanxiaobao.xyz/Article/details/gllqgqtwu.sHtML

Py:   def greet(name="World"): return name
来源：http://3g.fanxiaobao.xyz/Article/details/gtvdrywnj.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfpzxogss.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gpblekuqy.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://wap.fanxiaobao.xyz/Article/details/gtqzhhhph.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://blog.fanxiaobao.xyz/Article/details/gxcqgxqmt.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://baike.fanxiaobao.xyz/Article/details/gaoipaftd.sHtML

Ruby: def greet(name = "World") = name
来源：http://m.share.fanxiaobao.xyz/Article/details/gqjkhrgum.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://blog.fanxiaobao.xyz/Article/details/gmajeuftt.sHtML

[C03] 可变参数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjyuucszt.sHtML

Py:   def total(*args): return sum(args)
来源：http://read.share.fanxiaobao.xyz/Article/details/gwmdkykml.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://blog.fanxiaobao.xyz/Article/details/gvgrdtjqt.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.fanxiaobao.xyz/Article/details/glrcezdrr.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.fanxiaobao.xyz/Article/details/gwzzrmlad.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gvzgzexue.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gasismvop.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqrmwrqrj.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://read.share.fanxiaobao.xyz/Article/details/gkzfvkmjb.sHtML

[C04] 命名参数 / 关键字参数
来源：http://baike.fanxiaobao.xyz/Article/details/guxdxlyta.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gflvmjnrx.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://m.share.fanxiaobao.xyz/Article/details/gdhmdttpg.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://wap.fanxiaobao.xyz/Article/details/glvpohkkg.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wap.fanxiaobao.xyz/Article/details/gqnofaomm.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://wap.fanxiaobao.xyz/Article/details/gfxdtvooc.sHtML

Go:   // 无：用配置结构体参数
来源：http://wap.fanxiaobao.xyz/Article/details/gavsxrfwp.sHtML

Ruby: f(a: 1, b: 2)
来源：http://mobile.fanxiaobao.xyz/Article/details/gcsyobvhh.sHtML

C#:   f(a: 1, b: 2)
来源：http://3g.fanxiaobao.xyz/Article/details/gymviwfsh.sHtML

[C05] 返回多个值
来源：http://3g.fanxiaobao.xyz/Article/details/gccuwnozj.sHtML

Py:   return a, b
来源：http://m.share.fanxiaobao.xyz/Article/details/gidmbprms.sHtML

PHP:  return [$a, $b];
来源：http://m.share.fanxiaobao.xyz/Article/details/gqizxwumg.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://read.share.fanxiaobao.xyz/Article/details/ghhaxbfru.sHtML

TS:   return { a, b };
来源：http://wap.fanxiaobao.xyz/Article/details/goahvauvb.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://blog.fanxiaobao.xyz/Article/details/gkosbsrmz.sHtML

Go:   return a, b
来源：http://read.share.fanxiaobao.xyz/Article/details/gvehewaqv.sHtML

Ruby: return a, b
来源：http://mobile.fanxiaobao.xyz/Article/details/gjoiulegg.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://mobile.fanxiaobao.xyz/Article/details/gbadbgjff.sHtML

[C06] 匿名函数 / lambda
来源：http://m.share.fanxiaobao.xyz/Article/details/ggaozamja.sHtML

Py:   square = lambda x: x * x
来源：http://3g.fanxiaobao.xyz/Article/details/gumnkugwh.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghlygahhi.sHtML

JS:   const square = x => x * x;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goczhekgm.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.share.fanxiaobao.xyz/Article/details/gnqmasjuw.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://mobile.fanxiaobao.xyz/Article/details/gldannjjq.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.share.fanxiaobao.xyz/Article/details/gnjhxmesd.sHtML

Ruby: square = ->(x) { x * x }
来源：http://baike.fanxiaobao.xyz/Article/details/gccphoewt.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://read.share.fanxiaobao.xyz/Article/details/gmmnxyaes.sHtML

[C07] 把函数作为参数传入
来源：http://www.blog.fanxiaobao.xyz/Article/details/gquchnpnv.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmgshfppv.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://wap.fanxiaobao.xyz/Article/details/gzcwwkqrh.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://blog.fanxiaobao.xyz/Article/details/gpwjycsjs.sHtML

TS:   arr.map(String)
来源：http://m.share.fanxiaobao.xyz/Article/details/gkveywlrc.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://mobile.fanxiaobao.xyz/Article/details/ghwydmipm.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjudrqwxu.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glxxxwffo.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://wap.fanxiaobao.xyz/Article/details/gtzzdwrcl.sHtML

[C08] 闭包
来源：http://baike.fanxiaobao.xyz/Article/details/gjzlromoi.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://blog.fanxiaobao.xyz/Article/details/gizlmqzhs.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gmipgkrxw.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://m.share.fanxiaobao.xyz/Article/details/guycmggvi.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://baike.fanxiaobao.xyz/Article/details/grtxbwmds.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://baike.fanxiaobao.xyz/Article/details/gxqbvgowd.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtlotxtug.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwiqxuyxt.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gjtfkphzr.sHtML

[C09] 递归
来源：http://read.share.fanxiaobao.xyz/Article/details/gcfeaidit.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://mobile.fanxiaobao.xyz/Article/details/gfjbyfdjv.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gjnqigkcs.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.fanxiaobao.xyz/Article/details/gieihkfvz.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.fanxiaobao.xyz/Article/details/gdsaroafi.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://blog.fanxiaobao.xyz/Article/details/geiljbpia.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wap.fanxiaobao.xyz/Article/details/gtgxbcbtm.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://blog.fanxiaobao.xyz/Article/details/gpgmphwgc.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://blog.fanxiaobao.xyz/Article/details/gaqvguqbe.sHtML

[C10] 变量作用域
来源：http://www.share.fanxiaobao.xyz/Article/details/gdbagulsw.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://3g.fanxiaobao.xyz/Article/details/ggojkbbtn.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://baike.fanxiaobao.xyz/Article/details/gfsencawg.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.share.fanxiaobao.xyz/Article/details/guavuwmeb.sHtML

TS:   同 JS
来源：http://baike.fanxiaobao.xyz/Article/details/gjspmmqhm.sHtML

Java: 方法内为块级作用域
来源：http://m.share.fanxiaobao.xyz/Article/details/gualevtit.sHtML

Go:   花括号块级作用域
来源：http://m.share.fanxiaobao.xyz/Article/details/gxvjzwyew.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.share.fanxiaobao.xyz/Article/details/gzphjadxf.sHtML

C#:   块级作用域
来源：http://baike.fanxiaobao.xyz/Article/details/gwcpatlsg.sHtML

[C11] 模块导入与导出
来源：http://3g.fanxiaobao.xyz/Article/details/gwmbalwgm.sHtML

Py:   from module import func
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnzwosfxb.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzpdffsmo.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://blog.fanxiaobao.xyz/Article/details/gmicpzahr.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://baike.fanxiaobao.xyz/Article/details/gbdunaugf.sHtML

Java: import java.util.List;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnclgyokg.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://baike.fanxiaobao.xyz/Article/details/gkbryxauo.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://3g.fanxiaobao.xyz/Article/details/ghaniqomw.sHtML

C#:   using System.Text;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guwxdrsix.sHtML

[C12] 立即执行函数 IIFE
来源：http://blog.fanxiaobao.xyz/Article/details/gmleytdcq.sHtML

Py:   (lambda: print("run"))()
来源：http://mobile.fanxiaobao.xyz/Article/details/gxpphkmiu.sHtML

PHP:  (function () { echo "run"; })();
来源：http://wap.fanxiaobao.xyz/Article/details/geqershsq.sHtML

JS:   (() => { console.log("run"); })();
来源：http://3g.fanxiaobao.xyz/Article/details/gvuqdprhn.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.share.fanxiaobao.xyz/Article/details/gskhyjxdk.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://3g.fanxiaobao.xyz/Article/details/giwdhlgck.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://mobile.fanxiaobao.xyz/Article/details/gzydonsdm.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glrynimgz.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxyjgfgag.sHtML

[C13] 类型声明 / 类型注解
来源：http://blog.fanxiaobao.xyz/Article/details/gmvvxfqsc.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.share.fanxiaobao.xyz/Article/details/gfpptizgj.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gumjaorto.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://read.share.fanxiaobao.xyz/Article/details/gjlgxdyaj.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.fanxiaobao.xyz/Article/details/gwwmhgoyg.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://3g.fanxiaobao.xyz/Article/details/gwdyfdvlb.sHtML

Go:   func add(a, b int) int
来源：http://read.share.fanxiaobao.xyz/Article/details/gyaedblyl.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://baike.fanxiaobao.xyz/Article/details/gtsfdjcbe.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/golwpmiqd.sHtML

[C14] 泛型函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gnvpuzrvy.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://baike.fanxiaobao.xyz/Article/details/ggynbdven.sHtML

PHP:  // 无泛型
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gavipxwlk.sHtML

JS:   // 无泛型
来源：http://www.share.fanxiaobao.xyz/Article/details/gbvlviceu.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gmpjlrmwz.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://mobile.fanxiaobao.xyz/Article/details/grpgoktng.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyzrduiun.sHtML

Ruby: # 无泛型
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goysyvpov.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://m.share.fanxiaobao.xyz/Article/details/gniupklqm.sHtML

[C15] 解构 / 展开参数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpwsitxgv.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcykyuzvn.sHtML

PHP:  [$a, $b] = $pair;
来源：http://m.share.fanxiaobao.xyz/Article/details/gluapnvli.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://blog.fanxiaobao.xyz/Article/details/gwsxvbffz.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gytzgrtie.sHtML

Java: // 无解构
来源：http://wap.fanxiaobao.xyz/Article/details/gygjboput.sHtML

Go:   // 无解构
来源：http://blog.fanxiaobao.xyz/Article/details/gdiqsehwe.sHtML

Ruby: a, b = pair
来源：http://blog.fanxiaobao.xyz/Article/details/gmahkfqoc.sHtML

C#:   var (a, b) = pair;
来源：http://3g.fanxiaobao.xyz/Article/details/gwrkxiwqp.sHtML

[C16] 函数 / 方法重载
来源：http://read.share.fanxiaobao.xyz/Article/details/gesqqaacl.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://3g.fanxiaobao.xyz/Article/details/gqtbjxjkw.sHtML

PHP:  // 无重载
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gururvqcq.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.share.fanxiaobao.xyz/Article/details/gqmyrjggx.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://read.share.fanxiaobao.xyz/Article/details/gtnrxampf.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.share.fanxiaobao.xyz/Article/details/giyhvhzfi.sHtML

Go:   // 无重载：用不同函数名
来源：http://blog.fanxiaobao.xyz/Article/details/gqunsrnbe.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gylopzgac.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://wap.fanxiaobao.xyz/Article/details/gzcwisiaj.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gulfxzseh.sHtML

D. 数组 / 列表 / 集合
来源：http://mobile.fanxiaobao.xyz/Article/details/ggubpsial.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gajvrevha.sHtML

[D01] 创建数组 / 列表
来源：http://www.blog.fanxiaobao.xyz/Article/details/gidihokyr.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://m.share.fanxiaobao.xyz/Article/details/gjpjotczo.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://m.share.fanxiaobao.xyz/Article/details/gsfzqhzgt.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://3g.fanxiaobao.xyz/Article/details/gmicjpvju.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://read.share.fanxiaobao.xyz/Article/details/gqzovbamz.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtfhrcdcf.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnaxtgmgh.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqlithcst.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://blog.fanxiaobao.xyz/Article/details/gbyqgnmiv.sHtML

[D02] 追加元素到末尾
来源：http://read.share.fanxiaobao.xyz/Article/details/gsojbsvlz.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://m.share.fanxiaobao.xyz/Article/details/gebmicnmk.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://baike.fanxiaobao.xyz/Article/details/gvtmwncsl.sHtML

JS:   arr.push(4);
来源：http://wap.fanxiaobao.xyz/Article/details/gbfnvgdhj.sHtML

TS:   arr.push(4);
来源：http://www.share.fanxiaobao.xyz/Article/details/gxoiduczw.sHtML

Java: list.add(4);
来源：http://m.share.fanxiaobao.xyz/Article/details/gjajeytbw.sHtML

Go:   arr = append(arr, 4)
来源：http://m.share.fanxiaobao.xyz/Article/details/gfepnjocf.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://m.share.fanxiaobao.xyz/Article/details/gaunrshvf.sHtML

C#:   list.Add(4);
来源：http://3g.fanxiaobao.xyz/Article/details/gertqsrrq.sHtML

[D03] 在指定位置插入元素
来源：http://blog.fanxiaobao.xyz/Article/details/gbothzqes.sHtML

Py:   arr.insert(0, 0)
来源：http://3g.fanxiaobao.xyz/Article/details/ghqkzowty.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://read.share.fanxiaobao.xyz/Article/details/gflfvzdbg.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://blog.fanxiaobao.xyz/Article/details/ghpvquyyn.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://3g.fanxiaobao.xyz/Article/details/gfknevfce.sHtML

Java: list.add(0, 0);
来源：http://wap.fanxiaobao.xyz/Article/details/gcaxzppnn.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://baike.fanxiaobao.xyz/Article/details/ghgffxnog.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.share.fanxiaobao.xyz/Article/details/gtofgbcud.sHtML

C#:   list.Insert(0, 0);
来源：http://www.share.fanxiaobao.xyz/Article/details/gixeiqrhj.sHtML

[D04] 删除元素
来源：http://mobile.fanxiaobao.xyz/Article/details/gpptnconj.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wap.fanxiaobao.xyz/Article/details/gnsrpnubf.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://baike.fanxiaobao.xyz/Article/details/gcfmfciij.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.share.fanxiaobao.xyz/Article/details/gnfzqbduk.sHtML

TS:   arr.splice(0, 1);
来源：http://m.share.fanxiaobao.xyz/Article/details/gwjbhhzam.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://blog.fanxiaobao.xyz/Article/details/geqdnfqnn.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://read.share.fanxiaobao.xyz/Article/details/gsyynaujw.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.share.fanxiaobao.xyz/Article/details/gdvgalcrk.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.share.fanxiaobao.xyz/Article/details/guvlesuak.sHtML

[D05] 访问与修改元素
来源：http://baike.fanxiaobao.xyz/Article/details/glytuctka.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.fanxiaobao.xyz/Article/details/gdwlavrgc.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://m.share.fanxiaobao.xyz/Article/details/gconerbdn.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grmfgcqto.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://mobile.fanxiaobao.xyz/Article/details/gjjhrxcfp.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://baike.fanxiaobao.xyz/Article/details/gutemuzgk.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://mobile.fanxiaobao.xyz/Article/details/ghospeyrh.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.fanxiaobao.xyz/Article/details/grxsfprby.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://3g.fanxiaobao.xyz/Article/details/gyounveaj.sHtML

[D06] 数组长度
来源：http://www.share.fanxiaobao.xyz/Article/details/gauzwoyuo.sHtML

Py:   len(arr)
来源：http://www.share.fanxiaobao.xyz/Article/details/gdldybjoy.sHtML

PHP:  count($arr);
来源：http://wap.fanxiaobao.xyz/Article/details/gyoylnwfr.sHtML

JS:   arr.length
来源：http://www.share.fanxiaobao.xyz/Article/details/gvthantdi.sHtML

TS:   arr.length
来源：http://m.share.fanxiaobao.xyz/Article/details/gmliqbrtv.sHtML


<!-- 参考信息 -->