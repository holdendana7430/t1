代发 wailian999

[B05] 遍历数组 / 列表
来源：http://blog.fehbvm.com/Article/details/gjcjrhrjx.sHtML

Py:   for item in arr: print(item)
来源：http://www.m.share.fehbvm.com/Article/details/grhhxftlu.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://m.share.hesvh.cn/Article/details/gnaftwzyw.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://read.share.fehbvm.com/Article/details/gebeejnwi.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.share.zdbjq.cn/Article/details/guzxnsspt.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://read.share.hesvh.cn/Article/details/gwbomuvck.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://blog.zdbjq.cn/Article/details/ggawgdpei.sHtML

Ruby: arr.each { |item| puts item }
来源：http://read.share.zdbjq.cn/Article/details/gyyramubf.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://mobile.hesvh.cn/Article/details/gvqrzoipa.sHtML

[B06] 遍历字典 / 对象
来源：http://read.share.zdbjq.cn/Article/details/gxadzzwsa.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://3g.fehbvm.com/Article/details/ghdvbwcvz.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://m.share.zdbjq.cn/Article/details/gtqnmgpup.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mobile.fehbvm.com/Article/details/ghicougnd.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://read.share.fehbvm.com/Article/details/gpbgwfciu.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://wap.fehbvm.com/Article/details/gqvdtbgjx.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://baike.fehbvm.com/Article/details/gdpebwtvz.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://read.share.zdbjq.cn/Article/details/gclvevppb.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.m.share.fehbvm.com/Article/details/gnkoiyidl.sHtML

[B07] while 循环
来源：http://baike.hesvh.cn/Article/details/gyfakhfsa.sHtML

Py:   while i < 10: i += 1
来源：http://www.share.fehbvm.com/Article/details/gciiftatv.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://baike.zdbjq.cn/Article/details/gapezxyxk.sHtML

JS:   while (i < 10) { i++; }
来源：http://baike.fehbvm.com/Article/details/gpvhthteq.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.blog.zdbjq.cn/Article/details/gxlxayujp.sHtML

Java: while (i < 10) { i++; }
来源：http://read.share.hesvh.cn/Article/details/gwxhnjmbs.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://3g.zdbjq.cn/Article/details/grgckdqry.sHtML

Ruby: while i < 10; i += 1; end
来源：http://wap.hesvh.cn/Article/details/gnlckpbce.sHtML

C#:   while (i < 10) { i++; }
来源：http://read.share.zdbjq.cn/Article/details/gpwckrwps.sHtML

[B08] do-while（至少执行一次）
来源：http://www.m.share.zdbjq.cn/Article/details/gghnoobus.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.m.share.zdbjq.cn/Article/details/grizjlpbp.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://m.share.hesvh.cn/Article/details/giunqhvns.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.blog.hesvh.cn/Article/details/gwtiswrke.sHtML

TS:   do { i++; } while (i < 10);
来源：http://baike.hesvh.cn/Article/details/gcbbioxwv.sHtML

Java: do { i++; } while (i < 10);
来源：http://baike.hesvh.cn/Article/details/geedonzzs.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://m.share.fehbvm.com/Article/details/gqxznkneg.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://wap.fehbvm.com/Article/details/gmvidvhql.sHtML

C#:   do { i++; } while (i < 10);
来源：http://m.share.zdbjq.cn/Article/details/gkeoptehv.sHtML

[B09] break 与 continue
来源：http://www.share.hesvh.cn/Article/details/gmtvhdclq.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://mobile.hesvh.cn/Article/details/gcaujiekx.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.blog.zdbjq.cn/Article/details/gpanlxrhl.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.fehbvm.com/Article/details/gxthklecf.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.zdbjq.cn/Article/details/gjrztxjdi.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.hesvh.cn/Article/details/gihzlugvh.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://baike.hesvh.cn/Article/details/ghtidtmmu.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://m.share.zdbjq.cn/Article/details/gqdlfmhvv.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.zdbjq.cn/Article/details/giidpbsbj.sHtML

[B10] 遍历同时拿索引
来源：http://read.share.zdbjq.cn/Article/details/gvulpcnwt.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.share.hesvh.cn/Article/details/gsriqyfkr.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://mobile.fehbvm.com/Article/details/ggxdtxoku.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.m.share.fehbvm.com/Article/details/gmrvonwxo.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://blog.zdbjq.cn/Article/details/gtmjsxpqn.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://mobile.hesvh.cn/Article/details/gtoeajvxu.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://read.share.hesvh.cn/Article/details/gwivfpguc.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://blog.fehbvm.com/Article/details/gxtchznxo.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.share.fehbvm.com/Article/details/gkgttgxyk.sHtML

