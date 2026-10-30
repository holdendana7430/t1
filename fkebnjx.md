代发 wailian999

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://mobile.zdbjq.cn/Article/details/gwdqspnzq.sHtML

[B06] 遍历字典 / 对象
来源：http://read.share.zdbjq.cn/Article/details/ggyxnhrbx.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.share.zdbjq.cn/Article/details/glpbrpkie.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://read.share.zdbjq.cn/Article/details/gupfknoeh.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://baike.fehbvm.com/Article/details/gwjayzxxe.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.m.share.fehbvm.com/Article/details/glbisxjuk.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://read.share.zdbjq.cn/Article/details/gwxbtkzkb.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.share.fehbvm.com/Article/details/gbwrfrxtq.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://read.share.zdbjq.cn/Article/details/ghqzmflal.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://mobile.zdbjq.cn/Article/details/gjwjokxdn.sHtML

[B07] while 循环
来源：http://m.share.hesvh.cn/Article/details/gotikzdtx.sHtML

Py:   while i < 10: i += 1
来源：http://baike.zdbjq.cn/Article/details/gcjkwxmyc.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.m.share.hesvh.cn/Article/details/gnxfimgif.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.m.share.hesvh.cn/Article/details/gzpyjfmia.sHtML

TS:   while (i < 10) { i++; }
来源：http://m.share.hesvh.cn/Article/details/gvuyixtix.sHtML

Java: while (i < 10) { i++; }
来源：http://www.blog.hesvh.cn/Article/details/gnbrufogm.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://wap.fehbvm.com/Article/details/gnwpufjta.sHtML

Ruby: while i < 10; i += 1; end
来源：http://3g.fehbvm.com/Article/details/gopqmxvzn.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.blog.zdbjq.cn/Article/details/glvnshsvm.sHtML

[B08] do-while（至少执行一次）
来源：http://wap.hesvh.cn/Article/details/gfcyeskmy.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.m.share.fehbvm.com/Article/details/gyeusalkr.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.share.hesvh.cn/Article/details/gkwwarqur.sHtML

JS:   do { i++; } while (i < 10);
来源：http://m.share.hesvh.cn/Article/details/gcattrvsl.sHtML

TS:   do { i++; } while (i < 10);
来源：http://mobile.fehbvm.com/Article/details/gkizmpthj.sHtML

Java: do { i++; } while (i < 10);
来源：http://m.share.zdbjq.cn/Article/details/gzshosbix.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://baike.fehbvm.com/Article/details/gqrotunlq.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://mobile.fehbvm.com/Article/details/ggjbahkwj.sHtML

C#:   do { i++; } while (i < 10);
来源：http://m.share.zdbjq.cn/Article/details/gnpyfzdpx.sHtML

[B09] break 与 continue
来源：http://read.share.hesvh.cn/Article/details/gksekjdbb.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://baike.zdbjq.cn/Article/details/gomkrfffe.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://3g.zdbjq.cn/Article/details/gnocwpbrd.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.hesvh.cn/Article/details/gvdlbbwnw.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.fehbvm.com/Article/details/gdakhygqx.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.zdbjq.cn/Article/details/gzegutsvb.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.share.hesvh.cn/Article/details/gfufigrjr.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://m.share.zdbjq.cn/Article/details/gvywkwxwr.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.fehbvm.com/Article/details/gluypefqk.sHtML

[B10] 遍历同时拿索引
来源：http://baike.zdbjq.cn/Article/details/gyzajjfrb.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://blog.zdbjq.cn/Article/details/guvkvgrzl.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://blog.fehbvm.com/Article/details/gapnvinaf.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://3g.zdbjq.cn/Article/details/gdwtinhvp.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://m.share.zdbjq.cn/Article/details/gfzdbopig.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.m.share.hesvh.cn/Article/details/gtwwofyjb.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://wap.hesvh.cn/Article/details/grbhwiqzj.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.m.share.zdbjq.cn/Article/details/gkrrmwtgz.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://m.share.zdbjq.cn/Article/details/gfhtaqfmg.sHtML

[B11] 生成数字序列 / 区间
来源：http://read.share.zdbjq.cn/Article/details/giwwyzhec.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.blog.hesvh.cn/Article/details/gjvvatmop.sHtML

