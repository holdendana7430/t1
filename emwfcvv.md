代发 wailian999

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://m.share.fehbvm.com/Article/details/gqetyltkk.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://mobile.fehbvm.com/Article/details/grkmieoge.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://m.share.fehbvm.com/Article/details/gqtjikncv.sHtML

[B04] for 计数循环
来源：http://m.share.fehbvm.com/Article/details/gleefvbre.sHtML

Py:   for i in range(10): print(i)
来源：http://wap.fehbvm.com/Article/details/gcdzagoem.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.m.share.zdbjq.cn/Article/details/gzyijaako.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wap.fehbvm.com/Article/details/glafnlxcn.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://blog.hesvh.cn/Article/details/gwiskvsbw.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://wap.hesvh.cn/Article/details/gjfujiqmv.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.share.fehbvm.com/Article/details/gpblvgvct.sHtML

Ruby: 10.times { |i| puts i }
来源：http://baike.fehbvm.com/Article/details/glzlkcshh.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://baike.fehbvm.com/Article/details/ghapaiqls.sHtML

[B05] 遍历数组 / 列表
来源：http://www.share.zdbjq.cn/Article/details/gfldxuays.sHtML

Py:   for item in arr: print(item)
来源：http://blog.zdbjq.cn/Article/details/giddeyvaj.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.share.hesvh.cn/Article/details/gtewcibih.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://mobile.hesvh.cn/Article/details/grurcpwgp.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.m.share.zdbjq.cn/Article/details/ggalhthrh.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://read.share.fehbvm.com/Article/details/gydqnevsg.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://read.share.fehbvm.com/Article/details/gnyhxadyi.sHtML

Ruby: arr.each { |item| puts item }
来源：http://m.share.zdbjq.cn/Article/details/gdldvlxfi.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://wap.fehbvm.com/Article/details/ghllazjcl.sHtML

[B06] 遍历字典 / 对象
来源：http://3g.hesvh.cn/Article/details/gzkqcbfmo.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://read.share.hesvh.cn/Article/details/giqeegnra.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.blog.zdbjq.cn/Article/details/glitxbruv.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://3g.fehbvm.com/Article/details/gfolcjqlr.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://read.share.fehbvm.com/Article/details/gkfhuxcdb.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://3g.zdbjq.cn/Article/details/ggvfierix.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://wap.fehbvm.com/Article/details/grcvhkjjh.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://blog.fehbvm.com/Article/details/ggeyrtvxr.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://wap.zdbjq.cn/Article/details/ghknfqetg.sHtML

[B07] while 循环
来源：http://baike.zdbjq.cn/Article/details/goxoecoaz.sHtML

Py:   while i < 10: i += 1
来源：http://blog.zdbjq.cn/Article/details/gqjftklfc.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.blog.hesvh.cn/Article/details/gyymxbvpy.sHtML

JS:   while (i < 10) { i++; }
来源：http://3g.fehbvm.com/Article/details/ghkbljxgk.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.share.hesvh.cn/Article/details/gmchfgcqa.sHtML

Java: while (i < 10) { i++; }
来源：http://www.blog.hesvh.cn/Article/details/gufxinyiu.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.share.fehbvm.com/Article/details/gomahhhsl.sHtML

Ruby: while i < 10; i += 1; end
来源：http://baike.zdbjq.cn/Article/details/gjflivfqw.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.blog.hesvh.cn/Article/details/gjofizzud.sHtML

[B08] do-while（至少执行一次）
来源：http://blog.hesvh.cn/Article/details/ghusdlvcf.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://baike.zdbjq.cn/Article/details/gwwzbeobd.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://baike.hesvh.cn/Article/details/gnmdopeiz.sHtML

JS:   do { i++; } while (i < 10);
来源：http://wap.fehbvm.com/Article/details/gyfeqzvrm.sHtML

TS:   do { i++; } while (i < 10);
来源：http://baike.fehbvm.com/Article/details/ghvgwqilp.sHtML

Java: do { i++; } while (i < 10);
来源：http://mobile.zdbjq.cn/Article/details/gjokloaxx.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://wap.zdbjq.cn/Article/details/gpxoiqczq.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.share.fehbvm.com/Article/details/gclyxyclr.sHtML

C#:   do { i++; } while (i < 10);
来源：http://m.share.hesvh.cn/Article/details/ghwhshqgt.sHtML