[B11] 生成数字序列 / 区间
来源：http://3g.fehbvm.com/Article/details/gnwbajiey.sHtML

Py:   list(range(0, 10, 2))
来源：http://read.share.fehbvm.com/Article/details/gvaaajoka.sHtML

PHP:  range(0, 10, 2);
来源：http://m.share.fehbvm.com/Article/details/glzsdmmoa.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.blog.fehbvm.com/Article/details/glmslwyvw.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.fehbvm.com/Article/details/gdlxeoitt.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.m.share.zdbjq.cn/Article/details/gthbnhurg.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://blog.zdbjq.cn/Article/details/gzzkeahig.sHtML

Ruby: (0...10).step(2).to_a
来源：http://baike.hesvh.cn/Article/details/gncgukudn.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://wap.zdbjq.cn/Article/details/gblvdamxh.sHtML

[B12] 跳出多层循环
来源：http://www.m.share.hesvh.cn/Article/details/gvijcuwpi.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://wap.fehbvm.com/Article/details/gshlvfewb.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://blog.fehbvm.com/Article/details/gokduplcd.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.zdbjq.cn/Article/details/gvahfdyop.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://baike.hesvh.cn/Article/details/gxznhvruv.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://wap.fehbvm.com/Article/details/gbrvnufmp.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://baike.hesvh.cn/Article/details/gcqgujqcj.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://3g.fehbvm.com/Article/details/gadssudcf.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://wap.zdbjq.cn/Article/details/gpdzcpcjk.sHtML

[B13] 判断是否为数字
来源：http://3g.hesvh.cn/Article/details/gtiwsuwjb.sHtML

Py:   isinstance(x, (int, float))
来源：http://m.share.hesvh.cn/Article/details/gcdrpkdpg.sHtML

PHP:  is_numeric($x)
来源：http://www.share.fehbvm.com/Article/details/ghhkkrcip.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.fehbvm.com/Article/details/ghyoglbzx.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://blog.hesvh.cn/Article/details/gzqcdrifg.sHtML

Java: x instanceof Number
来源：http://m.share.zdbjq.cn/Article/details/gvwjicfte.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://read.share.zdbjq.cn/Article/details/giyksquud.sHtML

Ruby: x.is_a?(Numeric)
来源：http://wap.zdbjq.cn/Article/details/gmoozpsnq.sHtML

C#:   x is int or double or decimal
来源：http://read.share.hesvh.cn/Article/details/gjthdnvbj.sHtML

[B14] 判断值是否在集合内
来源：http://mobile.zdbjq.cn/Article/details/glvbjefky.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://wap.zdbjq.cn/Article/details/gmroclhfi.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://blog.hesvh.cn/Article/details/gvynqwpka.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://blog.hesvh.cn/Article/details/gqfyxpdvv.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://3g.zdbjq.cn/Article/details/ggyirkeit.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://m.share.zdbjq.cn/Article/details/gkjcnbsea.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://read.share.hesvh.cn/Article/details/gdyhgxoaz.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://baike.zdbjq.cn/Article/details/grjxeafyw.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.blog.hesvh.cn/Article/details/gzjmnbbui.sHtML

[B15] 布尔运算与取反
来源：http://wap.hesvh.cn/Article/details/gvkgxycmx.sHtML

Py:   a and b or not c
来源：http://baike.fehbvm.com/Article/details/ghsrmnolq.sHtML

PHP:  $a && $b || !$c
来源：http://3g.hesvh.cn/Article/details/gpdsnqfbe.sHtML

JS:   a && b || !c
来源：http://3g.hesvh.cn/Article/details/gpimondnd.sHtML

TS:   a && b || !c
来源：http://read.share.hesvh.cn/Article/details/gqpemlyhs.sHtML

Java: a && b || !c
来源：http://mobile.zdbjq.cn/Article/details/gjegxgzcu.sHtML

Go:   a && b || !c
来源：http://3g.fehbvm.com/Article/details/gmzfqixne.sHtML

Ruby: a && b || !c
来源：http://blog.hesvh.cn/Article/details/gxahyrxhl.sHtML

C#:   a && b || !c
来源：http://m.share.hesvh.cn/Article/details/gblgsswcz.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.m.share.hesvh.cn/Article/details/gzgpjganj.sHtML