PHP:  range(0, 10, 2);
来源：http://wap.fehbvm.com/Article/details/gbycqprbf.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.fehbvm.com/Article/details/grncdmman.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://read.share.zdbjq.cn/Article/details/gadhbqbwh.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://wap.fehbvm.com/Article/details/gqfstmixq.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://blog.fehbvm.com/Article/details/ggkxouibi.sHtML

Ruby: (0...10).step(2).to_a
来源：http://read.share.hesvh.cn/Article/details/gksuzvxow.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://baike.hesvh.cn/Article/details/giyagcvli.sHtML

[B12] 跳出多层循环
来源：http://m.share.fehbvm.com/Article/details/gliihtxgh.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.share.hesvh.cn/Article/details/ghetehzzo.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://read.share.fehbvm.com/Article/details/gwkixdpja.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.fehbvm.com/Article/details/gzmsbpqxs.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.fehbvm.com/Article/details/gxwibyhvn.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://blog.fehbvm.com/Article/details/gbuirleyr.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://3g.zdbjq.cn/Article/details/guvjkjitl.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.share.fehbvm.com/Article/details/gtardvflq.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://mobile.zdbjq.cn/Article/details/ggtbwvszs.sHtML

[B13] 判断是否为数字
来源：http://m.share.zdbjq.cn/Article/details/gzlzvsyfg.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.blog.hesvh.cn/Article/details/grmdjgmzc.sHtML

PHP:  is_numeric($x)
来源：http://blog.zdbjq.cn/Article/details/gwcazvfoj.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.zdbjq.cn/Article/details/gjcjoeiab.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.fehbvm.com/Article/details/guchmgzja.sHtML

Java: x instanceof Number
来源：http://baike.zdbjq.cn/Article/details/gwrodliun.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.share.fehbvm.com/Article/details/gvfllgbht.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.blog.zdbjq.cn/Article/details/gpbqrkbet.sHtML

C#:   x is int or double or decimal
来源：http://read.share.zdbjq.cn/Article/details/gvatorgij.sHtML

[B14] 判断值是否在集合内
来源：http://baike.zdbjq.cn/Article/details/gvpwrekec.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://read.share.fehbvm.com/Article/details/grwuqaipk.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.blog.fehbvm.com/Article/details/gesgaahih.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://wap.zdbjq.cn/Article/details/gdfiisuoq.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://read.share.fehbvm.com/Article/details/gaeukllrm.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://m.share.hesvh.cn/Article/details/gykxukghn.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://3g.zdbjq.cn/Article/details/gnodlmrqw.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gfftgbhmr.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.share.fehbvm.com/Article/details/ghyvlcblq.sHtML

[B15] 布尔运算与取反
来源：http://read.share.hesvh.cn/Article/details/ghfeljgat.sHtML

Py:   a and b or not c
来源：http://www.blog.fehbvm.com/Article/details/ghkawwnej.sHtML

PHP:  $a && $b || !$c
来源：http://www.share.fehbvm.com/Article/details/gfyxsqdsw.sHtML

JS:   a && b || !c
来源：http://read.share.hesvh.cn/Article/details/gcphznmek.sHtML

TS:   a && b || !c
来源：http://blog.hesvh.cn/Article/details/gznrfoaav.sHtML

Java: a && b || !c
来源：http://blog.fehbvm.com/Article/details/gqtnjxtev.sHtML

Go:   a && b || !c
来源：http://www.m.share.fehbvm.com/Article/details/gglkftcfr.sHtML

Ruby: a && b || !c
来源：http://mobile.zdbjq.cn/Article/details/gtydelpjk.sHtML

C#:   a && b || !c
来源：http://3g.fehbvm.com/Article/details/gadinznak.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://mobile.hesvh.cn/Article/details/gfhoagxin.sHtML

Py:   if not data: return
来源：http://wap.zdbjq.cn/Article/details/gokhrwqnj.sHtML

PHP:  if (!$data) { return; }
来源：http://read.share.fehbvm.com/Article/details/gjzevllay.sHtML

JS:   if (!data) return;
来源：http://baike.zdbjq.cn/Article/details/gajvqlwfc.sHtML

TS:   if (!data) return;
来源：http://mobile.fehbvm.com/Article/details/gqgwhmlnu.sHtML

Java: if (data == null) return;
来源：http://wap.fehbvm.com/Article/details/gyzabfvll.sHtML

Go:   if data == nil { return }
来源：http://www.blog.fehbvm.com/Article/details/grtmoiyou.sHtML

Ruby: return if data.nil?
来源：http://wap.hesvh.cn/Article/details/guannhypb.sHtML