[B09] break 与 continue
来源：http://www.m.share.zdbjq.cn/Article/details/gpfzmrrbn.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://blog.fehbvm.com/Article/details/gnqasvlxl.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.blog.zdbjq.cn/Article/details/gcbvqbggq.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.zdbjq.cn/Article/details/glzjyaypj.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.zdbjq.cn/Article/details/gtvrumdof.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.hesvh.cn/Article/details/ghayeasdy.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.m.share.hesvh.cn/Article/details/ghucbtrfh.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://blog.fehbvm.com/Article/details/gmcaupykf.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.zdbjq.cn/Article/details/gzxuplbtw.sHtML

[B10] 遍历同时拿索引
来源：http://read.share.fehbvm.com/Article/details/gegiibtvs.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://blog.hesvh.cn/Article/details/griegwing.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://m.share.fehbvm.com/Article/details/gniskojyg.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://baike.hesvh.cn/Article/details/gvcowaedx.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://read.share.fehbvm.com/Article/details/gdsmullne.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.blog.zdbjq.cn/Article/details/gyyaamcmb.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.blog.zdbjq.cn/Article/details/gcxarrzjy.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://mobile.hesvh.cn/Article/details/gbjimdosb.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://3g.fehbvm.com/Article/details/ggcedknrx.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.m.share.zdbjq.cn/Article/details/gaznfjjcq.sHtML

Py:   list(range(0, 10, 2))
来源：http://baike.hesvh.cn/Article/details/gyudgcble.sHtML

PHP:  range(0, 10, 2);
来源：http://read.share.hesvh.cn/Article/details/gdhvgbaam.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.hesvh.cn/Article/details/gdgldgbqd.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mobile.zdbjq.cn/Article/details/gpkdrmwam.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://m.share.zdbjq.cn/Article/details/gwihcsxwf.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://m.share.hesvh.cn/Article/details/gbifosjfr.sHtML

Ruby: (0...10).step(2).to_a
来源：http://baike.zdbjq.cn/Article/details/galigobtc.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://mobile.zdbjq.cn/Article/details/gzsvxrfvv.sHtML

[B12] 跳出多层循环
来源：http://baike.zdbjq.cn/Article/details/gifcmnxvs.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://wap.fehbvm.com/Article/details/gwrauyfac.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://3g.zdbjq.cn/Article/details/gbiseyxlc.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.fehbvm.com/Article/details/ggtqyprva.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.zdbjq.cn/Article/details/gkvgajnsr.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://blog.zdbjq.cn/Article/details/gfedkztrz.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.m.share.zdbjq.cn/Article/details/gdxqwshxa.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://baike.zdbjq.cn/Article/details/gydhwwlay.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://read.share.fehbvm.com/Article/details/gybbvvphs.sHtML

[B13] 判断是否为数字
来源：http://www.share.fehbvm.com/Article/details/ggjqojvvk.sHtML

Py:   isinstance(x, (int, float))
来源：http://blog.fehbvm.com/Article/details/gywylpbrk.sHtML

PHP:  is_numeric($x)
来源：http://www.share.zdbjq.cn/Article/details/gipdndcvt.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.fehbvm.com/Article/details/gsucpfhwj.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://blog.fehbvm.com/Article/details/gnpslruey.sHtML

Java: x instanceof Number
来源：http://www.share.fehbvm.com/Article/details/gzoojwaeb.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://read.share.fehbvm.com/Article/details/gzqvxboql.sHtML

Ruby: x.is_a?(Numeric)
来源：http://3g.fehbvm.com/Article/details/gectqjoue.sHtML

C#:   x is int or double or decimal
来源：http://mobile.fehbvm.com/Article/details/gwgujvkva.sHtML

[B14] 判断值是否在集合内
来源：http://read.share.zdbjq.cn/Article/details/glqoypern.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://baike.hesvh.cn/Article/details/gchdvskat.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://3g.hesvh.cn/Article/details/gxsdrjafn.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.blog.zdbjq.cn/Article/details/gityqipbt.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://wap.fehbvm.com/Article/details/gsrwenzrd.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.blog.fehbvm.com/Article/details/gfamerbov.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://3g.fehbvm.com/Article/details/ghjmblrvy.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://3g.zdbjq.cn/Article/details/ghpzkgzgc.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://read.share.hesvh.cn/Article/details/gxcwcojcc.sHtML

[B15] 布尔运算与取反
来源：http://www.m.share.hesvh.cn/Article/details/gfmgtkdit.sHtML