Py:   if not data: return
来源：http://www.blog.zdbjq.cn/Article/details/gcqbknkyu.sHtML

PHP:  if (!$data) { return; }
来源：http://www.share.zdbjq.cn/Article/details/gkrrwkfuk.sHtML

JS:   if (!data) return;
来源：http://read.share.zdbjq.cn/Article/details/gqpnwxhaz.sHtML

TS:   if (!data) return;
来源：http://blog.zdbjq.cn/Article/details/gqjvuszgq.sHtML

Java: if (data == null) return;
来源：http://3g.hesvh.cn/Article/details/gwawwwdis.sHtML

Go:   if data == nil { return }
来源：http://m.share.fehbvm.com/Article/details/ghijgrnjw.sHtML

Ruby: return if data.nil?
来源：http://3g.hesvh.cn/Article/details/ggabjleex.sHtML

C#:   if (data == null) return;
来源：http://blog.hesvh.cn/Article/details/gvsubiuer.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/guubyprgr.sHtML

C. 函数与作用域
来源：http://baike.zdbjq.cn/Article/details/gvaccyzch.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gutgqawaq.sHtML

[C01] 定义函数
来源：http://www.share.hesvh.cn/Article/details/gejifvvaq.sHtML

Py:   def add(a, b): return a + b
来源：http://read.share.zdbjq.cn/Article/details/gspyaphuj.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.hesvh.cn/Article/details/ggtlruaxz.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://blog.hesvh.cn/Article/details/gtnquecyf.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.hesvh.cn/Article/details/gcfphucms.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://m.share.fehbvm.com/Article/details/gmtkrfwxl.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://wap.hesvh.cn/Article/details/grcuvytzt.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.share.fehbvm.com/Article/details/gbzsqhpqx.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://baike.hesvh.cn/Article/details/gqpvcolql.sHtML

[C02] 默认参数
来源：http://blog.hesvh.cn/Article/details/gtmtojbpe.sHtML

Py:   def greet(name="World"): return name
来源：http://3g.fehbvm.com/Article/details/gjqeesabz.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://mobile.zdbjq.cn/Article/details/gfhayuylk.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://wap.fehbvm.com/Article/details/gasqidxbn.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://3g.zdbjq.cn/Article/details/gmuvdutul.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://read.share.fehbvm.com/Article/details/gnlzkqejm.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.share.fehbvm.com/Article/details/gvvarukza.sHtML

Ruby: def greet(name = "World") = name
来源：http://m.share.fehbvm.com/Article/details/gfcqegotu.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://3g.zdbjq.cn/Article/details/gzdlcyoww.sHtML

[C03] 可变参数
来源：http://3g.hesvh.cn/Article/details/guzqcjvnw.sHtML

Py:   def total(*args): return sum(args)
来源：http://3g.zdbjq.cn/Article/details/gbvdqpbyl.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://3g.fehbvm.com/Article/details/gjharqfow.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.hesvh.cn/Article/details/gzzhwqfny.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.zdbjq.cn/Article/details/gdifpohbi.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://mobile.fehbvm.com/Article/details/gxbypfajc.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.share.hesvh.cn/Article/details/gmjvzeuiq.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://mobile.zdbjq.cn/Article/details/gmptdovlt.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://blog.zdbjq.cn/Article/details/gxvpzxqon.sHtML

[C04] 命名参数 / 关键字参数
来源：http://3g.hesvh.cn/Article/details/gnregiuds.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://baike.hesvh.cn/Article/details/gtfkjebrh.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.m.share.zdbjq.cn/Article/details/gieddffds.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.blog.fehbvm.com/Article/details/gpfoslkbu.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wap.zdbjq.cn/Article/details/gaeraljio.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://baike.hesvh.cn/Article/details/guyfqjfjo.sHtML

Go:   // 无：用配置结构体参数
来源：http://blog.fehbvm.com/Article/details/guohefnqp.sHtML

Ruby: f(a: 1, b: 2)
来源：http://mobile.zdbjq.cn/Article/details/gkyylatox.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.share.hesvh.cn/Article/details/gvdnvwkwp.sHtML

[C05] 返回多个值
来源：http://www.share.zdbjq.cn/Article/details/goalfyzdr.sHtML

Py:   return a, b
来源：http://www.blog.hesvh.cn/Article/details/ggwovxafy.sHtML