C#:   if (data == null) return;
来源：http://mobile.zdbjq.cn/Article/details/ghgcqcikc.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gybycecui.sHtML

C. 函数与作用域
来源：http://www.share.hesvh.cn/Article/details/gwlurekfk.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gauwufdrk.sHtML

[C01] 定义函数
来源：http://www.blog.fehbvm.com/Article/details/gfcecsmav.sHtML

Py:   def add(a, b): return a + b
来源：http://m.share.hesvh.cn/Article/details/glweiupqz.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.hesvh.cn/Article/details/gbpbigjtn.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://wap.hesvh.cn/Article/details/giivburxz.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.hesvh.cn/Article/details/glflscrct.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.blog.fehbvm.com/Article/details/gzinifkzz.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.share.fehbvm.com/Article/details/gyhmsgkwj.sHtML

Ruby: def add(a, b); a + b; end
来源：http://baike.fehbvm.com/Article/details/gfmuaarra.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://wap.fehbvm.com/Article/details/gmqtxoojl.sHtML

[C02] 默认参数
来源：http://mobile.zdbjq.cn/Article/details/gufjygsvk.sHtML

Py:   def greet(name="World"): return name
来源：http://mobile.zdbjq.cn/Article/details/gewgdodim.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://m.share.zdbjq.cn/Article/details/grnpwasvd.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://baike.zdbjq.cn/Article/details/gbwztwozy.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.blog.hesvh.cn/Article/details/gpeptylud.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://wap.fehbvm.com/Article/details/gaadpzvqn.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://mobile.hesvh.cn/Article/details/grcajudpa.sHtML

Ruby: def greet(name = "World") = name
来源：http://blog.fehbvm.com/Article/details/guvfzdwop.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://blog.fehbvm.com/Article/details/gtjlvsywo.sHtML

[C03] 可变参数
来源：http://read.share.zdbjq.cn/Article/details/gzhuddngr.sHtML

Py:   def total(*args): return sum(args)
来源：http://m.share.hesvh.cn/Article/details/gdjvzjpnj.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://mobile.fehbvm.com/Article/details/gfrhvebgd.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.fehbvm.com/Article/details/gdodhqfmy.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.zdbjq.cn/Article/details/glfuprkkj.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://blog.fehbvm.com/Article/details/gofavfmaq.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.blog.zdbjq.cn/Article/details/gfisskamj.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://blog.fehbvm.com/Article/details/gmebomoxr.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://blog.fehbvm.com/Article/details/geldtkmiu.sHtML

[C04] 命名参数 / 关键字参数
来源：http://mobile.zdbjq.cn/Article/details/gsjkzwpqu.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://mobile.zdbjq.cn/Article/details/grzewrsoo.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://wap.zdbjq.cn/Article/details/gnskxjvug.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.blog.zdbjq.cn/Article/details/gpfatkiik.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://baike.zdbjq.cn/Article/details/gkdtomfxk.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://mobile.hesvh.cn/Article/details/glontaocf.sHtML

Go:   // 无：用配置结构体参数
来源：http://3g.hesvh.cn/Article/details/gpfeumcat.sHtML

Ruby: f(a: 1, b: 2)
来源：http://blog.hesvh.cn/Article/details/gmawadcbz.sHtML

C#:   f(a: 1, b: 2)
来源：http://mobile.fehbvm.com/Article/details/gmgetajmn.sHtML

[C05] 返回多个值
来源：http://blog.zdbjq.cn/Article/details/ggsulwsus.sHtML

Py:   return a, b
来源：http://www.share.zdbjq.cn/Article/details/gxjqbdarl.sHtML

PHP:  return [$a, $b];
来源：http://wap.fehbvm.com/Article/details/ggyxtklxr.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://read.share.zdbjq.cn/Article/details/gapbqojtq.sHtML

TS:   return { a, b };
来源：http://www.m.share.zdbjq.cn/Article/details/gbmoeixfi.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://blog.hesvh.cn/Article/details/gzcymqnil.sHtML

Go:   return a, b
来源：http://3g.fehbvm.com/Article/details/gdjrjpfhq.sHtML

Ruby: return a, b
来源：http://blog.hesvh.cn/Article/details/ggqehxafm.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://read.share.fehbvm.com/Article/details/gpxsucbiz.sHtML

[C06] 匿名函数 / lambda
来源：http://m.share.zdbjq.cn/Article/details/gliputsmq.sHtML