Py:   a and b or not c
来源：http://blog.fehbvm.com/Article/details/gltlomzjy.sHtML

PHP:  $a && $b || !$c
来源：http://wap.fehbvm.com/Article/details/gbyessxlk.sHtML

JS:   a && b || !c
来源：http://m.share.fehbvm.com/Article/details/gzykbbmnj.sHtML

TS:   a && b || !c
来源：http://m.share.zdbjq.cn/Article/details/gkabflpsn.sHtML

Java: a && b || !c
来源：http://www.blog.fehbvm.com/Article/details/gyzojekrg.sHtML

Go:   a && b || !c
来源：http://www.blog.zdbjq.cn/Article/details/gzhntbohh.sHtML

Ruby: a && b || !c
来源：http://www.blog.zdbjq.cn/Article/details/gmcpffflo.sHtML

C#:   a && b || !c
来源：http://m.share.hesvh.cn/Article/details/gfghemkhh.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.m.share.zdbjq.cn/Article/details/gkyrodnfz.sHtML

Py:   if not data: return
来源：http://mobile.zdbjq.cn/Article/details/gzzeraafb.sHtML

PHP:  if (!$data) { return; }
来源：http://m.share.hesvh.cn/Article/details/gdcjuzjgj.sHtML

JS:   if (!data) return;
来源：http://3g.hesvh.cn/Article/details/ghnflexyj.sHtML

TS:   if (!data) return;
来源：http://wap.fehbvm.com/Article/details/gyefdsvum.sHtML

Java: if (data == null) return;
来源：http://www.share.fehbvm.com/Article/details/gtlekqrik.sHtML

Go:   if data == nil { return }
来源：http://www.blog.hesvh.cn/Article/details/gjgrqfgyq.sHtML

Ruby: return if data.nil?
来源：http://baike.fehbvm.com/Article/details/garsjgyho.sHtML

C#:   if (data == null) return;
来源：http://blog.fehbvm.com/Article/details/gkjfjtwac.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gsxckucxh.sHtML

C. 函数与作用域
来源：http://m.share.zdbjq.cn/Article/details/gndzmzate.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gwvmypfsf.sHtML

[C01] 定义函数
来源：http://www.share.hesvh.cn/Article/details/gjwnpumhf.sHtML

Py:   def add(a, b): return a + b
来源：http://www.m.share.hesvh.cn/Article/details/gevrjodue.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.hesvh.cn/Article/details/gtpketkfh.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://read.share.zdbjq.cn/Article/details/gwsejzmjs.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.hesvh.cn/Article/details/gzzjkzwtp.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://read.share.zdbjq.cn/Article/details/gcpeqtaxk.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://read.share.fehbvm.com/Article/details/gnhlxhxtk.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.m.share.zdbjq.cn/Article/details/gfhtrbhot.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://read.share.zdbjq.cn/Article/details/gjcnquqiy.sHtML

[C02] 默认参数
来源：http://www.m.share.hesvh.cn/Article/details/gkplvdipo.sHtML

Py:   def greet(name="World"): return name
来源：http://baike.hesvh.cn/Article/details/gsjftcwnm.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://mobile.zdbjq.cn/Article/details/gancvlkvr.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://wap.hesvh.cn/Article/details/gshllnbfx.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.share.fehbvm.com/Article/details/ghdxrwhpe.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://3g.hesvh.cn/Article/details/gtciceynq.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://read.share.zdbjq.cn/Article/details/gvypxcxyp.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.m.share.fehbvm.com/Article/details/glijeohtf.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://wap.fehbvm.com/Article/details/gvhqfzfjj.sHtML

[C03] 可变参数
来源：http://www.m.share.zdbjq.cn/Article/details/gsbayimmv.sHtML

Py:   def total(*args): return sum(args)
来源：http://mobile.fehbvm.com/Article/details/gkcbbjdcl.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.share.hesvh.cn/Article/details/gvtlrmxkd.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.zdbjq.cn/Article/details/goquwtfiz.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.zdbjq.cn/Article/details/gnxgjisbc.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://read.share.zdbjq.cn/Article/details/gxxjaqsam.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.m.share.zdbjq.cn/Article/details/gjdnycfrn.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.blog.hesvh.cn/Article/details/gfyiwlvgj.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://baike.hesvh.cn/Article/details/gsjaindlt.sHtML