PHP:  return [$a, $b];
来源：http://wap.zdbjq.cn/Article/details/gktfzpedn.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://read.share.zdbjq.cn/Article/details/gwndszxni.sHtML

TS:   return { a, b };
来源：http://www.share.zdbjq.cn/Article/details/ghpmllqfn.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://blog.zdbjq.cn/Article/details/gvqoootkj.sHtML

Go:   return a, b
来源：http://www.m.share.zdbjq.cn/Article/details/grevlfeti.sHtML

Ruby: return a, b
来源：http://baike.hesvh.cn/Article/details/gikwykebh.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.blog.zdbjq.cn/Article/details/gmsuylplo.sHtML

[C06] 匿名函数 / lambda
来源：http://www.share.hesvh.cn/Article/details/gcsfnhgpn.sHtML

Py:   square = lambda x: x * x
来源：http://mobile.hesvh.cn/Article/details/gqwuuzkgn.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://read.share.fehbvm.com/Article/details/gjbynuvob.sHtML

JS:   const square = x => x * x;
来源：http://wap.zdbjq.cn/Article/details/gtitbivdp.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://baike.hesvh.cn/Article/details/gfsewupak.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://read.share.fehbvm.com/Article/details/guhngyznk.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://wap.hesvh.cn/Article/details/grgzcskki.sHtML

Ruby: square = ->(x) { x * x }
来源：http://m.share.hesvh.cn/Article/details/gpvzudwfo.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://baike.hesvh.cn/Article/details/gssujolxq.sHtML

[C07] 把函数作为参数传入
来源：http://3g.hesvh.cn/Article/details/gxvcxmugh.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://m.share.zdbjq.cn/Article/details/gdjvjgdsf.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.share.zdbjq.cn/Article/details/gsylxtfek.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://baike.fehbvm.com/Article/details/gmpixkeze.sHtML

TS:   arr.map(String)
来源：http://read.share.fehbvm.com/Article/details/guwbajrvd.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://m.share.hesvh.cn/Article/details/ghllvxlho.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.share.hesvh.cn/Article/details/gjwborfob.sHtML

Ruby: arr.map(&:upcase)
来源：http://wap.zdbjq.cn/Article/details/gwhedaurj.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.blog.zdbjq.cn/Article/details/ghttujbyj.sHtML

[C08] 闭包
来源：http://wap.hesvh.cn/Article/details/grbsbbjxq.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://3g.hesvh.cn/Article/details/gakxlcbrf.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://blog.fehbvm.com/Article/details/gpjxbhdyl.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.blog.zdbjq.cn/Article/details/gnkqaamxj.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://mobile.hesvh.cn/Article/details/gghdrlfzh.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://wap.zdbjq.cn/Article/details/gtbiwxgtv.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://mobile.fehbvm.com/Article/details/gtupxnqzk.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.share.hesvh.cn/Article/details/gicbanncx.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://blog.fehbvm.com/Article/details/gzloszsqt.sHtML

[C09] 递归
来源：http://mobile.fehbvm.com/Article/details/gxuxniwyt.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.share.zdbjq.cn/Article/details/gwwwuwtna.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://mobile.zdbjq.cn/Article/details/guaaxyoxd.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.fehbvm.com/Article/details/ghsskdfas.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.hesvh.cn/Article/details/gejjysfqi.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.blog.zdbjq.cn/Article/details/galkowsud.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.m.share.fehbvm.com/Article/details/gaktxichg.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mobile.fehbvm.com/Article/details/gfyyruqfd.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://baike.hesvh.cn/Article/details/gkxdtxdkb.sHtML

[C10] 变量作用域
来源：http://www.m.share.zdbjq.cn/Article/details/geoxglfvu.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://read.share.hesvh.cn/Article/details/gigzkjgtk.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mobile.fehbvm.com/Article/details/gmmunxspz.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://read.share.hesvh.cn/Article/details/gpobswond.sHtML

TS:   同 JS
来源：http://blog.zdbjq.cn/Article/details/guqyypsnw.sHtML

Java: 方法内为块级作用域
来源：http://m.share.zdbjq.cn/Article/details/gnmifjgkc.sHtML

Go:   花括号块级作用域
来源：http://www.m.share.fehbvm.com/Article/details/gzwfzvhzl.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://baike.zdbjq.cn/Article/details/gdqjcrtmm.sHtML

C#:   块级作用域
来源：http://read.share.zdbjq.cn/Article/details/gddgqjkwz.sHtML