Py:   square = lambda x: x * x
来源：http://baike.hesvh.cn/Article/details/gbuvtpxij.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://blog.zdbjq.cn/Article/details/gshzflrue.sHtML

JS:   const square = x => x * x;
来源：http://blog.fehbvm.com/Article/details/gmehdaded.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.blog.zdbjq.cn/Article/details/gtmlnimeg.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://wap.zdbjq.cn/Article/details/gsrlkfydj.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://mobile.fehbvm.com/Article/details/gnalhmfqj.sHtML

Ruby: square = ->(x) { x * x }
来源：http://3g.zdbjq.cn/Article/details/grpqqfsev.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.blog.hesvh.cn/Article/details/gywhfgpqw.sHtML

[C07] 把函数作为参数传入
来源：http://www.share.zdbjq.cn/Article/details/gyuovkpag.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.share.hesvh.cn/Article/details/gabpxcebv.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://mobile.fehbvm.com/Article/details/gumcvpetz.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://mobile.hesvh.cn/Article/details/gkxcvxvmz.sHtML

TS:   arr.map(String)
来源：http://www.blog.hesvh.cn/Article/details/gcpfmslyg.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://wap.hesvh.cn/Article/details/gpqmsrwho.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://m.share.hesvh.cn/Article/details/glsxbrhvb.sHtML

Ruby: arr.map(&:upcase)
来源：http://blog.zdbjq.cn/Article/details/gzdnlixsj.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.m.share.hesvh.cn/Article/details/gcvsmpxac.sHtML

[C08] 闭包
来源：http://read.share.hesvh.cn/Article/details/gqrrxgrxs.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://m.share.hesvh.cn/Article/details/ghsdbdvod.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://wap.fehbvm.com/Article/details/gxtdyezjq.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://blog.fehbvm.com/Article/details/gsjqxttsa.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://baike.zdbjq.cn/Article/details/gvbqjgmfl.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.m.share.fehbvm.com/Article/details/guzgepxzx.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.share.zdbjq.cn/Article/details/gsgyogrwu.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://3g.fehbvm.com/Article/details/gjcountik.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://3g.fehbvm.com/Article/details/gwmtjxcjk.sHtML

[C09] 递归
来源：http://www.share.hesvh.cn/Article/details/gteqydiji.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://baike.fehbvm.com/Article/details/gphakwgvs.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://mobile.fehbvm.com/Article/details/gufvfyufg.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.zdbjq.cn/Article/details/gpdjvbcvd.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.fehbvm.com/Article/details/gfxajbiso.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://3g.hesvh.cn/Article/details/glcyxotmb.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://blog.zdbjq.cn/Article/details/glvusqdrs.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.share.hesvh.cn/Article/details/gwnswondt.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.m.share.zdbjq.cn/Article/details/gcqjvzydl.sHtML

[C10] 变量作用域
来源：http://blog.zdbjq.cn/Article/details/gtcdhdvou.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://3g.fehbvm.com/Article/details/gffdklkzh.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mobile.hesvh.cn/Article/details/gtzidnzjg.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://mobile.fehbvm.com/Article/details/gqsolufjb.sHtML

TS:   同 JS
来源：http://m.share.hesvh.cn/Article/details/guuknlhrk.sHtML

Java: 方法内为块级作用域
来源：http://m.share.fehbvm.com/Article/details/gabdolcbh.sHtML

Go:   花括号块级作用域
来源：http://3g.hesvh.cn/Article/details/gdzmateeb.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://m.share.hesvh.cn/Article/details/gwuszjykh.sHtML

C#:   块级作用域
来源：http://mobile.hesvh.cn/Article/details/gkkjqepox.sHtML

[C11] 模块导入与导出
来源：http://www.m.share.zdbjq.cn/Article/details/gjoqdvzxw.sHtML

Py:   from module import func
来源：http://baike.hesvh.cn/Article/details/gbzqbxkmx.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://baike.hesvh.cn/Article/details/gsagswdeo.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://mobile.fehbvm.com/Article/details/ggfzqvitf.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://mobile.fehbvm.com/Article/details/gytvhuppn.sHtML

Java: import java.util.List;
来源：http://baike.zdbjq.cn/Article/details/gmmyewybs.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://wap.fehbvm.com/Article/details/gnmrrgenh.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.share.zdbjq.cn/Article/details/gwngwpycn.sHtML

