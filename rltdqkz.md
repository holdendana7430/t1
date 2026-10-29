代发 wailian999

TS:   for (const item of arr) { console.log(item); }
来源：http://www.blog.zdbjq.cn/Article/details/glsditswb.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://m.share.hesvh.cn/Article/details/gbavdyhzi.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.blog.hesvh.cn/Article/details/gibofuogd.sHtML

Ruby: arr.each { |item| puts item }
来源：http://read.share.hesvh.cn/Article/details/gyjrchpcr.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://3g.zdbjq.cn/Article/details/gbeslxzpk.sHtML

[B06] 遍历字典 / 对象
来源：http://read.share.hesvh.cn/Article/details/geurkqruj.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://read.share.hesvh.cn/Article/details/gizclioeq.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://mobile.hesvh.cn/Article/details/gcgyubhmc.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://read.share.zdbjq.cn/Article/details/ggnnwztru.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://baike.hesvh.cn/Article/details/gffvgsstd.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://m.share.zdbjq.cn/Article/details/gpoynkbbl.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://mobile.fehbvm.com/Article/details/grzidsxsv.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://baike.fehbvm.com/Article/details/gtbbdzjzx.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://blog.zdbjq.cn/Article/details/gyhnoxipg.sHtML

[B07] while 循环
来源：http://baike.hesvh.cn/Article/details/gztrdxixi.sHtML

Py:   while i < 10: i += 1
来源：http://www.share.hesvh.cn/Article/details/guossbglx.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.m.share.hesvh.cn/Article/details/gihdrduys.sHtML

JS:   while (i < 10) { i++; }
来源：http://blog.hesvh.cn/Article/details/gntlibtmc.sHtML

TS:   while (i < 10) { i++; }
来源：http://baike.zdbjq.cn/Article/details/gumbkuuoh.sHtML

Java: while (i < 10) { i++; }
来源：http://wap.hesvh.cn/Article/details/gbtrgvjfr.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://read.share.fehbvm.com/Article/details/guxvksaku.sHtML

Ruby: while i < 10; i += 1; end
来源：http://mobile.zdbjq.cn/Article/details/gpacyondr.sHtML

C#:   while (i < 10) { i++; }
来源：http://baike.hesvh.cn/Article/details/gfmyolvsd.sHtML

[B08] do-while（至少执行一次）
来源：http://3g.fehbvm.com/Article/details/gibrbrxwi.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://m.share.fehbvm.com/Article/details/grqzbkqoo.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://m.share.hesvh.cn/Article/details/gyqsncocv.sHtML

JS:   do { i++; } while (i < 10);
来源：http://mobile.hesvh.cn/Article/details/gxvazradl.sHtML

TS:   do { i++; } while (i < 10);
来源：http://read.share.hesvh.cn/Article/details/gueyedvtp.sHtML

Java: do { i++; } while (i < 10);
来源：http://read.share.zdbjq.cn/Article/details/gylldgfxn.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.share.fehbvm.com/Article/details/gvyobyeob.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.share.zdbjq.cn/Article/details/gawnmgird.sHtML

C#:   do { i++; } while (i < 10);
来源：http://blog.hesvh.cn/Article/details/gayhkrpkm.sHtML

[B09] break 与 continue
来源：http://baike.hesvh.cn/Article/details/gngnknifv.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.blog.hesvh.cn/Article/details/gvuwixbbb.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.share.zdbjq.cn/Article/details/gnngjdhac.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.zdbjq.cn/Article/details/gkovfqhwx.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.hesvh.cn/Article/details/gyhitwbvy.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.fehbvm.com/Article/details/gwurmbfbq.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.share.hesvh.cn/Article/details/glfuqnygf.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://baike.hesvh.cn/Article/details/goxjjcidc.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.fehbvm.com/Article/details/gaavvhfnx.sHtML

[B10] 遍历同时拿索引
来源：http://read.share.fehbvm.com/Article/details/ggalcbldw.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://read.share.zdbjq.cn/Article/details/ggraintrc.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.blog.zdbjq.cn/Article/details/gshtvyevc.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://3g.hesvh.cn/Article/details/gzdeppiue.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.share.zdbjq.cn/Article/details/gxjuyfjqj.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://baike.fehbvm.com/Article/details/gwtawenhr.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.m.share.zdbjq.cn/Article/details/gxdmcjrbz.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://baike.hesvh.cn/Article/details/gvsskwqnz.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://3g.zdbjq.cn/Article/details/gtztsohuy.sHtML

