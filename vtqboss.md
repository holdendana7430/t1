代发 wailian999

[B05] 遍历数组 / 列表
来源：http://read.share.fanxiaobao.xyz/Article/details/gqlnawrww.sHtML

Py:   for item in arr: print(item)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gviddpmvz.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://blog.fanxiaobao.xyz/Article/details/gbwmfcxbc.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gggntpoqo.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://wap.fanxiaobao.xyz/Article/details/guwezasff.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://mobile.fanxiaobao.xyz/Article/details/gxmrxmgfq.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://wap.fanxiaobao.xyz/Article/details/gpsxasmpe.sHtML

Ruby: arr.each { |item| puts item }
来源：http://read.share.fanxiaobao.xyz/Article/details/gdelptkmh.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://mobile.fanxiaobao.xyz/Article/details/gralmuwjb.sHtML

[B06] 遍历字典 / 对象
来源：http://blog.fanxiaobao.xyz/Article/details/gvfttrluf.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.share.fanxiaobao.xyz/Article/details/gcvdpugoe.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://baike.fanxiaobao.xyz/Article/details/gtagsqqvo.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpmkvyfod.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://blog.fanxiaobao.xyz/Article/details/gwonvpmgg.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyycbehrf.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://blog.fanxiaobao.xyz/Article/details/gxcwxircq.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxcilzscg.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.share.fanxiaobao.xyz/Article/details/grhxybsgg.sHtML

[B07] while 循环
来源：http://wap.fanxiaobao.xyz/Article/details/gsbhcbrqb.sHtML

Py:   while i < 10: i += 1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gflvrmijn.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnhzscmta.sHtML