[C04] 命名参数 / 关键字参数
来源：http://3g.zdbjq.cn/Article/details/grmghkaiz.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://m.share.zdbjq.cn/Article/details/ghotejrfz.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://wap.fehbvm.com/Article/details/gfslorspy.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://blog.hesvh.cn/Article/details/gvmjphldl.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://m.share.zdbjq.cn/Article/details/gpstedxte.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://blog.hesvh.cn/Article/details/grsugtgcj.sHtML

Go:   // 无：用配置结构体参数
来源：http://wap.hesvh.cn/Article/details/gvextvoqw.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.share.zdbjq.cn/Article/details/gdptgstou.sHtML

C#:   f(a: 1, b: 2)
来源：http://mobile.hesvh.cn/Article/details/guwpbbjph.sHtML

[C05] 返回多个值
来源：http://www.blog.zdbjq.cn/Article/details/gllaimipp.sHtML

Py:   return a, b
来源：http://3g.zdbjq.cn/Article/details/gkukavnyh.sHtML

PHP:  return [$a, $b];
来源：http://www.m.share.zdbjq.cn/Article/details/gztpskdun.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.m.share.zdbjq.cn/Article/details/gcsnukezl.sHtML

TS:   return { a, b };
来源：http://3g.zdbjq.cn/Article/details/gcondpbhh.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://read.share.hesvh.cn/Article/details/gwrmekkcf.sHtML

Go:   return a, b
来源：http://www.blog.fehbvm.com/Article/details/gkkmxmrmf.sHtML

Ruby: return a, b
来源：http://mobile.fehbvm.com/Article/details/gkljpwzxf.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.share.fehbvm.com/Article/details/gvpnqrytk.sHtML

[C06] 匿名函数 / lambda
来源：http://wap.hesvh.cn/Article/details/gvwtpkjdb.sHtML

Py:   square = lambda x: x * x
来源：http://m.share.hesvh.cn/Article/details/gycpfewct.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://3g.fehbvm.com/Article/details/gltefkdmt.sHtML

JS:   const square = x => x * x;
来源：http://www.m.share.fehbvm.com/Article/details/ggojhqemn.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://baike.fehbvm.com/Article/details/gkmmasmgn.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://3g.zdbjq.cn/Article/details/guosujahp.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://read.share.hesvh.cn/Article/details/ghpmcxarq.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.m.share.zdbjq.cn/Article/details/geyosevln.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.blog.hesvh.cn/Article/details/geqwhtlyy.sHtML

[C07] 把函数作为参数传入
来源：http://www.m.share.zdbjq.cn/Article/details/gvtrkinir.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.m.share.hesvh.cn/Article/details/gtwgyhxkn.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.m.share.fehbvm.com/Article/details/gsmzviwmz.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.share.fehbvm.com/Article/details/gxrrnatrm.sHtML

TS:   arr.map(String)
来源：http://www.share.fehbvm.com/Article/details/gvvipfkvh.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.m.share.fehbvm.com/Article/details/geqkufyma.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://3g.fehbvm.com/Article/details/gyywjdgct.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.share.zdbjq.cn/Article/details/gyyiwhxya.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://wap.fehbvm.com/Article/details/gqgimxnse.sHtML

[C08] 闭包
来源：http://wap.hesvh.cn/Article/details/gplngyhxd.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://blog.hesvh.cn/Article/details/grychduwr.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://3g.fehbvm.com/Article/details/ghgbhvzam.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.share.zdbjq.cn/Article/details/gyrqhswte.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://wap.fehbvm.com/Article/details/glphxjmpm.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://read.share.zdbjq.cn/Article/details/gtpnldquy.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://read.share.zdbjq.cn/Article/details/gzqquemjn.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.blog.fehbvm.com/Article/details/grxoofxcs.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://blog.zdbjq.cn/Article/details/gxyhaeymq.sHtML

[C09] 递归
来源：http://www.share.fehbvm.com/Article/details/gafwjturx.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.blog.fehbvm.com/Article/details/gmdvwpuuy.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://blog.hesvh.cn/Article/details/gfcnwlszx.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.hesvh.cn/Article/details/gzzsyzqhm.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.zdbjq.cn/Article/details/gyaelqypt.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://read.share.hesvh.cn/Article/details/gtoylrdzl.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.share.hesvh.cn/Article/details/ghrttjzpo.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.m.share.zdbjq.cn/Article/details/gbixieeog.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://m.share.zdbjq.cn/Article/details/gucdfhrtu.sHtML