C#:   using System.Text;
来源：http://mobile.hesvh.cn/Article/details/gplfrvgto.sHtML

[C12] 立即执行函数 IIFE
来源：http://blog.fehbvm.com/Article/details/gjhhxwdvk.sHtML

Py:   (lambda: print("run"))()
来源：http://www.blog.zdbjq.cn/Article/details/gmufwsemc.sHtML

PHP:  (function () { echo "run"; })();
来源：http://m.share.zdbjq.cn/Article/details/gsgbxmtuq.sHtML

JS:   (() => { console.log("run"); })();
来源：http://3g.hesvh.cn/Article/details/glsaaapxi.sHtML

TS:   (() => { console.log("run"); })();
来源：http://blog.fehbvm.com/Article/details/gzforfshw.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://mobile.fehbvm.com/Article/details/gboffeubv.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://blog.hesvh.cn/Article/details/gdoknmuvk.sHtML

Ruby: -> { puts "run" }.call
来源：http://mobile.hesvh.cn/Article/details/gnfnbbqss.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://read.share.zdbjq.cn/Article/details/gohjhdbng.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.share.zdbjq.cn/Article/details/gdjcsdnvj.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://read.share.hesvh.cn/Article/details/gepzysmqq.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.zdbjq.cn/Article/details/gokbdbbxh.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://3g.zdbjq.cn/Article/details/gwssmonqr.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.fehbvm.com/Article/details/gafczqbmb.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.share.zdbjq.cn/Article/details/ghjywbxhh.sHtML

Go:   func add(a, b int) int
来源：http://www.share.fehbvm.com/Article/details/gmklvtzma.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.share.fehbvm.com/Article/details/gqgiirhbj.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.blog.zdbjq.cn/Article/details/gjbexfcrs.sHtML

[C14] 泛型函数
来源：http://3g.hesvh.cn/Article/details/gvwcnuoxd.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://m.share.zdbjq.cn/Article/details/gwwzliwjy.sHtML

PHP:  // 无泛型
来源：http://mobile.hesvh.cn/Article/details/goucyuuim.sHtML

JS:   // 无泛型
来源：http://www.m.share.hesvh.cn/Article/details/gomnhukef.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://blog.zdbjq.cn/Article/details/gbklprfjp.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://mobile.hesvh.cn/Article/details/gfzhznxzl.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://blog.zdbjq.cn/Article/details/gorkggceg.sHtML

Ruby: # 无泛型
来源：http://www.blog.zdbjq.cn/Article/details/gcsibqylf.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://blog.zdbjq.cn/Article/details/gemmmvpbt.sHtML

[C15] 解构 / 展开参数
来源：http://read.share.zdbjq.cn/Article/details/gvwgjawwn.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.share.hesvh.cn/Article/details/gtkvluxdj.sHtML

PHP:  [$a, $b] = $pair;
来源：http://read.share.hesvh.cn/Article/details/guizrihbw.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.share.hesvh.cn/Article/details/gtgyhdxvz.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://blog.fehbvm.com/Article/details/gbjcvthen.sHtML

Java: // 无解构
来源：http://www.share.hesvh.cn/Article/details/gcplsmzlk.sHtML

Go:   // 无解构
来源：http://www.share.hesvh.cn/Article/details/gnzueusid.sHtML

Ruby: a, b = pair
来源：http://m.share.hesvh.cn/Article/details/gaenjymul.sHtML

C#:   var (a, b) = pair;
来源：http://baike.zdbjq.cn/Article/details/grbnkjdmd.sHtML

[C16] 函数 / 方法重载
来源：http://3g.hesvh.cn/Article/details/gloyakrrc.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://read.share.fehbvm.com/Article/details/glmcnaowp.sHtML

PHP:  // 无重载
来源：http://wap.zdbjq.cn/Article/details/gqisrddog.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.m.share.zdbjq.cn/Article/details/gzmvqcmvk.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://blog.zdbjq.cn/Article/details/gkmphpqcv.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://blog.fehbvm.com/Article/details/ggcuraksp.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.share.zdbjq.cn/Article/details/gwhhryoxn.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.blog.zdbjq.cn/Article/details/gtqlyhpua.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://mobile.fehbvm.com/Article/details/gmyujiqok.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gjamrfzny.sHtML

D. 数组 / 列表 / 集合
来源：http://wap.fehbvm.com/Article/details/glwygzdqa.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gdhqzgdnr.sHtML