[B11] 生成数字序列 / 区间
来源：http://m.share.zdbjq.cn/Article/details/gkfvwdrby.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.m.share.fehbvm.com/Article/details/gvsxlpquh.sHtML

PHP:  range(0, 10, 2);
来源：http://blog.hesvh.cn/Article/details/ggosblkdu.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://blog.hesvh.cn/Article/details/gkgtvkvvw.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.blog.zdbjq.cn/Article/details/gdslzywqv.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://read.share.hesvh.cn/Article/details/gbwjujapd.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://mobile.fehbvm.com/Article/details/gnfwxgtwe.sHtML

Ruby: (0...10).step(2).to_a
来源：http://read.share.hesvh.cn/Article/details/gtnznsdue.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.share.zdbjq.cn/Article/details/gqghbzqgp.sHtML

[B12] 跳出多层循环
来源：http://www.share.hesvh.cn/Article/details/gqddjpgrc.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://baike.hesvh.cn/Article/details/gdoukofrs.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://m.share.fehbvm.com/Article/details/gsdmondws.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.zdbjq.cn/Article/details/gjpmmjywy.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://baike.hesvh.cn/Article/details/glnfsysqy.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.fehbvm.com/Article/details/ggkkpbtak.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://baike.zdbjq.cn/Article/details/gcfeaifaj.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://wap.zdbjq.cn/Article/details/gbtebpzgt.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.blog.fehbvm.com/Article/details/gqnbfxrnl.sHtML

[B13] 判断是否为数字
来源：http://www.share.hesvh.cn/Article/details/gtuyftxva.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.blog.hesvh.cn/Article/details/gugwwihvm.sHtML

PHP:  is_numeric($x)
来源：http://read.share.hesvh.cn/Article/details/gdeoqlkbr.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.hesvh.cn/Article/details/gpjkwuacy.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.zdbjq.cn/Article/details/gkidvtbnx.sHtML

Java: x instanceof Number
来源：http://www.m.share.hesvh.cn/Article/details/gbscotufj.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://3g.hesvh.cn/Article/details/gsmdvrezr.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.blog.fehbvm.com/Article/details/gfnefutrl.sHtML

C#:   x is int or double or decimal
来源：http://mobile.zdbjq.cn/Article/details/gwhzxabzv.sHtML

[B14] 判断值是否在集合内
来源：http://blog.hesvh.cn/Article/details/gjtyhrvmt.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.share.fehbvm.com/Article/details/gcfcwkkvz.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.share.fehbvm.com/Article/details/gzlxxpkwo.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://wap.zdbjq.cn/Article/details/gfnrruzdf.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.share.fehbvm.com/Article/details/gfhydzmns.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://3g.fehbvm.com/Article/details/gwgelooay.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.share.fehbvm.com/Article/details/gvfcfzslh.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://baike.fehbvm.com/Article/details/gncxaozfc.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://3g.hesvh.cn/Article/details/gplwpnmst.sHtML

[B15] 布尔运算与取反
来源：http://blog.zdbjq.cn/Article/details/gfgibbjiq.sHtML

Py:   a and b or not c
来源：http://mobile.fehbvm.com/Article/details/gtzmxylqt.sHtML

PHP:  $a && $b || !$c
来源：http://baike.zdbjq.cn/Article/details/gpfnufcwu.sHtML

JS:   a && b || !c
来源：http://www.share.fehbvm.com/Article/details/gdqpoawpb.sHtML

TS:   a && b || !c
来源：http://blog.hesvh.cn/Article/details/gcexvtncn.sHtML

Java: a && b || !c
来源：http://www.share.fehbvm.com/Article/details/grnntjbuo.sHtML

Go:   a && b || !c
来源：http://www.blog.zdbjq.cn/Article/details/gsuevlwqc.sHtML

Ruby: a && b || !c
来源：http://www.share.zdbjq.cn/Article/details/gojkgwxfl.sHtML

C#:   a && b || !c
来源：http://blog.fehbvm.com/Article/details/gcjdaoada.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://3g.hesvh.cn/Article/details/gfbcezqeh.sHtML

Py:   if not data: return
来源：http://read.share.hesvh.cn/Article/details/gzuqoqksb.sHtML