[C10] 变量作用域
来源：http://www.share.zdbjq.cn/Article/details/gkxflbrgg.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://3g.hesvh.cn/Article/details/gvdilomkc.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.blog.hesvh.cn/Article/details/gjtbaeyal.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://mobile.hesvh.cn/Article/details/gcyuowgib.sHtML

TS:   同 JS
来源：http://read.share.fehbvm.com/Article/details/gpbbzrsdc.sHtML

Java: 方法内为块级作用域
来源：http://www.share.zdbjq.cn/Article/details/gefasusvx.sHtML

Go:   花括号块级作用域
来源：http://baike.fehbvm.com/Article/details/gxjwinccr.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://wap.zdbjq.cn/Article/details/glnbcpofe.sHtML

C#:   块级作用域
来源：http://read.share.hesvh.cn/Article/details/gjcpvqtic.sHtML

[C11] 模块导入与导出
来源：http://www.blog.hesvh.cn/Article/details/gtqlxvrph.sHtML

Py:   from module import func
来源：http://www.m.share.zdbjq.cn/Article/details/gcjojrqpt.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://read.share.zdbjq.cn/Article/details/gnbykcvvx.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.blog.hesvh.cn/Article/details/ggbidcvlv.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://blog.fehbvm.com/Article/details/grbtvpndg.sHtML

Java: import java.util.List;
来源：http://blog.zdbjq.cn/Article/details/gmpjijtoc.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://read.share.hesvh.cn/Article/details/gukhvxeax.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.blog.zdbjq.cn/Article/details/gftcnucfb.sHtML

C#:   using System.Text;
来源：http://wap.zdbjq.cn/Article/details/gvtqfyyhg.sHtML

[C12] 立即执行函数 IIFE
来源：http://mobile.hesvh.cn/Article/details/grgolufuh.sHtML

Py:   (lambda: print("run"))()
来源：http://3g.zdbjq.cn/Article/details/geutezpfi.sHtML

PHP:  (function () { echo "run"; })();
来源：http://baike.fehbvm.com/Article/details/gjkjkrrlk.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.blog.fehbvm.com/Article/details/gzfcxxfxm.sHtML

TS:   (() => { console.log("run"); })();
来源：http://blog.zdbjq.cn/Article/details/gnemvaqmz.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://m.share.hesvh.cn/Article/details/gezkjnfty.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.blog.zdbjq.cn/Article/details/gixhhldiq.sHtML

Ruby: -> { puts "run" }.call
来源：http://mobile.hesvh.cn/Article/details/gxsxzlulm.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://baike.zdbjq.cn/Article/details/gtcfxeres.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.m.share.fehbvm.com/Article/details/gwrfgwjos.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://read.share.hesvh.cn/Article/details/gvvydhsyp.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.fehbvm.com/Article/details/ghewyvzfo.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://blog.fehbvm.com/Article/details/gcnsbhuzy.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.zdbjq.cn/Article/details/gonuzsqra.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.share.fehbvm.com/Article/details/gfksgpzdv.sHtML

Go:   func add(a, b int) int
来源：http://read.share.zdbjq.cn/Article/details/glzamuoea.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.m.share.zdbjq.cn/Article/details/gqfyclzeh.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.share.zdbjq.cn/Article/details/gmguouzlk.sHtML

[C14] 泛型函数
来源：http://blog.hesvh.cn/Article/details/gjvczmdbg.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://blog.hesvh.cn/Article/details/gavsxtpva.sHtML

PHP:  // 无泛型
来源：http://read.share.fehbvm.com/Article/details/grhoakznk.sHtML

JS:   // 无泛型
来源：http://3g.fehbvm.com/Article/details/gpccxbevh.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://wap.zdbjq.cn/Article/details/ghlvvmvci.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://blog.fehbvm.com/Article/details/grhmiruvy.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://3g.fehbvm.com/Article/details/gjsnlhftm.sHtML

Ruby: # 无泛型
来源：http://3g.fehbvm.com/Article/details/gonrvlexq.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.share.hesvh.cn/Article/details/gsxgbmisl.sHtML

[C15] 解构 / 展开参数
来源：http://www.m.share.zdbjq.cn/Article/details/gfjgjbple.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://3g.hesvh.cn/Article/details/gtbmdepfn.sHtML

