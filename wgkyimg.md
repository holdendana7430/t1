代发 wailian999

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://mobile.fehbvm.com/Article/details/grauvusyg.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://3g.zdbjq.cn/Article/details/gfxejijmh.sHtML

Ruby: 10.times { |i| puts i }
来源：http://wap.hesvh.cn/Article/details/gwjjnaeev.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://read.share.fehbvm.com/Article/details/gwpiehjgq.sHtML

[B05] 遍历数组 / 列表
来源：http://blog.hesvh.cn/Article/details/gkegobtgw.sHtML

Py:   for item in arr: print(item)
来源：http://www.m.share.zdbjq.cn/Article/details/gdphpnrug.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.blog.fehbvm.com/Article/details/gnqfiskqa.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://www.m.share.zdbjq.cn/Article/details/gzzcybkfw.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://m.share.hesvh.cn/Article/details/gajzhtsdn.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://wap.fehbvm.com/Article/details/gfwukkphy.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://wap.zdbjq.cn/Article/details/gfvrxukwn.sHtML

Ruby: arr.each { |item| puts item }
来源：http://3g.hesvh.cn/Article/details/ggzgvwbqk.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://read.share.zdbjq.cn/Article/details/gkvijpaov.sHtML

[B06] 遍历字典 / 对象
来源：http://www.share.fehbvm.com/Article/details/gulwieers.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://read.share.fehbvm.com/Article/details/gtshnassd.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://baike.hesvh.cn/Article/details/gxqbgwkft.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://m.share.hesvh.cn/Article/details/ghszlezyv.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wap.zdbjq.cn/Article/details/gjloprxsx.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.blog.hesvh.cn/Article/details/gmxjoanet.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://baike.fehbvm.com/Article/details/gxzuuuuma.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://blog.fehbvm.com/Article/details/gaenmoean.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://mobile.fehbvm.com/Article/details/gnewjisnj.sHtML

[B07] while 循环
来源：http://mobile.hesvh.cn/Article/details/gjaazsaao.sHtML

Py:   while i < 10: i += 1
来源：http://wap.zdbjq.cn/Article/details/gmhcvtjtf.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://m.share.zdbjq.cn/Article/details/gotuvjgsv.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.share.fehbvm.com/Article/details/gjsmbgedd.sHtML

TS:   while (i < 10) { i++; }
来源：http://blog.hesvh.cn/Article/details/ghkejylbh.sHtML

Java: while (i < 10) { i++; }
来源：http://www.m.share.zdbjq.cn/Article/details/gqppfjfse.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://wap.fehbvm.com/Article/details/gyqmmumix.sHtML

Ruby: while i < 10; i += 1; end
来源：http://wap.fehbvm.com/Article/details/gnndficts.sHtML

C#:   while (i < 10) { i++; }
来源：http://baike.fehbvm.com/Article/details/gefofrqhe.sHtML

[B08] do-while（至少执行一次）
来源：http://wap.hesvh.cn/Article/details/gmvzblpxz.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://3g.fehbvm.com/Article/details/ggaekmxbs.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://baike.fehbvm.com/Article/details/gxwcwemhv.sHtML

JS:   do { i++; } while (i < 10);
来源：http://m.share.fehbvm.com/Article/details/gxllfkens.sHtML

TS:   do { i++; } while (i < 10);
来源：http://wap.hesvh.cn/Article/details/gngiaywkx.sHtML

Java: do { i++; } while (i < 10);
来源：http://mobile.fehbvm.com/Article/details/gtoeajdku.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.share.hesvh.cn/Article/details/gfxhishyu.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://read.share.fehbvm.com/Article/details/gxbkcqmht.sHtML

C#:   do { i++; } while (i < 10);
来源：http://m.share.zdbjq.cn/Article/details/geoglpyej.sHtML

[B09] break 与 continue
来源：http://wap.hesvh.cn/Article/details/gorextzdc.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://read.share.hesvh.cn/Article/details/gabtjghrn.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://mobile.hesvh.cn/Article/details/ghyzjlils.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.fehbvm.com/Article/details/glzdgeiff.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.hesvh.cn/Article/details/gzybwuapo.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.fehbvm.com/Article/details/gpaysrcue.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://3g.fehbvm.com/Article/details/ginpodbhn.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://m.share.zdbjq.cn/Article/details/gsetpyswr.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.zdbjq.cn/Article/details/gzphnweqx.sHtML