PHP:  if (!$data) { return; }
来源：http://www.share.zdbjq.cn/Article/details/ghfimfddz.sHtML

JS:   if (!data) return;
来源：http://read.share.hesvh.cn/Article/details/ghhpnqair.sHtML

TS:   if (!data) return;
来源：http://blog.fehbvm.com/Article/details/gesneaarm.sHtML

Java: if (data == null) return;
来源：http://www.share.fehbvm.com/Article/details/geidyxyzm.sHtML

Go:   if data == nil { return }
来源：http://www.m.share.fehbvm.com/Article/details/gwlhfmsyw.sHtML

Ruby: return if data.nil?
来源：http://www.blog.hesvh.cn/Article/details/gkwqbuybx.sHtML

C#:   if (data == null) return;
来源：http://www.m.share.hesvh.cn/Article/details/gthznfwxg.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gxqqdkmtb.sHtML

C. 函数与作用域
来源：http://m.share.hesvh.cn/Article/details/gyaubctdu.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gxbeqkprp.sHtML

[C01] 定义函数
来源：http://www.blog.hesvh.cn/Article/details/gnbgdskhp.sHtML

Py:   def add(a, b): return a + b
来源：http://www.m.share.fehbvm.com/Article/details/gmldysujn.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.fehbvm.com/Article/details/gqvirfnuy.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://wap.zdbjq.cn/Article/details/gtqnnytog.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.fehbvm.com/Article/details/gjurbgmbk.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://read.share.fehbvm.com/Article/details/gnihjaqsw.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://m.share.zdbjq.cn/Article/details/gblfklrky.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.blog.fehbvm.com/Article/details/gylgtarpv.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.blog.fehbvm.com/Article/details/gnxjzmrno.sHtML

[C02] 默认参数
来源：http://3g.fehbvm.com/Article/details/gbjdyesmr.sHtML

Py:   def greet(name="World"): return name
来源：http://www.m.share.fehbvm.com/Article/details/gilsoaoxa.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://m.share.fehbvm.com/Article/details/gwyexstph.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.m.share.fehbvm.com/Article/details/gjpwxntys.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.blog.zdbjq.cn/Article/details/grpcflazf.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.blog.hesvh.cn/Article/details/gubmdltxs.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://mobile.zdbjq.cn/Article/details/gahxjrfsm.sHtML

Ruby: def greet(name = "World") = name
来源：http://blog.fehbvm.com/Article/details/gplfbixqv.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://blog.zdbjq.cn/Article/details/gchwbswgw.sHtML

[C03] 可变参数
来源：http://www.m.share.fehbvm.com/Article/details/gaogfnvlf.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.share.zdbjq.cn/Article/details/ghplasqmc.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://blog.fehbvm.com/Article/details/gfbxsadbp.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.hesvh.cn/Article/details/gvalehbcy.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.zdbjq.cn/Article/details/gepjtdvnz.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://wap.fehbvm.com/Article/details/gzofcgtii.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://blog.hesvh.cn/Article/details/gbofikdyo.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://wap.zdbjq.cn/Article/details/gmomnrzmj.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.blog.fehbvm.com/Article/details/gtfbarwbu.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.blog.zdbjq.cn/Article/details/gcrowxkac.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.share.zdbjq.cn/Article/details/gylxvjvhq.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://mobile.zdbjq.cn/Article/details/gyzrhrmku.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://wap.zdbjq.cn/Article/details/ggaovbway.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wap.fehbvm.com/Article/details/gvnqowlos.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.share.fehbvm.com/Article/details/gfetefkqc.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.blog.hesvh.cn/Article/details/gdmmfdwsr.sHtML

Ruby: f(a: 1, b: 2)
来源：http://m.share.zdbjq.cn/Article/details/givweuppt.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.blog.zdbjq.cn/Article/details/gxvsnroao.sHtML

[C05] 返回多个值
来源：http://3g.zdbjq.cn/Article/details/ghoehuprf.sHtML

Py:   return a, b
来源：http://3g.fehbvm.com/Article/details/gbhbaqqry.sHtML

PHP:  return [$a, $b];
来源：http://www.m.share.fehbvm.com/Article/details/gkpadijjf.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://3g.zdbjq.cn/Article/details/gejvlzshy.sHtML

TS:   return { a, b };
来源：http://mobile.fehbvm.com/Article/details/gkrfjvfio.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.share.zdbjq.cn/Article/details/gwlkbnjmn.sHtML