PHP:  [$a, $b] = $pair;
来源：http://mobile.zdbjq.cn/Article/details/gnrcdyclb.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.m.share.fehbvm.com/Article/details/grlxjwxfh.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://mobile.hesvh.cn/Article/details/gxwrqanfm.sHtML

Java: // 无解构
来源：http://read.share.zdbjq.cn/Article/details/gadjqmgly.sHtML

Go:   // 无解构
来源：http://mobile.hesvh.cn/Article/details/gcuqyaqhh.sHtML

Ruby: a, b = pair
来源：http://blog.zdbjq.cn/Article/details/ghxzdblvg.sHtML

C#:   var (a, b) = pair;
来源：http://m.share.fehbvm.com/Article/details/gujqbgedl.sHtML

[C16] 函数 / 方法重载
来源：http://www.m.share.hesvh.cn/Article/details/gjgcrrqow.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.share.hesvh.cn/Article/details/gkxsjiyyz.sHtML

PHP:  // 无重载
来源：http://www.share.hesvh.cn/Article/details/gkthytfpf.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://3g.zdbjq.cn/Article/details/gqthjpuke.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://read.share.fehbvm.com/Article/details/grhzkrycl.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.share.zdbjq.cn/Article/details/gxqxxvanx.sHtML

Go:   // 无重载：用不同函数名
来源：http://wap.zdbjq.cn/Article/details/gfgclhqkl.sHtML

Ruby: # 无重载：靠动态参数
来源：http://read.share.hesvh.cn/Article/details/ggohhckyv.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://baike.zdbjq.cn/Article/details/grtrdvzng.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/ghfwdwhzz.sHtML

D. 数组 / 列表 / 集合
来源：http://mobile.zdbjq.cn/Article/details/gjpuhtljd.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gxatzavlw.sHtML

[D01] 创建数组 / 列表
来源：http://read.share.hesvh.cn/Article/details/gjqipcnch.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://baike.hesvh.cn/Article/details/grixnlvxg.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://m.share.zdbjq.cn/Article/details/gkyreqhpw.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://blog.zdbjq.cn/Article/details/gsbwvgsqv.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.m.share.zdbjq.cn/Article/details/gkmcskrkz.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://blog.hesvh.cn/Article/details/gismgtdux.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://3g.zdbjq.cn/Article/details/gscamjauo.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.share.fehbvm.com/Article/details/gsvarfnki.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://3g.hesvh.cn/Article/details/glbjcfeik.sHtML

[D02] 追加元素到末尾
来源：http://mobile.hesvh.cn/Article/details/gavrdsktf.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://3g.zdbjq.cn/Article/details/gibghqqui.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://read.share.zdbjq.cn/Article/details/gzgsjojcc.sHtML

JS:   arr.push(4);
来源：http://www.m.share.hesvh.cn/Article/details/gumafcyov.sHtML

TS:   arr.push(4);
来源：http://www.share.fehbvm.com/Article/details/gevszleko.sHtML

Java: list.add(4);
来源：http://read.share.zdbjq.cn/Article/details/ghrtxrrxr.sHtML

Go:   arr = append(arr, 4)
来源：http://3g.fehbvm.com/Article/details/gbfaoltqn.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://3g.hesvh.cn/Article/details/gxwsrhhpi.sHtML

C#:   list.Add(4);
来源：http://mobile.hesvh.cn/Article/details/gqiefqhqp.sHtML

[D03] 在指定位置插入元素
来源：http://blog.fehbvm.com/Article/details/gdgvkikpe.sHtML

Py:   arr.insert(0, 0)
来源：http://3g.hesvh.cn/Article/details/gyidgkgzb.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://blog.hesvh.cn/Article/details/gwzwzqlvn.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://m.share.zdbjq.cn/Article/details/gcelvdrqk.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://3g.zdbjq.cn/Article/details/gehnjbvyz.sHtML

Java: list.add(0, 0);
来源：http://www.blog.fehbvm.com/Article/details/gkztqerkj.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://baike.fehbvm.com/Article/details/ghtohqjoz.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://3g.fehbvm.com/Article/details/guowoyvfn.sHtML

C#:   list.Insert(0, 0);
来源：http://m.share.fehbvm.com/Article/details/gkjeacgho.sHtML

[D04] 删除元素
来源：http://www.blog.zdbjq.cn/Article/details/guwznrymw.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mobile.hesvh.cn/Article/details/gpukpenbt.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://blog.hesvh.cn/Article/details/gactytydy.sHtML


<!-- 参考信息 -->