JS:   while (i < 10) { i++; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gvvolincf.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gkheicufb.sHtML

Java: while (i < 10) { i++; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gljwtmeqn.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://blog.fanxiaobao.xyz/Article/details/gwquogffp.sHtML

Ruby: while i < 10; i += 1; end
来源：http://blog.fanxiaobao.xyz/Article/details/gfslwrnco.sHtML

C#:   while (i < 10) { i++; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gvbesbxzw.sHtML

[B08] do-while（至少执行一次）
来源：http://www.share.fanxiaobao.xyz/Article/details/gtsmplfzk.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.share.fanxiaobao.xyz/Article/details/goquntced.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggovrrboj.sHtML

JS:   do { i++; } while (i < 10);
来源：http://m.share.fanxiaobao.xyz/Article/details/gcsmnukuo.sHtML

TS:   do { i++; } while (i < 10);
来源：http://m.share.fanxiaobao.xyz/Article/details/guaogbach.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gipyfgqdq.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://m.share.fanxiaobao.xyz/Article/details/getlxfxni.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://wap.fanxiaobao.xyz/Article/details/ggumwfpqg.sHtML

C#:   do { i++; } while (i < 10);
来源：http://mobile.fanxiaobao.xyz/Article/details/gzmklorcv.sHtML

[B09] break 与 continue
来源：http://3g.fanxiaobao.xyz/Article/details/gmxncppks.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://3g.fanxiaobao.xyz/Article/details/goqhaomts.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://3g.fanxiaobao.xyz/Article/details/gyscfitll.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gaowjgyet.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.fanxiaobao.xyz/Article/details/ghjstcflt.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.fanxiaobao.xyz/Article/details/ggcmgmbmx.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://mobile.fanxiaobao.xyz/Article/details/guhcqubwt.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://baike.fanxiaobao.xyz/Article/details/gtmnwjgfk.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gehadnqye.sHtML

[B10] 遍历同时拿索引
来源：http://www.blog.fanxiaobao.xyz/Article/details/gghflzwiv.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://m.share.fanxiaobao.xyz/Article/details/ghygsjsuh.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/guqfkgwas.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://wap.fanxiaobao.xyz/Article/details/gwfxvtbgn.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://wap.fanxiaobao.xyz/Article/details/gioxggtcr.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.share.fanxiaobao.xyz/Article/details/gtjkgmike.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://mobile.fanxiaobao.xyz/Article/details/ghmaegwau.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://mobile.fanxiaobao.xyz/Article/details/grvjciwed.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://3g.fanxiaobao.xyz/Article/details/gwzkazbqv.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfjgipjbm.sHtML

Py:   list(range(0, 10, 2))
来源：http://baike.fanxiaobao.xyz/Article/details/gktutuhmo.sHtML

PHP:  range(0, 10, 2);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtmhmxsnl.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gybtqxhgy.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyoubkqcr.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://mobile.fanxiaobao.xyz/Article/details/gdhygaofa.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghtovnkdg.sHtML

Ruby: (0...10).step(2).to_a
来源：http://blog.fanxiaobao.xyz/Article/details/gjgeipvfj.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://read.share.fanxiaobao.xyz/Article/details/gaemgqizi.sHtML

[B12] 跳出多层循环
来源：http://blog.fanxiaobao.xyz/Article/details/grmsfszdn.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://mobile.fanxiaobao.xyz/Article/details/ghvvqsboh.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://mobile.fanxiaobao.xyz/Article/details/gtjmnhudo.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://baike.fanxiaobao.xyz/Article/details/gdwvvefqk.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gycframaw.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.share.fanxiaobao.xyz/Article/details/gkbmfrshn.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://m.share.fanxiaobao.xyz/Article/details/guukwktdy.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://m.share.fanxiaobao.xyz/Article/details/glgtzwtra.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.share.fanxiaobao.xyz/Article/details/gizzaljqo.sHtML

[B13] 判断是否为数字
来源：http://www.share.fanxiaobao.xyz/Article/details/gcajectoo.sHtML

Py:   isinstance(x, (int, float))
来源：http://blog.fanxiaobao.xyz/Article/details/ggbbdhorr.sHtML

PHP:  is_numeric($x)
来源：http://wap.fanxiaobao.xyz/Article/details/gjicevjxj.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://3g.fanxiaobao.xyz/Article/details/gvkpnliqd.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://3g.fanxiaobao.xyz/Article/details/gqycvpkez.sHtML

Java: x instanceof Number
来源：http://blog.fanxiaobao.xyz/Article/details/gusqldefm.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://read.share.fanxiaobao.xyz/Article/details/glarpmlgu.sHtML

Ruby: x.is_a?(Numeric)
来源：http://blog.fanxiaobao.xyz/Article/details/goxkhkihn.sHtML

C#:   x is int or double or decimal
来源：http://m.share.fanxiaobao.xyz/Article/details/gvhtojkgx.sHtML

[B14] 判断值是否在集合内
来源：http://blog.fanxiaobao.xyz/Article/details/gdaiscwhz.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpyokrmdf.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://mobile.fanxiaobao.xyz/Article/details/gpwvwccmq.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://m.share.fanxiaobao.xyz/Article/details/gqwfsqqnt.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://3g.fanxiaobao.xyz/Article/details/gbvzgaxfq.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.share.fanxiaobao.xyz/Article/details/gsnhaxvbb.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://baike.fanxiaobao.xyz/Article/details/gbldbkyld.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://baike.fanxiaobao.xyz/Article/details/gqhriafih.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.share.fanxiaobao.xyz/Article/details/gkcngpbfk.sHtML

[B15] 布尔运算与取反
来源：http://baike.fanxiaobao.xyz/Article/details/gltgpsdng.sHtML

Py:   a and b or not c
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkjnuwlkw.sHtML

PHP:  $a && $b || !$c
来源：http://mobile.fanxiaobao.xyz/Article/details/goimtpfeg.sHtML

JS:   a && b || !c
来源：http://baike.fanxiaobao.xyz/Article/details/gtfzsihxd.sHtML

TS:   a && b || !c
来源：http://mobile.fanxiaobao.xyz/Article/details/gyrapiqmk.sHtML

Java: a && b || !c
来源：http://3g.fanxiaobao.xyz/Article/details/gtejgdqwu.sHtML

Go:   a && b || !c
来源：http://mobile.fanxiaobao.xyz/Article/details/gbdohiihk.sHtML

Ruby: a && b || !c
来源：http://wap.fanxiaobao.xyz/Article/details/gjhfluynj.sHtML

C#:   a && b || !c
来源：http://read.share.fanxiaobao.xyz/Article/details/geggdkfny.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://blog.fanxiaobao.xyz/Article/details/gtvftuwdr.sHtML

Py:   if not data: return
来源：http://www.share.fanxiaobao.xyz/Article/details/ghnjekycz.sHtML

PHP:  if (!$data) { return; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzissmfru.sHtML

JS:   if (!data) return;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjftfwpre.sHtML

TS:   if (!data) return;
来源：http://blog.fanxiaobao.xyz/Article/details/gvjdxfvqd.sHtML

Java: if (data == null) return;
来源：http://baike.fanxiaobao.xyz/Article/details/gloaelamu.sHtML

Go:   if data == nil { return }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gltvnmlys.sHtML

Ruby: return if data.nil?
来源：http://baike.fanxiaobao.xyz/Article/details/gveyzfrqq.sHtML

C#:   if (data == null) return;
来源：http://m.share.fanxiaobao.xyz/Article/details/gkoqjwyoq.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpzkaceay.sHtML

C. 函数与作用域
来源：http://mobile.fanxiaobao.xyz/Article/details/gukjjlzdh.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gftycxbef.sHtML

[C01] 定义函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gmmyrybsf.sHtML

Py:   def add(a, b): return a + b
来源：http://3g.fanxiaobao.xyz/Article/details/gkvkhelmx.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.fanxiaobao.xyz/Article/details/gzzkoyehv.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gqhdmwltp.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwsctahyi.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://baike.fanxiaobao.xyz/Article/details/gpegzylbr.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://3g.fanxiaobao.xyz/Article/details/grstxlukx.sHtML

Ruby: def add(a, b); a + b; end
来源：http://baike.fanxiaobao.xyz/Article/details/guxyksqqv.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnzhnjioq.sHtML

[C02] 默认参数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmqiwsfwp.sHtML

Py:   def greet(name="World"): return name
来源：http://www.share.fanxiaobao.xyz/Article/details/gykrbelsa.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://m.share.fanxiaobao.xyz/Article/details/grdoooyqb.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gdllakzfw.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqjronhot.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://baike.fanxiaobao.xyz/Article/details/gkpuajreb.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://3g.fanxiaobao.xyz/Article/details/gpgknufiv.sHtML

Ruby: def greet(name = "World") = name
来源：http://3g.fanxiaobao.xyz/Article/details/gcgbatkyv.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvauueyli.sHtML

[C03] 可变参数
来源：http://3g.fanxiaobao.xyz/Article/details/gejxfampt.sHtML

Py:   def total(*args): return sum(args)
来源：http://mobile.fanxiaobao.xyz/Article/details/gnozvwswe.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://blog.fanxiaobao.xyz/Article/details/gbyytiyya.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.fanxiaobao.xyz/Article/details/gonzgbbxx.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtlsznyvl.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gpaugcjto.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwsvpkdfy.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://wap.fanxiaobao.xyz/Article/details/gzyjzbctc.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://m.share.fanxiaobao.xyz/Article/details/gdujpjfgp.sHtML

[C04] 命名参数 / 关键字参数
来源：http://blog.fanxiaobao.xyz/Article/details/gvgazvbgp.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://baike.fanxiaobao.xyz/Article/details/gozdhuebg.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://wap.fanxiaobao.xyz/Article/details/gnoaqhiah.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://blog.fanxiaobao.xyz/Article/details/glrbeuqiy.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://mobile.fanxiaobao.xyz/Article/details/gqauciplv.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://baike.fanxiaobao.xyz/Article/details/gqanopqwg.sHtML

Go:   // 无：用配置结构体参数
来源：http://3g.fanxiaobao.xyz/Article/details/gjrjuacrz.sHtML

Ruby: f(a: 1, b: 2)
来源：http://baike.fanxiaobao.xyz/Article/details/gyuuoanvs.sHtML

C#:   f(a: 1, b: 2)
来源：http://wap.fanxiaobao.xyz/Article/details/gwmdxyxcz.sHtML

[C05] 返回多个值
来源：http://read.share.fanxiaobao.xyz/Article/details/gzvrjtyjc.sHtML

Py:   return a, b
来源：http://m.share.fanxiaobao.xyz/Article/details/gjozahidh.sHtML

PHP:  return [$a, $b];
来源：http://m.share.fanxiaobao.xyz/Article/details/gnqqhkyqc.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://wap.fanxiaobao.xyz/Article/details/gggduoyye.sHtML

TS:   return { a, b };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjwaebmhh.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://read.share.fanxiaobao.xyz/Article/details/gbiqxgflt.sHtML

Go:   return a, b
来源：http://m.share.fanxiaobao.xyz/Article/details/gdwjpqxjf.sHtML

Ruby: return a, b
来源：http://www.blog.fanxiaobao.xyz/Article/details/gshjtcfce.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://wap.fanxiaobao.xyz/Article/details/gnfnzwenm.sHtML

[C06] 匿名函数 / lambda
来源：http://read.share.fanxiaobao.xyz/Article/details/giljmgxga.sHtML

Py:   square = lambda x: x * x
来源：http://mobile.fanxiaobao.xyz/Article/details/gsfjjnjan.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.share.fanxiaobao.xyz/Article/details/gawzuanwb.sHtML

JS:   const square = x => x * x;
来源：http://wap.fanxiaobao.xyz/Article/details/ggaiqicey.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggkmgkdhg.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://baike.fanxiaobao.xyz/Article/details/gkhzswzso.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://baike.fanxiaobao.xyz/Article/details/gzqzbhbhl.sHtML

Ruby: square = ->(x) { x * x }
来源：http://baike.fanxiaobao.xyz/Article/details/gbkerkbjk.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://blog.fanxiaobao.xyz/Article/details/gkopbhocv.sHtML

[C07] 把函数作为参数传入
来源：http://m.share.fanxiaobao.xyz/Article/details/gwegcotis.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://m.share.fanxiaobao.xyz/Article/details/guszbalfx.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.share.fanxiaobao.xyz/Article/details/gvrdlfpfw.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcijobkwj.sHtML

TS:   arr.map(String)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gatfkkelb.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmulylrsm.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.share.fanxiaobao.xyz/Article/details/gsfwandpd.sHtML

Ruby: arr.map(&:upcase)
来源：http://m.share.fanxiaobao.xyz/Article/details/gfwhnpdga.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://read.share.fanxiaobao.xyz/Article/details/gjdevbhpm.sHtML

[C08] 闭包
来源：http://wap.fanxiaobao.xyz/Article/details/gyvmuqkuw.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://m.share.fanxiaobao.xyz/Article/details/gdocqlgmb.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://3g.fanxiaobao.xyz/Article/details/gpccliaat.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcevcxgdu.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gksimwmpa.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://blog.fanxiaobao.xyz/Article/details/gihqfwjat.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://blog.fanxiaobao.xyz/Article/details/gzlhznugd.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://baike.fanxiaobao.xyz/Article/details/grgasazta.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guxsghahf.sHtML

[C09] 递归
来源：http://www.share.fanxiaobao.xyz/Article/details/geqxysdbb.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://wap.fanxiaobao.xyz/Article/details/giwzxetyq.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://wap.fanxiaobao.xyz/Article/details/gzwrewatz.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.fanxiaobao.xyz/Article/details/gtroujckm.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.fanxiaobao.xyz/Article/details/gquwtizry.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.share.fanxiaobao.xyz/Article/details/giaoedfvp.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://m.share.fanxiaobao.xyz/Article/details/gomstlatk.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyfbbusgv.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://read.share.fanxiaobao.xyz/Article/details/gzrkwpaxm.sHtML

[C10] 变量作用域
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glphhrgri.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.share.fanxiaobao.xyz/Article/details/gccdajzzc.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://baike.fanxiaobao.xyz/Article/details/gqtmjvlai.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://wap.fanxiaobao.xyz/Article/details/gryutpjoa.sHtML

TS:   同 JS
来源：http://mobile.fanxiaobao.xyz/Article/details/gwtsnbfxo.sHtML

Java: 方法内为块级作用域
来源：http://wap.fanxiaobao.xyz/Article/details/gpngnpdcy.sHtML

Go:   花括号块级作用域
来源：http://wap.fanxiaobao.xyz/Article/details/gumksebww.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://3g.fanxiaobao.xyz/Article/details/gnqpyfrir.sHtML

C#:   块级作用域
来源：http://blog.fanxiaobao.xyz/Article/details/ggopjqncv.sHtML

[C11] 模块导入与导出
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkljvkdzb.sHtML

Py:   from module import func
来源：http://read.share.fanxiaobao.xyz/Article/details/gcypfxqss.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaunnrkio.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.share.fanxiaobao.xyz/Article/details/gbeyjfgcr.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://mobile.fanxiaobao.xyz/Article/details/glwmtkzpl.sHtML

Java: import java.util.List;
来源：http://www.share.fanxiaobao.xyz/Article/details/gsvjeahgw.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://read.share.fanxiaobao.xyz/Article/details/gtidgnogw.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://mobile.fanxiaobao.xyz/Article/details/ghdgckptw.sHtML

C#:   using System.Text;
来源：http://baike.fanxiaobao.xyz/Article/details/gmjpnmrep.sHtML

[C12] 立即执行函数 IIFE
来源：http://mobile.fanxiaobao.xyz/Article/details/gcojkvalp.sHtML

Py:   (lambda: print("run"))()
来源：http://blog.fanxiaobao.xyz/Article/details/grehflkfk.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guymnjecs.sHtML

JS:   (() => { console.log("run"); })();
来源：http://blog.fanxiaobao.xyz/Article/details/gjrggfweh.sHtML

TS:   (() => { console.log("run"); })();
来源：http://blog.fanxiaobao.xyz/Article/details/gikoujvmq.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://mobile.fanxiaobao.xyz/Article/details/gtcrzljzo.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://m.share.fanxiaobao.xyz/Article/details/gtgyawzub.sHtML

Ruby: -> { puts "run" }.call
来源：http://baike.fanxiaobao.xyz/Article/details/gimntkpkt.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://blog.fanxiaobao.xyz/Article/details/gamptntji.sHtML

[C13] 类型声明 / 类型注解
来源：http://baike.fanxiaobao.xyz/Article/details/gpkkptkwh.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://read.share.fanxiaobao.xyz/Article/details/gaqtofmrr.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.fanxiaobao.xyz/Article/details/grtywcpxf.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://wap.fanxiaobao.xyz/Article/details/gzqwzmhqb.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.fanxiaobao.xyz/Article/details/gvwmlizgq.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://blog.fanxiaobao.xyz/Article/details/gvvsefaju.sHtML

Go:   func add(a, b int) int
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpovrrubo.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjnkopatw.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://mobile.fanxiaobao.xyz/Article/details/grykjidis.sHtML

[C14] 泛型函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gqagzawxg.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmfvdunng.sHtML

PHP:  // 无泛型
来源：http://www.share.fanxiaobao.xyz/Article/details/gcnyyeixr.sHtML

JS:   // 无泛型
来源：http://baike.fanxiaobao.xyz/Article/details/gwwxlwhdl.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://baike.fanxiaobao.xyz/Article/details/gvfvzdqpl.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://blog.fanxiaobao.xyz/Article/details/ghospdtmt.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqxejolks.sHtML

Ruby: # 无泛型
来源：http://m.share.fanxiaobao.xyz/Article/details/gtzpqghzz.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wap.fanxiaobao.xyz/Article/details/gqlfibnlf.sHtML

[C15] 解构 / 展开参数
来源：http://read.share.fanxiaobao.xyz/Article/details/gbxrtqloa.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://3g.fanxiaobao.xyz/Article/details/gfvhmzusv.sHtML

PHP:  [$a, $b] = $pair;
来源：http://m.share.fanxiaobao.xyz/Article/details/gqqjmwfaw.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://baike.fanxiaobao.xyz/Article/details/ghfgqejxm.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grsgdghmb.sHtML

Java: // 无解构
来源：http://wap.fanxiaobao.xyz/Article/details/gdwicoksc.sHtML

Go:   // 无解构
来源：http://mobile.fanxiaobao.xyz/Article/details/gnnkcuzae.sHtML

Ruby: a, b = pair
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtxadyyzb.sHtML

C#:   var (a, b) = pair;
来源：http://www.share.fanxiaobao.xyz/Article/details/gcstcekwv.sHtML

[C16] 函数 / 方法重载
来源：http://wap.fanxiaobao.xyz/Article/details/grrhtzsxq.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://mobile.fanxiaobao.xyz/Article/details/glaubwpjj.sHtML

PHP:  // 无重载
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gemnedsau.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://baike.fanxiaobao.xyz/Article/details/gxdxnqfrs.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://3g.fanxiaobao.xyz/Article/details/gbocemswb.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gggmxrvxk.sHtML

Go:   // 无重载：用不同函数名
来源：http://m.share.fanxiaobao.xyz/Article/details/gdzzvwuzy.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtgzfftkk.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gsrupcszi.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtwkjrkzl.sHtML

D. 数组 / 列表 / 集合
来源：http://blog.fanxiaobao.xyz/Article/details/gfdphshzb.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gdayypknq.sHtML

[D01] 创建数组 / 列表
来源：http://3g.fanxiaobao.xyz/Article/details/gegmtqery.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://mobile.fanxiaobao.xyz/Article/details/gfdeojyvf.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://m.share.fanxiaobao.xyz/Article/details/gmsdgcdss.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://blog.fanxiaobao.xyz/Article/details/gcsyzhrau.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://blog.fanxiaobao.xyz/Article/details/gvpruelqi.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://blog.fanxiaobao.xyz/Article/details/gavqyuhpm.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.share.fanxiaobao.xyz/Article/details/gtsnxmksb.sHtML

Ruby: arr = [1, 2, 3]
来源：http://wap.fanxiaobao.xyz/Article/details/gjmogjfrh.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://baike.fanxiaobao.xyz/Article/details/glfzppdry.sHtML

[D02] 追加元素到末尾
来源：http://blog.fanxiaobao.xyz/Article/details/guojvezps.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://blog.fanxiaobao.xyz/Article/details/ggiblxrgd.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://read.share.fanxiaobao.xyz/Article/details/giddtfajs.sHtML

JS:   arr.push(4);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guflhzolx.sHtML

TS:   arr.push(4);
来源：http://www.share.fanxiaobao.xyz/Article/details/grkgewvpa.sHtML

Java: list.add(4);
来源：http://mobile.fanxiaobao.xyz/Article/details/gicplbpdl.sHtML

Go:   arr = append(arr, 4)
来源：http://wap.fanxiaobao.xyz/Article/details/grlmawaku.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://wap.fanxiaobao.xyz/Article/details/gpoammawn.sHtML

C#:   list.Add(4);
来源：http://read.share.fanxiaobao.xyz/Article/details/gccojcqub.sHtML

[D03] 在指定位置插入元素
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbaioutgv.sHtML

Py:   arr.insert(0, 0)
来源：http://mobile.fanxiaobao.xyz/Article/details/gfhaevwrb.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://wap.fanxiaobao.xyz/Article/details/gtnrikgrs.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcznazxil.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://baike.fanxiaobao.xyz/Article/details/grxssugyp.sHtML

Java: list.add(0, 0);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdntcfbmy.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://mobile.fanxiaobao.xyz/Article/details/gkecydujz.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://baike.fanxiaobao.xyz/Article/details/ghiyivkaw.sHtML

C#:   list.Insert(0, 0);
来源：http://3g.fanxiaobao.xyz/Article/details/gfqlyofjo.sHtML

[D04] 删除元素
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvdicratz.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.share.fanxiaobao.xyz/Article/details/gxcuzmsmc.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.share.fanxiaobao.xyz/Article/details/glfpzbdqv.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://blog.fanxiaobao.xyz/Article/details/gomagzjaz.sHtML

TS:   arr.splice(0, 1);
来源：http://read.share.fanxiaobao.xyz/Article/details/gexklmddm.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gotcvxaan.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://blog.fanxiaobao.xyz/Article/details/gtnxnsxmq.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mobile.fanxiaobao.xyz/Article/details/gdywgzjqc.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjntndoje.sHtML

[D05] 访问与修改元素
来源：http://3g.fanxiaobao.xyz/Article/details/gcnkcnzic.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.fanxiaobao.xyz/Article/details/gwmqleycu.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.share.fanxiaobao.xyz/Article/details/gcjvcpeeq.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://baike.fanxiaobao.xyz/Article/details/gdgsvdhiq.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.share.fanxiaobao.xyz/Article/details/gsynpemoj.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://3g.fanxiaobao.xyz/Article/details/gmzgelzjw.sHtML


<!-- 参考信息 -->