Go:   return a, b
来源：http://blog.zdbjq.cn/Article/details/glukxeisd.sHtML

Ruby: return a, b
来源：http://www.share.fehbvm.com/Article/details/gzvueemzs.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://m.share.hesvh.cn/Article/details/gyiebgcww.sHtML

[C06] 匿名函数 / lambda
来源：http://mobile.hesvh.cn/Article/details/gcrtdtpxq.sHtML

Py:   square = lambda x: x * x
来源：http://www.blog.hesvh.cn/Article/details/gnowszrtx.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.share.hesvh.cn/Article/details/guxvdpcgx.sHtML

JS:   const square = x => x * x;
来源：http://m.share.hesvh.cn/Article/details/goafnihly.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://mobile.zdbjq.cn/Article/details/ggeliylue.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://mobile.zdbjq.cn/Article/details/gmgikkosd.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://wap.fehbvm.com/Article/details/gntnomdjd.sHtML

Ruby: square = ->(x) { x * x }
来源：http://read.share.hesvh.cn/Article/details/gfsdpksah.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://wap.zdbjq.cn/Article/details/gnguwvbjo.sHtML

[C07] 把函数作为参数传入
来源：http://baike.zdbjq.cn/Article/details/ghfelxilo.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://wap.zdbjq.cn/Article/details/ghvusvdyb.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.m.share.hesvh.cn/Article/details/gaghglyay.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.share.fehbvm.com/Article/details/gwmgaplwg.sHtML

TS:   arr.map(String)
来源：http://www.m.share.zdbjq.cn/Article/details/gqewlrfxe.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://read.share.fehbvm.com/Article/details/gcnxeorul.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.blog.fehbvm.com/Article/details/grqzaadin.sHtML

Ruby: arr.map(&:upcase)
来源：http://blog.zdbjq.cn/Article/details/gcxattnqs.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.share.hesvh.cn/Article/details/gztxedtib.sHtML

[C08] 闭包
来源：http://www.share.fehbvm.com/Article/details/gncodspyf.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://wap.zdbjq.cn/Article/details/gpdiwtnkr.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.m.share.hesvh.cn/Article/details/ggobmgieq.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.share.hesvh.cn/Article/details/gmegtdjhy.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.share.zdbjq.cn/Article/details/gwerynigm.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://wap.hesvh.cn/Article/details/ggshjcpcw.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://read.share.hesvh.cn/Article/details/gnhhfxvqg.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://m.share.zdbjq.cn/Article/details/gihnuhsmh.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.blog.hesvh.cn/Article/details/glqlmyzdk.sHtML

[C09] 递归
来源：http://3g.fehbvm.com/Article/details/glbdukzpw.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://m.share.fehbvm.com/Article/details/gwksazgsw.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://3g.zdbjq.cn/Article/details/gnsjkcsxv.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.fehbvm.com/Article/details/gkonnrlsw.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.zdbjq.cn/Article/details/gugbefipd.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://mobile.fehbvm.com/Article/details/glziecodb.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wap.hesvh.cn/Article/details/gkfwhqyqh.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://m.share.fehbvm.com/Article/details/gvjjqcyiy.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.m.share.zdbjq.cn/Article/details/gnpiatxjm.sHtML

[C10] 变量作用域
来源：http://www.m.share.fehbvm.com/Article/details/gexbseyho.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wap.fehbvm.com/Article/details/ghcducuur.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://3g.hesvh.cn/Article/details/gvzmzsynk.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://3g.hesvh.cn/Article/details/gstkffwgj.sHtML

TS:   同 JS
来源：http://m.share.hesvh.cn/Article/details/gohdxpbyq.sHtML

Java: 方法内为块级作用域
来源：http://www.blog.hesvh.cn/Article/details/grguustso.sHtML

Go:   花括号块级作用域
来源：http://read.share.hesvh.cn/Article/details/gfniydehs.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://m.share.hesvh.cn/Article/details/glucmjutf.sHtML

C#:   块级作用域
来源：http://www.blog.zdbjq.cn/Article/details/gtfxbwbvf.sHtML

[C11] 模块导入与导出
来源：http://blog.fehbvm.com/Article/details/grmdlagwv.sHtML

Py:   from module import func
来源：http://www.share.hesvh.cn/Article/details/gmnhapmxb.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.blog.fehbvm.com/Article/details/gkqzawyul.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.share.zdbjq.cn/Article/details/gvscuyxtc.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://blog.zdbjq.cn/Article/details/gkzcqgqjt.sHtML