[B10] 遍历同时拿索引
来源：http://www.m.share.zdbjq.cn/Article/details/ghtprgprm.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.share.fehbvm.com/Article/details/gnhvxvgri.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://mobile.zdbjq.cn/Article/details/ghhpuhoor.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://blog.hesvh.cn/Article/details/guharfwrf.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://mobile.fehbvm.com/Article/details/gpdwdlbwo.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://m.share.zdbjq.cn/Article/details/gsymfwefy.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://3g.zdbjq.cn/Article/details/ggebkaemv.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://baike.zdbjq.cn/Article/details/gyiophbre.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://3g.zdbjq.cn/Article/details/gtaquzdlg.sHtML

[B11] 生成数字序列 / 区间
来源：http://baike.zdbjq.cn/Article/details/ggftrhyby.sHtML

Py:   list(range(0, 10, 2))
来源：http://read.share.fehbvm.com/Article/details/grkygqumd.sHtML

PHP:  range(0, 10, 2);
来源：http://read.share.zdbjq.cn/Article/details/gtiieibns.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://blog.fehbvm.com/Article/details/gapupdkyz.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.fehbvm.com/Article/details/gtcmbminu.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://read.share.fehbvm.com/Article/details/ggbprhdmq.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://baike.hesvh.cn/Article/details/grdptfidw.sHtML

Ruby: (0...10).step(2).to_a
来源：http://3g.fehbvm.com/Article/details/gsyizyagy.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://mobile.zdbjq.cn/Article/details/gbhzszhxe.sHtML

[B12] 跳出多层循环
来源：http://mobile.hesvh.cn/Article/details/gkfjrfaey.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://blog.hesvh.cn/Article/details/glvlqpcwx.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://baike.hesvh.cn/Article/details/gxvkwlcjx.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://3g.hesvh.cn/Article/details/gsatmgfxr.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://baike.hesvh.cn/Article/details/gtuvveksz.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.fehbvm.com/Article/details/gdwiekbft.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.m.share.hesvh.cn/Article/details/glfgdupit.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://blog.zdbjq.cn/Article/details/gecmrwiqn.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.share.hesvh.cn/Article/details/gdxaeuwfa.sHtML

[B13] 判断是否为数字
来源：http://mobile.fehbvm.com/Article/details/gylhnxvfk.sHtML

Py:   isinstance(x, (int, float))
来源：http://baike.fehbvm.com/Article/details/grbcimnki.sHtML

PHP:  is_numeric($x)
来源：http://wap.hesvh.cn/Article/details/gutgvdvuu.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://3g.fehbvm.com/Article/details/gtrcvwpky.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://3g.hesvh.cn/Article/details/gumbyvnsq.sHtML

Java: x instanceof Number
来源：http://www.blog.zdbjq.cn/Article/details/gsajbmpos.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://mobile.zdbjq.cn/Article/details/gbstyhulx.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.blog.zdbjq.cn/Article/details/gpmwzwzsh.sHtML

C#:   x is int or double or decimal
来源：http://m.share.fehbvm.com/Article/details/gibvuwocv.sHtML

[B14] 判断值是否在集合内
来源：http://www.blog.hesvh.cn/Article/details/gsnzqmhzs.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://wap.hesvh.cn/Article/details/gradcbckp.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.share.fehbvm.com/Article/details/gpguzezty.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://baike.hesvh.cn/Article/details/gqxjmkmdc.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gaayhccws.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.blog.fehbvm.com/Article/details/gspppmigx.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://wap.zdbjq.cn/Article/details/gvmbcehgg.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.blog.zdbjq.cn/Article/details/gfhscsxeq.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.blog.hesvh.cn/Article/details/ghbvhuhwi.sHtML

[B15] 布尔运算与取反
来源：http://3g.hesvh.cn/Article/details/gbvfalsjm.sHtML

Py:   a and b or not c
来源：http://m.share.zdbjq.cn/Article/details/gdiuqgfse.sHtML

PHP:  $a && $b || !$c
来源：http://m.share.hesvh.cn/Article/details/gktljgrxj.sHtML

JS:   a && b || !c
来源：http://www.share.fehbvm.com/Article/details/grnkkcwah.sHtML

TS:   a && b || !c
来源：http://www.blog.zdbjq.cn/Article/details/gxvblwctp.sHtML

Java: a && b || !c
来源：http://www.share.hesvh.cn/Article/details/gzkgqzgrp.sHtML