[D01] 创建数组 / 列表
来源：http://mobile.fehbvm.com/Article/details/grprrczxc.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://3g.fehbvm.com/Article/details/gnlsubbjj.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://wap.zdbjq.cn/Article/details/glpodxbvt.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://3g.fehbvm.com/Article/details/gislfptpu.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.blog.zdbjq.cn/Article/details/gdiyfczla.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.blog.fehbvm.com/Article/details/gfjkwlqxr.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://m.share.fehbvm.com/Article/details/ghvlpoorw.sHtML

Ruby: arr = [1, 2, 3]
来源：http://wap.hesvh.cn/Article/details/gvjvxbyyc.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://blog.hesvh.cn/Article/details/gzqhgdvrs.sHtML

[D02] 追加元素到末尾
来源：http://www.share.zdbjq.cn/Article/details/grfzlfxyz.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://m.share.hesvh.cn/Article/details/giyyhxqef.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.m.share.hesvh.cn/Article/details/gizxvizwf.sHtML

JS:   arr.push(4);
来源：http://blog.zdbjq.cn/Article/details/gahzlyhzi.sHtML

TS:   arr.push(4);
来源：http://www.m.share.hesvh.cn/Article/details/gtighqago.sHtML

Java: list.add(4);
来源：http://read.share.fehbvm.com/Article/details/ggebwngie.sHtML

Go:   arr = append(arr, 4)
来源：http://www.blog.zdbjq.cn/Article/details/gwuhoyhxo.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://m.share.fehbvm.com/Article/details/gnlwtrglu.sHtML

C#:   list.Add(4);
来源：http://wap.hesvh.cn/Article/details/gxcyzvrna.sHtML

[D03] 在指定位置插入元素
来源：http://www.blog.zdbjq.cn/Article/details/geoxvrsao.sHtML

Py:   arr.insert(0, 0)
来源：http://mobile.zdbjq.cn/Article/details/giseemdam.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://3g.zdbjq.cn/Article/details/gmqwavlrs.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://m.share.fehbvm.com/Article/details/gpdbfbmej.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.m.share.hesvh.cn/Article/details/ggnaqdtyp.sHtML

Java: list.add(0, 0);
来源：http://www.m.share.hesvh.cn/Article/details/ggfvndcyk.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://mobile.zdbjq.cn/Article/details/ghnrnhswu.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.blog.zdbjq.cn/Article/details/gxfdwmulv.sHtML

C#:   list.Insert(0, 0);
来源：http://www.share.zdbjq.cn/Article/details/gfadytktq.sHtML

[D04] 删除元素
来源：http://3g.hesvh.cn/Article/details/gsgkmvndk.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mobile.hesvh.cn/Article/details/grylncndw.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://baike.hesvh.cn/Article/details/gnkzceyzk.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://baike.hesvh.cn/Article/details/gqwowzgyx.sHtML

TS:   arr.splice(0, 1);
来源：http://baike.hesvh.cn/Article/details/geownmgnr.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.share.hesvh.cn/Article/details/ghqzldrec.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.blog.fehbvm.com/Article/details/gmgrlafoz.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mobile.fehbvm.com/Article/details/gpzavwjdl.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://read.share.fehbvm.com/Article/details/gurklggho.sHtML

[D05] 访问与修改元素
来源：http://mobile.hesvh.cn/Article/details/gkouceqnk.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.fehbvm.com/Article/details/ggvjrozhf.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.blog.zdbjq.cn/Article/details/gfimfgjbs.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wap.zdbjq.cn/Article/details/gkfwlxsdt.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://read.share.fehbvm.com/Article/details/gnljhugzq.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.share.hesvh.cn/Article/details/glzjrxent.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://blog.zdbjq.cn/Article/details/gskctykbo.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.fehbvm.com/Article/details/gsgtdmpzn.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wap.fehbvm.com/Article/details/gfqqonqid.sHtML

[D06] 数组长度
来源：http://www.share.hesvh.cn/Article/details/gsthzkytl.sHtML

Py:   len(arr)
来源：http://wap.fehbvm.com/Article/details/ghhmuyssn.sHtML

PHP:  count($arr);
来源：http://read.share.hesvh.cn/Article/details/gvfdbykfj.sHtML

JS:   arr.length
来源：http://3g.zdbjq.cn/Article/details/gmnijhhyv.sHtML

TS:   arr.length
来源：http://read.share.hesvh.cn/Article/details/gylavgqxj.sHtML


<!-- 参考信息 -->