[C11] 模块导入与导出
来源：http://www.m.share.hesvh.cn/Article/details/gvzgmiiqu.sHtML

Py:   from module import func
来源：http://blog.fehbvm.com/Article/details/ggbkmqiqo.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.share.hesvh.cn/Article/details/gyyololqi.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.m.share.zdbjq.cn/Article/details/gzbwbivvh.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.m.share.hesvh.cn/Article/details/gorfgqxib.sHtML

Java: import java.util.List;
来源：http://m.share.fehbvm.com/Article/details/gchpmjakq.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.m.share.fehbvm.com/Article/details/ghzwbroyr.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://3g.hesvh.cn/Article/details/gvcemhgyi.sHtML

C#:   using System.Text;
来源：http://www.blog.fehbvm.com/Article/details/gzundelpx.sHtML

[C12] 立即执行函数 IIFE
来源：http://wap.zdbjq.cn/Article/details/grwfbqltq.sHtML

Py:   (lambda: print("run"))()
来源：http://www.m.share.zdbjq.cn/Article/details/getheitcn.sHtML

PHP:  (function () { echo "run"; })();
来源：http://mobile.fehbvm.com/Article/details/gudwpsnxq.sHtML

JS:   (() => { console.log("run"); })();
来源：http://baike.hesvh.cn/Article/details/gaynkfswq.sHtML

TS:   (() => { console.log("run"); })();
来源：http://baike.hesvh.cn/Article/details/gkygztccz.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wap.hesvh.cn/Article/details/gupvlubfp.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://mobile.zdbjq.cn/Article/details/giktiaaby.sHtML

Ruby: -> { puts "run" }.call
来源：http://blog.fehbvm.com/Article/details/gtfsxoqfz.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://m.share.zdbjq.cn/Article/details/gqgoekfif.sHtML

[C13] 类型声明 / 类型注解
来源：http://blog.zdbjq.cn/Article/details/gcspmvbtw.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.m.share.zdbjq.cn/Article/details/gwoqeqyqz.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.hesvh.cn/Article/details/gluoppuiv.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.share.fehbvm.com/Article/details/gmbilubfr.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.hesvh.cn/Article/details/gkpupreau.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://baike.zdbjq.cn/Article/details/gcbociobw.sHtML

Go:   func add(a, b int) int
来源：http://read.share.hesvh.cn/Article/details/gicgniduz.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://blog.hesvh.cn/Article/details/guqozhuhi.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://3g.zdbjq.cn/Article/details/gtasbxjed.sHtML

[C14] 泛型函数
来源：http://wap.hesvh.cn/Article/details/gazmnpibk.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.share.fehbvm.com/Article/details/gfmhwhkme.sHtML

PHP:  // 无泛型
来源：http://baike.hesvh.cn/Article/details/gwgwlfgrq.sHtML

JS:   // 无泛型
来源：http://www.share.fehbvm.com/Article/details/gdbdazacl.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://read.share.fehbvm.com/Article/details/ghuenlbca.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://3g.fehbvm.com/Article/details/gngqkkgdn.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.share.zdbjq.cn/Article/details/gzxvlbyga.sHtML

Ruby: # 无泛型
来源：http://baike.hesvh.cn/Article/details/ggauvbivf.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.share.zdbjq.cn/Article/details/gtyqdfrys.sHtML

[C15] 解构 / 展开参数
来源：http://m.share.zdbjq.cn/Article/details/gloucteit.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://mobile.zdbjq.cn/Article/details/goisaorgz.sHtML

PHP:  [$a, $b] = $pair;
来源：http://read.share.hesvh.cn/Article/details/glgoujggk.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.share.fehbvm.com/Article/details/gsqbnbacm.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.blog.hesvh.cn/Article/details/ghbxztmup.sHtML

Java: // 无解构
来源：http://m.share.fehbvm.com/Article/details/gquhiepxs.sHtML

Go:   // 无解构
来源：http://mobile.hesvh.cn/Article/details/gpwbeedxm.sHtML

Ruby: a, b = pair
来源：http://www.share.hesvh.cn/Article/details/gmzudlgwd.sHtML

C#:   var (a, b) = pair;
来源：http://read.share.hesvh.cn/Article/details/gyrwhzntd.sHtML

[C16] 函数 / 方法重载
来源：http://www.share.zdbjq.cn/Article/details/ggyrvzkmx.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.share.zdbjq.cn/Article/details/grmvbeefe.sHtML