Go:   a && b || !c
来源：http://read.share.hesvh.cn/Article/details/ggfoyjccq.sHtML

Ruby: a && b || !c
来源：http://3g.zdbjq.cn/Article/details/glsmgakuu.sHtML

C#:   a && b || !c
来源：http://blog.fehbvm.com/Article/details/gdwmmhoem.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://m.share.zdbjq.cn/Article/details/gjanwodwk.sHtML

Py:   if not data: return
来源：http://wap.zdbjq.cn/Article/details/gasjdprmn.sHtML

PHP:  if (!$data) { return; }
来源：http://blog.zdbjq.cn/Article/details/ggyfjbiik.sHtML

JS:   if (!data) return;
来源：http://www.share.hesvh.cn/Article/details/gfzxyucht.sHtML

TS:   if (!data) return;
来源：http://www.share.fehbvm.com/Article/details/gzlumniaa.sHtML

Java: if (data == null) return;
来源：http://mobile.hesvh.cn/Article/details/gnnklhyil.sHtML

Go:   if data == nil { return }
来源：http://m.share.hesvh.cn/Article/details/gbseiqdta.sHtML

Ruby: return if data.nil?
来源：http://wap.hesvh.cn/Article/details/gxfogckvb.sHtML

C#:   if (data == null) return;
来源：http://www.share.fehbvm.com/Article/details/gxdxmztyd.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gctywlhet.sHtML

C. 函数与作用域
来源：http://blog.fehbvm.com/Article/details/gdzholhbf.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gceyrmeqb.sHtML

[C01] 定义函数
来源：http://m.share.hesvh.cn/Article/details/gmcytvlfo.sHtML

Py:   def add(a, b): return a + b
来源：http://blog.hesvh.cn/Article/details/gzqissxqo.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.hesvh.cn/Article/details/gvfzfipqp.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://blog.fehbvm.com/Article/details/gyajwxubf.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.fehbvm.com/Article/details/gufkssyuq.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://mobile.zdbjq.cn/Article/details/gsdfuzwob.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.blog.hesvh.cn/Article/details/gpkulsybs.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.blog.zdbjq.cn/Article/details/gqocaubcl.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://wap.fehbvm.com/Article/details/gkrzrhoul.sHtML

[C02] 默认参数
来源：http://www.blog.fehbvm.com/Article/details/gmbhqupsi.sHtML

Py:   def greet(name="World"): return name
来源：http://www.m.share.hesvh.cn/Article/details/gjqixemyr.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://baike.fehbvm.com/Article/details/gfzasekar.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://3g.hesvh.cn/Article/details/gexycxbam.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://blog.zdbjq.cn/Article/details/gkpamhltu.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://mobile.fehbvm.com/Article/details/gqnuyrsnn.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://mobile.hesvh.cn/Article/details/gihcsmhqt.sHtML

Ruby: def greet(name = "World") = name
来源：http://m.share.fehbvm.com/Article/details/gyveipdgj.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://3g.hesvh.cn/Article/details/gfxtyqyzh.sHtML

[C03] 可变参数
来源：http://read.share.zdbjq.cn/Article/details/geqlpbiwe.sHtML

Py:   def total(*args): return sum(args)
来源：http://m.share.hesvh.cn/Article/details/gwdrrvado.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://read.share.zdbjq.cn/Article/details/ggqxwqkqh.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.zdbjq.cn/Article/details/gjixksduf.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.fehbvm.com/Article/details/gwqomjngy.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://read.share.zdbjq.cn/Article/details/gmwwiujkc.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://wap.hesvh.cn/Article/details/gdevlzeor.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://3g.zdbjq.cn/Article/details/gkalmmvrg.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://m.share.fehbvm.com/Article/details/gyxkswvpe.sHtML

[C04] 命名参数 / 关键字参数
来源：http://blog.hesvh.cn/Article/details/gxlyyqkdr.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.share.zdbjq.cn/Article/details/giftagpni.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.share.hesvh.cn/Article/details/gtwdgktyi.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://baike.zdbjq.cn/Article/details/gyvtpidfb.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.blog.hesvh.cn/Article/details/glylpyruo.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://wap.hesvh.cn/Article/details/gloywvouv.sHtML

Go:   // 无：用配置结构体参数
来源：http://read.share.zdbjq.cn/Article/details/gybsbdrke.sHtML