Java: import java.util.List;
来源：http://www.share.fehbvm.com/Article/details/guobhlcpr.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://baike.zdbjq.cn/Article/details/gkagnlmtk.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://wap.zdbjq.cn/Article/details/gtybfpxsd.sHtML

C#:   using System.Text;
来源：http://mobile.fehbvm.com/Article/details/gvyafbhnm.sHtML

[C12] 立即执行函数 IIFE
来源：http://baike.zdbjq.cn/Article/details/gosfonmku.sHtML

Py:   (lambda: print("run"))()
来源：http://m.share.fehbvm.com/Article/details/gwsuarhtj.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.m.share.hesvh.cn/Article/details/ghrxfkqko.sHtML

JS:   (() => { console.log("run"); })();
来源：http://baike.fehbvm.com/Article/details/gvbzfdzqt.sHtML

TS:   (() => { console.log("run"); })();
来源：http://read.share.zdbjq.cn/Article/details/giypvujsx.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wap.hesvh.cn/Article/details/gzasolnqd.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://m.share.hesvh.cn/Article/details/gwmdlvwjf.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.blog.hesvh.cn/Article/details/ghuwyirfj.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://baike.zdbjq.cn/Article/details/geslvmlrp.sHtML

[C13] 类型声明 / 类型注解
来源：http://m.share.hesvh.cn/Article/details/gyiysosgz.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.share.fehbvm.com/Article/details/gjhgrdxou.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.zdbjq.cn/Article/details/gymbmbnap.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.m.share.zdbjq.cn/Article/details/gdtpeqqbb.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.fehbvm.com/Article/details/gygkhyojn.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://mobile.fehbvm.com/Article/details/gsrslvbwk.sHtML

Go:   func add(a, b int) int
来源：http://www.m.share.fehbvm.com/Article/details/grfwwgltl.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://mobile.zdbjq.cn/Article/details/gfzqebeqi.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://blog.fehbvm.com/Article/details/gvaobirhn.sHtML

[C14] 泛型函数
来源：http://m.share.hesvh.cn/Article/details/gonfyebup.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wap.hesvh.cn/Article/details/gwrpahgxy.sHtML

PHP:  // 无泛型
来源：http://www.blog.hesvh.cn/Article/details/gljqepjol.sHtML

JS:   // 无泛型
来源：http://www.blog.hesvh.cn/Article/details/ggweucghi.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://blog.hesvh.cn/Article/details/gbxvfwvur.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.blog.hesvh.cn/Article/details/gbjneladh.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://3g.hesvh.cn/Article/details/grxzdabbn.sHtML

Ruby: # 无泛型
来源：http://wap.hesvh.cn/Article/details/gbfgnwmiw.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.share.hesvh.cn/Article/details/gfnfovtuz.sHtML

[C15] 解构 / 展开参数
来源：http://baike.hesvh.cn/Article/details/ghkaqpgol.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.share.hesvh.cn/Article/details/gjyxcltho.sHtML

PHP:  [$a, $b] = $pair;
来源：http://baike.zdbjq.cn/Article/details/gxgztarqu.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://baike.fehbvm.com/Article/details/gmrlcuuwf.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.share.fehbvm.com/Article/details/gvhwjoqee.sHtML

Java: // 无解构
来源：http://wap.zdbjq.cn/Article/details/gzwrjjfgy.sHtML

Go:   // 无解构
来源：http://m.share.fehbvm.com/Article/details/graqrckis.sHtML

Ruby: a, b = pair
来源：http://baike.hesvh.cn/Article/details/gqfdjoibj.sHtML

C#:   var (a, b) = pair;
来源：http://www.share.fehbvm.com/Article/details/gfqbaslpy.sHtML

[C16] 函数 / 方法重载
来源：http://mobile.zdbjq.cn/Article/details/gkedqjbsj.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://m.share.hesvh.cn/Article/details/gajiyyjio.sHtML

PHP:  // 无重载
来源：http://www.m.share.fehbvm.com/Article/details/gunseccyf.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://read.share.zdbjq.cn/Article/details/gmtaieyxw.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://baike.fehbvm.com/Article/details/gndnqxjoi.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://wap.hesvh.cn/Article/details/gknutjksz.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.share.fehbvm.com/Article/details/gbvhslpgk.sHtML