PHP:  // 无重载
来源：http://wap.fehbvm.com/Article/details/gbstcjuld.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.share.zdbjq.cn/Article/details/gjtqhxvpl.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://mobile.zdbjq.cn/Article/details/guzkcohop.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://wap.fehbvm.com/Article/details/gjfaaawzs.sHtML

Go:   // 无重载：用不同函数名
来源：http://wap.hesvh.cn/Article/details/gqfmtbctb.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.m.share.fehbvm.com/Article/details/galfdnznu.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://baike.zdbjq.cn/Article/details/gdlpfioil.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gchwrgetw.sHtML

D. 数组 / 列表 / 集合
来源：http://m.share.zdbjq.cn/Article/details/gcihtllxp.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gvitkivze.sHtML

[D01] 创建数组 / 列表
来源：http://3g.zdbjq.cn/Article/details/gccgmlaxr.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://wap.zdbjq.cn/Article/details/gkjfexhhs.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://m.share.zdbjq.cn/Article/details/gowvktbrp.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://baike.zdbjq.cn/Article/details/gpzqaylhg.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.m.share.zdbjq.cn/Article/details/gklppunxm.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mobile.zdbjq.cn/Article/details/gpnizozfa.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.blog.zdbjq.cn/Article/details/gxcxuyajo.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.m.share.zdbjq.cn/Article/details/giyztcixc.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://blog.hesvh.cn/Article/details/gfoxsobrg.sHtML

[D02] 追加元素到末尾
来源：http://www.m.share.zdbjq.cn/Article/details/giqflzqqy.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wap.hesvh.cn/Article/details/gsljnwfut.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.m.share.zdbjq.cn/Article/details/gdvhwrtfs.sHtML

JS:   arr.push(4);
来源：http://blog.zdbjq.cn/Article/details/gnayhniyt.sHtML

TS:   arr.push(4);
来源：http://www.m.share.zdbjq.cn/Article/details/gzcxhgkbs.sHtML

Java: list.add(4);
来源：http://mobile.fehbvm.com/Article/details/gvmgwbxfz.sHtML

Go:   arr = append(arr, 4)
来源：http://read.share.fehbvm.com/Article/details/gzctulyso.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://3g.zdbjq.cn/Article/details/gxwzzuxth.sHtML

C#:   list.Add(4);
来源：http://read.share.fehbvm.com/Article/details/gnxoadcis.sHtML

[D03] 在指定位置插入元素
来源：http://www.share.hesvh.cn/Article/details/girmwnpio.sHtML

Py:   arr.insert(0, 0)
来源：http://mobile.zdbjq.cn/Article/details/gcbzdbcbg.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://blog.hesvh.cn/Article/details/girrkkpub.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wap.hesvh.cn/Article/details/gwdniedsw.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://baike.fehbvm.com/Article/details/gqzazwypg.sHtML

Java: list.add(0, 0);
来源：http://3g.hesvh.cn/Article/details/gekqwmysv.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://wap.zdbjq.cn/Article/details/gsnrzbukr.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://blog.hesvh.cn/Article/details/gnmdhzspe.sHtML

C#:   list.Insert(0, 0);
来源：http://blog.fehbvm.com/Article/details/gydyngaef.sHtML

[D04] 删除元素
来源：http://baike.zdbjq.cn/Article/details/gfhwqfebm.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://baike.zdbjq.cn/Article/details/gyqpibabz.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.blog.fehbvm.com/Article/details/gonkmiqxt.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.m.share.fehbvm.com/Article/details/gblgxunpy.sHtML

TS:   arr.splice(0, 1);
来源：http://www.blog.hesvh.cn/Article/details/gkwpdicqu.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.blog.fehbvm.com/Article/details/glextkuyh.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.blog.zdbjq.cn/Article/details/gxxnkgmra.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://3g.fehbvm.com/Article/details/gyxtngcfe.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://m.share.zdbjq.cn/Article/details/gympswwks.sHtML

[D05] 访问与修改元素
来源：http://read.share.fehbvm.com/Article/details/gmpzmbaby.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.fehbvm.com/Article/details/gwcfxaefb.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://blog.fehbvm.com/Article/details/gphbdxeiq.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.m.share.zdbjq.cn/Article/details/gztyurjzj.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://baike.zdbjq.cn/Article/details/gyrxajezg.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://3g.hesvh.cn/Article/details/gzwfeczuw.sHtML


<!-- 参考信息 -->