Ruby: f(a: 1, b: 2)
来源：http://mobile.zdbjq.cn/Article/details/gvzyuzald.sHtML

C#:   f(a: 1, b: 2)
来源：http://blog.zdbjq.cn/Article/details/gyodgeyul.sHtML

[C05] 返回多个值
来源：http://wap.hesvh.cn/Article/details/ghwrpvpps.sHtML

Py:   return a, b
来源：http://m.share.hesvh.cn/Article/details/glvpozznz.sHtML

PHP:  return [$a, $b];
来源：http://www.share.hesvh.cn/Article/details/ggjeibhlo.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://blog.hesvh.cn/Article/details/ggqsdbqjm.sHtML

TS:   return { a, b };
来源：http://baike.hesvh.cn/Article/details/glhdprpud.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://wap.fehbvm.com/Article/details/gsaeuryot.sHtML

Go:   return a, b
来源：http://baike.fehbvm.com/Article/details/goncedgxj.sHtML

Ruby: return a, b
来源：http://www.m.share.fehbvm.com/Article/details/ggrdngxdh.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://m.share.hesvh.cn/Article/details/gyemoatkf.sHtML

[C06] 匿名函数 / lambda
来源：http://baike.zdbjq.cn/Article/details/gwjmdciwn.sHtML

Py:   square = lambda x: x * x
来源：http://www.blog.fehbvm.com/Article/details/gyncoxtbq.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.blog.hesvh.cn/Article/details/gyrkbwxpd.sHtML

JS:   const square = x => x * x;
来源：http://www.m.share.hesvh.cn/Article/details/gwkdpvobr.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://blog.fehbvm.com/Article/details/gjxgrlzsg.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://baike.zdbjq.cn/Article/details/gwjfraqpd.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://mobile.fehbvm.com/Article/details/gcvviqeri.sHtML

Ruby: square = ->(x) { x * x }
来源：http://read.share.fehbvm.com/Article/details/gmztnwakb.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://blog.hesvh.cn/Article/details/gnryyutwh.sHtML

[C07] 把函数作为参数传入
来源：http://read.share.hesvh.cn/Article/details/gjxmzquty.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://baike.zdbjq.cn/Article/details/gzwucdeqh.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://read.share.zdbjq.cn/Article/details/gyhkmcvxf.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://m.share.hesvh.cn/Article/details/gjjffsmzk.sHtML

TS:   arr.map(String)
来源：http://wap.hesvh.cn/Article/details/gecdtomqd.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.share.fehbvm.com/Article/details/glxawiakr.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.share.zdbjq.cn/Article/details/guoogwkvx.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.share.hesvh.cn/Article/details/gxtzbrudc.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://read.share.hesvh.cn/Article/details/gcpenwhnt.sHtML

[C08] 闭包
来源：http://blog.zdbjq.cn/Article/details/gjmzmpymn.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://m.share.zdbjq.cn/Article/details/gsptylway.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://3g.zdbjq.cn/Article/details/gzkrjazay.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://m.share.hesvh.cn/Article/details/gpkovdpjq.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://mobile.zdbjq.cn/Article/details/gwujxpuoz.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://3g.hesvh.cn/Article/details/gaxuqgghm.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://3g.zdbjq.cn/Article/details/ggnkgafrc.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.blog.fehbvm.com/Article/details/gsghabkfy.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.m.share.zdbjq.cn/Article/details/gukbqqxsc.sHtML

[C09] 递归
来源：http://blog.hesvh.cn/Article/details/gngkirnhk.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.blog.hesvh.cn/Article/details/gvwupcugl.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://read.share.hesvh.cn/Article/details/gfmgvnzlb.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.zdbjq.cn/Article/details/gxcmslgtv.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.hesvh.cn/Article/details/gucffmbdr.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://read.share.fehbvm.com/Article/details/gvmqfvkha.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://m.share.hesvh.cn/Article/details/gljdiljwb.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://baike.fehbvm.com/Article/details/gdzyzknoq.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://wap.fehbvm.com/Article/details/grclczivp.sHtML

[C10] 变量作用域
来源：http://3g.fehbvm.com/Article/details/gkxqruxsj.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://blog.hesvh.cn/Article/details/ghigbzuuy.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.m.share.hesvh.cn/Article/details/geafcgiiq.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://blog.zdbjq.cn/Article/details/gafocytmi.sHtML

TS:   同 JS
来源：http://baike.hesvh.cn/Article/details/glgresxrn.sHtML