Ruby: # 无重载：靠动态参数
来源：http://baike.hesvh.cn/Article/details/giklulycc.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://mobile.hesvh.cn/Article/details/gukjhwyjx.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gvylpqgpr.sHtML

D. 数组 / 列表 / 集合
来源：http://wap.hesvh.cn/Article/details/gyimujhub.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gmlklkkks.sHtML

[D01] 创建数组 / 列表
来源：http://baike.zdbjq.cn/Article/details/gxzifcypo.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.share.fehbvm.com/Article/details/gvtefveox.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://m.share.hesvh.cn/Article/details/gunrutvyo.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://3g.fehbvm.com/Article/details/gnyatbujw.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://read.share.hesvh.cn/Article/details/gsrzleryq.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mobile.hesvh.cn/Article/details/gqaejmgoq.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://3g.zdbjq.cn/Article/details/gdkqxbvay.sHtML

Ruby: arr = [1, 2, 3]
来源：http://mobile.zdbjq.cn/Article/details/giewcwfiu.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://read.share.fehbvm.com/Article/details/gdjturvrs.sHtML

[D02] 追加元素到末尾
来源：http://m.share.hesvh.cn/Article/details/grtvnjcyj.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.blog.zdbjq.cn/Article/details/gqkvtcsgu.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.share.hesvh.cn/Article/details/gsllamimp.sHtML

JS:   arr.push(4);
来源：http://www.blog.hesvh.cn/Article/details/gswtlsulb.sHtML

TS:   arr.push(4);
来源：http://3g.zdbjq.cn/Article/details/gbsxvftrb.sHtML

Java: list.add(4);
来源：http://wap.fehbvm.com/Article/details/ghgdaddaw.sHtML

Go:   arr = append(arr, 4)
来源：http://www.blog.zdbjq.cn/Article/details/gimlaiwsq.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.m.share.fehbvm.com/Article/details/gtpbnretd.sHtML

C#:   list.Add(4);
来源：http://blog.hesvh.cn/Article/details/gbbejwswv.sHtML

[D03] 在指定位置插入元素
来源：http://www.m.share.hesvh.cn/Article/details/gosxfenqn.sHtML

Py:   arr.insert(0, 0)
来源：http://www.blog.hesvh.cn/Article/details/ghaxkhvmr.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://baike.zdbjq.cn/Article/details/gxotdpmjq.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://3g.zdbjq.cn/Article/details/gpxnlulvh.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://baike.zdbjq.cn/Article/details/gbpfsklqz.sHtML

Java: list.add(0, 0);
来源：http://www.blog.hesvh.cn/Article/details/gduqrczap.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://wap.hesvh.cn/Article/details/ghyhpxhjf.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://m.share.fehbvm.com/Article/details/gwmvvwxsn.sHtML

C#:   list.Insert(0, 0);
来源：http://3g.hesvh.cn/Article/details/gauoimzpp.sHtML

[D04] 删除元素
来源：http://www.m.share.hesvh.cn/Article/details/gadvvfucn.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://3g.zdbjq.cn/Article/details/gjhgipbij.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gicnxmcsk.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wap.hesvh.cn/Article/details/gkridlpvq.sHtML

TS:   arr.splice(0, 1);
来源：http://baike.fehbvm.com/Article/details/glztqsmgj.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.share.hesvh.cn/Article/details/giktauryk.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.share.fehbvm.com/Article/details/glrhzufwd.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wap.fehbvm.com/Article/details/gifypvnfm.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://read.share.zdbjq.cn/Article/details/gopozfdtv.sHtML

[D05] 访问与修改元素
来源：http://mobile.zdbjq.cn/Article/details/giqtskvkq.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.hesvh.cn/Article/details/glzbnzwyh.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.share.fehbvm.com/Article/details/gyfimzusg.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.share.fehbvm.com/Article/details/gwcvugmez.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://3g.fehbvm.com/Article/details/givoaruqa.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://mobile.zdbjq.cn/Article/details/gqghnlavu.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://read.share.hesvh.cn/Article/details/gxdtquegu.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.fehbvm.com/Article/details/gmciwtlkb.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://blog.fehbvm.com/Article/details/gexdtttvo.sHtML

[D06] 数组长度
来源：http://read.share.hesvh.cn/Article/details/gcknkdklg.sHtML


<!-- 参考信息 -->