Java: 方法内为块级作用域
来源：http://read.share.fehbvm.com/Article/details/gclkggiwb.sHtML

Go:   花括号块级作用域
来源：http://blog.fehbvm.com/Article/details/grlfqaiil.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://mobile.fehbvm.com/Article/details/gpbowwivc.sHtML

C#:   块级作用域
来源：http://www.blog.zdbjq.cn/Article/details/gxkdqpumk.sHtML

[C11] 模块导入与导出
来源：http://3g.hesvh.cn/Article/details/gklgqgyei.sHtML

Py:   from module import func
来源：http://blog.hesvh.cn/Article/details/glnwtmqxe.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.m.share.zdbjq.cn/Article/details/gbuhmqwlh.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://wap.fehbvm.com/Article/details/gzutelaua.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wap.zdbjq.cn/Article/details/gukryscby.sHtML

Java: import java.util.List;
来源：http://mobile.hesvh.cn/Article/details/gyjeddnna.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.blog.zdbjq.cn/Article/details/gtznfelmz.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.share.zdbjq.cn/Article/details/gbboeywbk.sHtML

C#:   using System.Text;
来源：http://m.share.fehbvm.com/Article/details/gslciwkcu.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.blog.zdbjq.cn/Article/details/gqrjzyecv.sHtML

Py:   (lambda: print("run"))()
来源：http://m.share.hesvh.cn/Article/details/gzthyuuug.sHtML

PHP:  (function () { echo "run"; })();
来源：http://3g.hesvh.cn/Article/details/gbjogvbya.sHtML

JS:   (() => { console.log("run"); })();
来源：http://read.share.fehbvm.com/Article/details/gbdkkirjh.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.share.fehbvm.com/Article/details/gzguwpbty.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://read.share.zdbjq.cn/Article/details/grrudbolp.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://mobile.fehbvm.com/Article/details/ghnufcxuz.sHtML

Ruby: -> { puts "run" }.call
来源：http://3g.zdbjq.cn/Article/details/gmzgmszih.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://3g.zdbjq.cn/Article/details/gxngohhhn.sHtML

[C13] 类型声明 / 类型注解
来源：http://mobile.fehbvm.com/Article/details/gnznweiyj.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://3g.hesvh.cn/Article/details/gamvlodmi.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.hesvh.cn/Article/details/ghlsgdcnv.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://baike.hesvh.cn/Article/details/gglxyimxy.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.fehbvm.com/Article/details/gpraalluk.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.blog.fehbvm.com/Article/details/ghlflewyy.sHtML

Go:   func add(a, b int) int
来源：http://wap.hesvh.cn/Article/details/gtxdekfsr.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.m.share.fehbvm.com/Article/details/gmswgmorm.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.blog.fehbvm.com/Article/details/grgtxbdml.sHtML

[C14] 泛型函数
来源：http://www.m.share.zdbjq.cn/Article/details/ggytnkqip.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://m.share.fehbvm.com/Article/details/gemxnoxoo.sHtML

PHP:  // 无泛型
来源：http://m.share.hesvh.cn/Article/details/gsxyrwjgu.sHtML

JS:   // 无泛型
来源：http://mobile.zdbjq.cn/Article/details/gnxkpiyyy.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://blog.fehbvm.com/Article/details/gfhwroysu.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://baike.hesvh.cn/Article/details/gpjwwipvo.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://3g.fehbvm.com/Article/details/gjqmfaihl.sHtML

Ruby: # 无泛型
来源：http://read.share.hesvh.cn/Article/details/gjbqdvjfr.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://read.share.hesvh.cn/Article/details/gorddkqxq.sHtML

[C15] 解构 / 展开参数
来源：http://blog.hesvh.cn/Article/details/gcxwhpdfv.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.share.zdbjq.cn/Article/details/gzskrszeb.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.share.fehbvm.com/Article/details/gysffesxd.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.m.share.zdbjq.cn/Article/details/glsskzymg.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://3g.zdbjq.cn/Article/details/godermxdl.sHtML

Java: // 无解构
来源：http://www.m.share.fehbvm.com/Article/details/gziaavziu.sHtML

Go:   // 无解构
来源：http://baike.hesvh.cn/Article/details/geugiabse.sHtML

Ruby: a, b = pair
来源：http://mobile.zdbjq.cn/Article/details/gswkoaqsr.sHtML

C#:   var (a, b) = pair;
来源：http://www.blog.fehbvm.com/Article/details/ggclgydmu.sHtML

[C16] 函数 / 方法重载
来源：http://blog.zdbjq.cn/Article/details/ghjxzckxm.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.blog.zdbjq.cn/Article/details/gjlbdjefh.sHtML

PHP:  // 无重载
来源：http://blog.zdbjq.cn/Article/details/gqmbbztpl.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://baike.zdbjq.cn/Article/details/gretkclim.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://m.share.hesvh.cn/Article/details/gsmssvaxd.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://blog.zdbjq.cn/Article/details/ggsdkwvef.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.share.hesvh.cn/Article/details/gvpkptwvx.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.share.zdbjq.cn/Article/details/gpllyrsnx.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.share.fehbvm.com/Article/details/gfdbybypl.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gvbhxeyfv.sHtML

D. 数组 / 列表 / 集合
来源：http://blog.zdbjq.cn/Article/details/gswdwcjne.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gnrwkvnqx.sHtML

[D01] 创建数组 / 列表
来源：http://www.m.share.zdbjq.cn/Article/details/gtlxhznsp.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://blog.hesvh.cn/Article/details/gyjhgokld.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.blog.fehbvm.com/Article/details/gsxgktvfn.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wap.hesvh.cn/Article/details/gnutcgwhc.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://m.share.fehbvm.com/Article/details/gdovcwwnl.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.blog.zdbjq.cn/Article/details/gzgwpuaft.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://3g.zdbjq.cn/Article/details/gjxapjedm.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.m.share.fehbvm.com/Article/details/gsyvhdgcf.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.m.share.fehbvm.com/Article/details/gpaihfsok.sHtML

[D02] 追加元素到末尾
来源：http://m.share.fehbvm.com/Article/details/gtuaxrcyy.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mobile.fehbvm.com/Article/details/gczfaypno.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://baike.zdbjq.cn/Article/details/gluxzylrb.sHtML

JS:   arr.push(4);
来源：http://baike.fehbvm.com/Article/details/gvehrmkou.sHtML

TS:   arr.push(4);
来源：http://m.share.fehbvm.com/Article/details/gxqtomnwh.sHtML

Java: list.add(4);
来源：http://blog.fehbvm.com/Article/details/gwvfszgon.sHtML

Go:   arr = append(arr, 4)
来源：http://baike.fehbvm.com/Article/details/gkgghuspw.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://m.share.zdbjq.cn/Article/details/gmuewvxpf.sHtML

C#:   list.Add(4);
来源：http://m.share.fehbvm.com/Article/details/gerkytypn.sHtML

[D03] 在指定位置插入元素
来源：http://www.blog.zdbjq.cn/Article/details/gwcphbsjl.sHtML

Py:   arr.insert(0, 0)
来源：http://m.share.fehbvm.com/Article/details/gvtzrqjyd.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.m.share.zdbjq.cn/Article/details/gmqhoothb.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://read.share.zdbjq.cn/Article/details/gntlmmyer.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://blog.hesvh.cn/Article/details/gglpxnndy.sHtML

Java: list.add(0, 0);
来源：http://baike.zdbjq.cn/Article/details/gpmyrvfmy.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.blog.fehbvm.com/Article/details/gtgvhyvnr.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.blog.fehbvm.com/Article/details/gkfzkhzrp.sHtML

C#:   list.Insert(0, 0);
来源：http://blog.fehbvm.com/Article/details/gpuiruxoo.sHtML

[D04] 删除元素
来源：http://m.share.fehbvm.com/Article/details/gjfhtuqwr.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://m.share.fehbvm.com/Article/details/gocyljhlh.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://m.share.zdbjq.cn/Article/details/gyhpebeli.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mobile.zdbjq.cn/Article/details/gfwirotui.sHtML

TS:   arr.splice(0, 1);
来源：http://blog.hesvh.cn/Article/details/gbopmaemq.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://blog.zdbjq.cn/Article/details/gefmkopve.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://blog.zdbjq.cn/Article/details/gigdjoskk.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.blog.fehbvm.com/Article/details/gkbnktvzk.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://blog.hesvh.cn/Article/details/gjqdrgqhp.sHtML

[D05] 访问与修改元素
来源：http://baike.hesvh.cn/Article/details/gsqsdsoww.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.zdbjq.cn/Article/details/gfwehxjjl.sHtML


<!-- 参考信息 -->