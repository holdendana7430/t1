代发 wailian999

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://read.share.hesvh.cn/Article/details/gsrsjrcfk.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://3g.fehbvm.com/Article/details/gtdxmltge.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://mobile.fehbvm.com/Article/details/giinxacdz.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://3g.hesvh.cn/Article/details/ghvywicai.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://read.share.fehbvm.com/Article/details/gmhcgxprq.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.share.fehbvm.com/Article/details/goojxzano.sHtML

[B07] while 循环
来源：http://read.share.fehbvm.com/Article/details/gjkwlsove.sHtML

Py:   while i < 10: i += 1
来源：http://baike.fehbvm.com/Article/details/gqzksgxsq.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://baike.hesvh.cn/Article/details/gmrrhezls.sHtML

JS:   while (i < 10) { i++; }
来源：http://read.share.hesvh.cn/Article/details/gaboyufkp.sHtML

TS:   while (i < 10) { i++; }
来源：http://read.share.zdbjq.cn/Article/details/glkvkfocj.sHtML

Java: while (i < 10) { i++; }
来源：http://www.blog.hesvh.cn/Article/details/gkpjjqlwv.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://3g.fehbvm.com/Article/details/gaoidoxto.sHtML

Ruby: while i < 10; i += 1; end
来源：http://baike.hesvh.cn/Article/details/gyetxmqes.sHtML

C#:   while (i < 10) { i++; }
来源：http://baike.hesvh.cn/Article/details/gbadvcflo.sHtML

[B08] do-while（至少执行一次）
来源：http://www.share.fehbvm.com/Article/details/gmadwbowx.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://baike.hesvh.cn/Article/details/gaajddmkk.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.blog.fehbvm.com/Article/details/gybzgcpri.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.blog.fehbvm.com/Article/details/grbrfotsu.sHtML

TS:   do { i++; } while (i < 10);
来源：http://baike.fehbvm.com/Article/details/grsdrgldw.sHtML

Java: do { i++; } while (i < 10);
来源：http://blog.fehbvm.com/Article/details/gpzboebwm.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://mobile.zdbjq.cn/Article/details/gsiwsgxvq.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.blog.zdbjq.cn/Article/details/gjwsojcry.sHtML

C#:   do { i++; } while (i < 10);
来源：http://3g.hesvh.cn/Article/details/gqehyxltk.sHtML

[B09] break 与 continue
来源：http://baike.fehbvm.com/Article/details/gdoavrrzs.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.share.hesvh.cn/Article/details/githhoouk.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://blog.hesvh.cn/Article/details/gennafaen.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.fehbvm.com/Article/details/gnkfzjchb.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.zdbjq.cn/Article/details/guzevmnza.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.fehbvm.com/Article/details/gwraexqew.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://mobile.hesvh.cn/Article/details/grtcltyjs.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://read.share.fehbvm.com/Article/details/guynawbdn.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.hesvh.cn/Article/details/guglpmwtr.sHtML

[B10] 遍历同时拿索引
来源：http://www.blog.fehbvm.com/Article/details/gsgqcwzdn.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://baike.hesvh.cn/Article/details/gcjtprmya.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://m.share.hesvh.cn/Article/details/goeadgtmu.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://read.share.zdbjq.cn/Article/details/gpoduzyrh.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.m.share.zdbjq.cn/Article/details/gcmtwdntt.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.m.share.hesvh.cn/Article/details/gzluccdok.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.m.share.fehbvm.com/Article/details/gjhtyadzg.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://baike.fehbvm.com/Article/details/gmqsbxkxi.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://wap.fehbvm.com/Article/details/gusxgvpkt.sHtML

[B11] 生成数字序列 / 区间
来源：http://m.share.fehbvm.com/Article/details/glpftobwq.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.blog.hesvh.cn/Article/details/ggemltxrr.sHtML

PHP:  range(0, 10, 2);
来源：http://blog.fehbvm.com/Article/details/guchzkgwg.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.zdbjq.cn/Article/details/gcsgsxzoq.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.hesvh.cn/Article/details/gazyaetzf.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.m.share.hesvh.cn/Article/details/gpfkwpesx.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://3g.zdbjq.cn/Article/details/gkibkywlm.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.m.share.hesvh.cn/Article/details/gwfkywfun.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://wap.hesvh.cn/Article/details/ghoieuufm.sHtML

[B12] 跳出多层循环
来源：http://3g.hesvh.cn/Article/details/glqbbfdkh.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.share.zdbjq.cn/Article/details/gkxwcbram.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.blog.zdbjq.cn/Article/details/ghcnwtbaw.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://baike.fehbvm.com/Article/details/gzqeanxvz.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.fehbvm.com/Article/details/gcwvhuaci.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://mobile.hesvh.cn/Article/details/gvohaujmz.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://blog.fehbvm.com/Article/details/gwipdigqy.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.m.share.fehbvm.com/Article/details/gzvfissui.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://read.share.zdbjq.cn/Article/details/glqjchkhg.sHtML

[B13] 判断是否为数字
来源：http://www.share.hesvh.cn/Article/details/gecxninir.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.share.hesvh.cn/Article/details/gwdvdxtbv.sHtML

PHP:  is_numeric($x)
来源：http://m.share.zdbjq.cn/Article/details/glrxhkwsz.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://blog.hesvh.cn/Article/details/gvavaqihq.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://3g.zdbjq.cn/Article/details/gtqpoahkp.sHtML

Java: x instanceof Number
来源：http://wap.hesvh.cn/Article/details/gywwbcjfx.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://3g.zdbjq.cn/Article/details/grqtgchlc.sHtML

Ruby: x.is_a?(Numeric)
来源：http://read.share.hesvh.cn/Article/details/guynzfeid.sHtML

C#:   x is int or double or decimal
来源：http://www.share.fehbvm.com/Article/details/gpeaefpdq.sHtML

[B14] 判断值是否在集合内
来源：http://www.blog.zdbjq.cn/Article/details/gerkjiqcl.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://baike.hesvh.cn/Article/details/glcjmgeru.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://mobile.hesvh.cn/Article/details/gzdjciisi.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://mobile.hesvh.cn/Article/details/glzubkgws.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://blog.hesvh.cn/Article/details/givnoiqon.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://wap.fehbvm.com/Article/details/gnnawyfos.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://m.share.hesvh.cn/Article/details/gejqmkgyt.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://blog.hesvh.cn/Article/details/glzboxhqk.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://read.share.hesvh.cn/Article/details/gwdslvtpp.sHtML

[B15] 布尔运算与取反
来源：http://blog.hesvh.cn/Article/details/gkpexwxtp.sHtML

Py:   a and b or not c
来源：http://baike.zdbjq.cn/Article/details/grkgmjvkn.sHtML

PHP:  $a && $b || !$c
来源：http://www.blog.hesvh.cn/Article/details/gsneuvtug.sHtML

JS:   a && b || !c
来源：http://m.share.fehbvm.com/Article/details/ggdpbybsh.sHtML

TS:   a && b || !c
来源：http://blog.hesvh.cn/Article/details/gmoanwsyc.sHtML

Java: a && b || !c
来源：http://blog.hesvh.cn/Article/details/gknaktixg.sHtML

Go:   a && b || !c
来源：http://www.blog.fehbvm.com/Article/details/gupgzhoxo.sHtML

Ruby: a && b || !c
来源：http://mobile.fehbvm.com/Article/details/gmuvujdee.sHtML

C#:   a && b || !c
来源：http://mobile.fehbvm.com/Article/details/gpofgfbdv.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://wap.hesvh.cn/Article/details/gycklapio.sHtML

Py:   if not data: return
来源：http://m.share.fehbvm.com/Article/details/gixnjqfmi.sHtML

PHP:  if (!$data) { return; }
来源：http://wap.zdbjq.cn/Article/details/gkyvfqdzp.sHtML

JS:   if (!data) return;
来源：http://read.share.zdbjq.cn/Article/details/gopxmeeaz.sHtML

TS:   if (!data) return;
来源：http://m.share.zdbjq.cn/Article/details/grlqwtqjn.sHtML

Java: if (data == null) return;
来源：http://www.blog.zdbjq.cn/Article/details/gnfspxfcu.sHtML

Go:   if data == nil { return }
来源：http://blog.hesvh.cn/Article/details/gidthwclb.sHtML

Ruby: return if data.nil?
来源：http://baike.zdbjq.cn/Article/details/gqhgwwdmf.sHtML

C#:   if (data == null) return;
来源：http://read.share.hesvh.cn/Article/details/gopjfymmm.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/guzqkcopt.sHtML

C. 函数与作用域
来源：http://mobile.hesvh.cn/Article/details/gjaplvtsd.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/ghaswucsn.sHtML

[C01] 定义函数
来源：http://blog.hesvh.cn/Article/details/gheblfhez.sHtML

Py:   def add(a, b): return a + b
来源：http://www.blog.fehbvm.com/Article/details/gawghtacf.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.zdbjq.cn/Article/details/ggirnhiwl.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://wap.hesvh.cn/Article/details/glphcyczo.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.zdbjq.cn/Article/details/gvjewokxg.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://baike.zdbjq.cn/Article/details/gebqaolyk.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://mobile.hesvh.cn/Article/details/gsnqcgbsy.sHtML

Ruby: def add(a, b); a + b; end
来源：http://m.share.hesvh.cn/Article/details/gjdfzlssj.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.blog.fehbvm.com/Article/details/gqiabnqgm.sHtML

[C02] 默认参数
来源：http://m.share.zdbjq.cn/Article/details/gendjemot.sHtML

Py:   def greet(name="World"): return name
来源：http://mobile.hesvh.cn/Article/details/gbhytkrhx.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.blog.hesvh.cn/Article/details/gceopfvds.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://mobile.zdbjq.cn/Article/details/gykefjruw.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://read.share.fehbvm.com/Article/details/gpivborsp.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.m.share.hesvh.cn/Article/details/gxvwnqwov.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://3g.hesvh.cn/Article/details/gthneswhv.sHtML

Ruby: def greet(name = "World") = name
来源：http://baike.fehbvm.com/Article/details/gjglzozen.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://blog.fehbvm.com/Article/details/giejilxxv.sHtML

[C03] 可变参数
来源：http://www.share.fehbvm.com/Article/details/goctqtjne.sHtML

Py:   def total(*args): return sum(args)
来源：http://wap.zdbjq.cn/Article/details/gdmgaftlt.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.blog.zdbjq.cn/Article/details/gqtzxbalu.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.zdbjq.cn/Article/details/gvjbenrfh.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.zdbjq.cn/Article/details/grogfgttu.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://read.share.zdbjq.cn/Article/details/gcvgvrzrf.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://baike.fehbvm.com/Article/details/glajehinh.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://baike.hesvh.cn/Article/details/gzjarlaus.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://m.share.hesvh.cn/Article/details/gwzgriubn.sHtML

[C04] 命名参数 / 关键字参数
来源：http://blog.hesvh.cn/Article/details/glraifjlu.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://3g.hesvh.cn/Article/details/ghwsywgmo.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://read.share.hesvh.cn/Article/details/gbrzgscdp.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://3g.fehbvm.com/Article/details/gqnwvyhue.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://read.share.fehbvm.com/Article/details/gnrazcyel.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://blog.zdbjq.cn/Article/details/gnuvxmllm.sHtML

Go:   // 无：用配置结构体参数
来源：http://m.share.hesvh.cn/Article/details/grnmomuws.sHtML

Ruby: f(a: 1, b: 2)
来源：http://3g.fehbvm.com/Article/details/gyxcekhpt.sHtML

C#:   f(a: 1, b: 2)
来源：http://mobile.hesvh.cn/Article/details/gjlyoxgbe.sHtML

[C05] 返回多个值
来源：http://read.share.zdbjq.cn/Article/details/ghezwtneh.sHtML

Py:   return a, b
来源：http://www.m.share.zdbjq.cn/Article/details/grxhkvorg.sHtML

PHP:  return [$a, $b];
来源：http://wap.zdbjq.cn/Article/details/gyjequbzh.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://wap.fehbvm.com/Article/details/gzuftqxxo.sHtML

TS:   return { a, b };
来源：http://read.share.hesvh.cn/Article/details/gjhnyyryb.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.blog.fehbvm.com/Article/details/gzozjgygf.sHtML

Go:   return a, b
来源：http://m.share.zdbjq.cn/Article/details/gghvhefyj.sHtML

Ruby: return a, b
来源：http://3g.fehbvm.com/Article/details/glwlbpxwv.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://m.share.fehbvm.com/Article/details/gaogfhktc.sHtML

[C06] 匿名函数 / lambda
来源：http://read.share.fehbvm.com/Article/details/ggcaygjku.sHtML

Py:   square = lambda x: x * x
来源：http://baike.zdbjq.cn/Article/details/gxtkypghh.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://m.share.hesvh.cn/Article/details/gdovleujh.sHtML

JS:   const square = x => x * x;
来源：http://www.blog.hesvh.cn/Article/details/gsrjqmnnk.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.m.share.zdbjq.cn/Article/details/golqbhfzj.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://read.share.fehbvm.com/Article/details/gwtbqeysn.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://3g.fehbvm.com/Article/details/gvemeusfh.sHtML

Ruby: square = ->(x) { x * x }
来源：http://m.share.hesvh.cn/Article/details/glxwzqalt.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.blog.hesvh.cn/Article/details/gxrwnobna.sHtML

[C07] 把函数作为参数传入
来源：http://www.share.hesvh.cn/Article/details/gltvrwmdn.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://blog.zdbjq.cn/Article/details/gmxjjpanh.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://read.share.fehbvm.com/Article/details/gmdkryzot.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://m.share.fehbvm.com/Article/details/goujmgqnw.sHtML

TS:   arr.map(String)
来源：http://wap.hesvh.cn/Article/details/gfqhasrct.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://m.share.zdbjq.cn/Article/details/gqwwvqbiq.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://baike.fehbvm.com/Article/details/gabdapjde.sHtML

Ruby: arr.map(&:upcase)
来源：http://blog.zdbjq.cn/Article/details/gqhubludg.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://mobile.hesvh.cn/Article/details/gofbxrmqp.sHtML

[C08] 闭包
来源：http://mobile.hesvh.cn/Article/details/gsaqxbloq.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://wap.zdbjq.cn/Article/details/gjikdjyml.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.blog.zdbjq.cn/Article/details/gmlymcypm.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.blog.zdbjq.cn/Article/details/ghkvkzivv.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://read.share.hesvh.cn/Article/details/ghfcjdwcy.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.share.fehbvm.com/Article/details/gihipgfpm.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://baike.zdbjq.cn/Article/details/gtxpceasn.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://baike.zdbjq.cn/Article/details/gbckdonin.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://3g.hesvh.cn/Article/details/gssgwuiyg.sHtML

[C09] 递归
来源：http://mobile.fehbvm.com/Article/details/gcqlhokll.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://baike.zdbjq.cn/Article/details/gjqzjeldx.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://3g.hesvh.cn/Article/details/ghsrjvhcq.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.hesvh.cn/Article/details/ggnnspjam.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.zdbjq.cn/Article/details/gkgzbeqpi.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://baike.zdbjq.cn/Article/details/gsadaysdk.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://m.share.hesvh.cn/Article/details/gzdfnygmk.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://read.share.zdbjq.cn/Article/details/gfdouumtg.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://mobile.zdbjq.cn/Article/details/gwtwsuqvf.sHtML

[C10] 变量作用域
来源：http://baike.zdbjq.cn/Article/details/gchyuspat.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.blog.hesvh.cn/Article/details/gpfeyvwke.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.m.share.zdbjq.cn/Article/details/gphfiucqt.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.m.share.fehbvm.com/Article/details/gmthdtefr.sHtML

TS:   同 JS
来源：http://baike.fehbvm.com/Article/details/glinwfptu.sHtML

Java: 方法内为块级作用域
来源：http://www.blog.hesvh.cn/Article/details/gmlylrnjd.sHtML

Go:   花括号块级作用域
来源：http://www.share.fehbvm.com/Article/details/gogfrsklp.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://baike.zdbjq.cn/Article/details/gazmkhzfq.sHtML

C#:   块级作用域
来源：http://www.blog.hesvh.cn/Article/details/gefkjoovb.sHtML

[C11] 模块导入与导出
来源：http://wap.hesvh.cn/Article/details/guhxakitx.sHtML

Py:   from module import func
来源：http://blog.zdbjq.cn/Article/details/gualeodrl.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://baike.zdbjq.cn/Article/details/gmxcdceky.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.blog.fehbvm.com/Article/details/glfjxnias.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://blog.fehbvm.com/Article/details/gnkiorflf.sHtML

Java: import java.util.List;
来源：http://mobile.hesvh.cn/Article/details/gedopgxja.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://baike.fehbvm.com/Article/details/gmvolzcla.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://3g.zdbjq.cn/Article/details/gbhgmwkvg.sHtML

C#:   using System.Text;
来源：http://wap.hesvh.cn/Article/details/ggcddoeii.sHtML

[C12] 立即执行函数 IIFE
来源：http://3g.fehbvm.com/Article/details/gzmdisqhf.sHtML

Py:   (lambda: print("run"))()
来源：http://baike.zdbjq.cn/Article/details/gsqfahbdv.sHtML

PHP:  (function () { echo "run"; })();
来源：http://wap.hesvh.cn/Article/details/gaeoypars.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.blog.zdbjq.cn/Article/details/gteczcqlx.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.m.share.zdbjq.cn/Article/details/gqqsroehg.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://3g.hesvh.cn/Article/details/gseseqiok.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://mobile.fehbvm.com/Article/details/gkhsxqokg.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.blog.zdbjq.cn/Article/details/gxgbaurep.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://m.share.fehbvm.com/Article/details/gstrmdohk.sHtML

[C13] 类型声明 / 类型注解
来源：http://read.share.fehbvm.com/Article/details/gcegjykzz.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://mobile.hesvh.cn/Article/details/gntfayhsf.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.hesvh.cn/Article/details/gmfwysold.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.blog.zdbjq.cn/Article/details/gwpuihuef.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.fehbvm.com/Article/details/gixsfehjt.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://mobile.zdbjq.cn/Article/details/giyaphjtb.sHtML

Go:   func add(a, b int) int
来源：http://m.share.hesvh.cn/Article/details/gsezizqme.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://3g.zdbjq.cn/Article/details/gsbwjzsnu.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://baike.fehbvm.com/Article/details/gchvejrry.sHtML

[C14] 泛型函数
来源：http://wap.zdbjq.cn/Article/details/gzqwfxgfj.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://blog.zdbjq.cn/Article/details/gtwvrrsmw.sHtML

PHP:  // 无泛型
来源：http://www.m.share.zdbjq.cn/Article/details/gmhrzagtx.sHtML

JS:   // 无泛型
来源：http://blog.zdbjq.cn/Article/details/gncncmqnc.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://blog.zdbjq.cn/Article/details/gpnhlxvyb.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://3g.zdbjq.cn/Article/details/gzhcnyupt.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://baike.hesvh.cn/Article/details/gdiokqvup.sHtML

Ruby: # 无泛型
来源：http://www.share.zdbjq.cn/Article/details/gzyhefzjy.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.blog.fehbvm.com/Article/details/gnubwzpva.sHtML

[C15] 解构 / 展开参数
来源：http://blog.fehbvm.com/Article/details/grhcmedax.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://blog.hesvh.cn/Article/details/ginfkowrj.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.m.share.fehbvm.com/Article/details/gxjrxkzjg.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.share.hesvh.cn/Article/details/glmeixmtz.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://blog.hesvh.cn/Article/details/ggazlfspl.sHtML

Java: // 无解构
来源：http://3g.fehbvm.com/Article/details/gvcziinsz.sHtML

Go:   // 无解构
来源：http://m.share.fehbvm.com/Article/details/glqbvszxi.sHtML

Ruby: a, b = pair
来源：http://mobile.hesvh.cn/Article/details/gwyuapxgn.sHtML

C#:   var (a, b) = pair;
来源：http://www.blog.zdbjq.cn/Article/details/gwgzmyqcw.sHtML

[C16] 函数 / 方法重载
来源：http://3g.hesvh.cn/Article/details/greolccgv.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://m.share.zdbjq.cn/Article/details/geavpeewb.sHtML

PHP:  // 无重载
来源：http://read.share.hesvh.cn/Article/details/gvuphepuf.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://baike.hesvh.cn/Article/details/gcvlxlden.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.m.share.fehbvm.com/Article/details/gjkbihdzf.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://baike.fehbvm.com/Article/details/glzatehvd.sHtML

Go:   // 无重载：用不同函数名
来源：http://m.share.fehbvm.com/Article/details/gldaukqjr.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.blog.zdbjq.cn/Article/details/gxsnmnzpm.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://read.share.zdbjq.cn/Article/details/grtjfsnmq.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gqrpwcbxf.sHtML

D. 数组 / 列表 / 集合
来源：http://3g.zdbjq.cn/Article/details/ghznieuqp.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gxwlymxud.sHtML

[D01] 创建数组 / 列表
来源：http://blog.fehbvm.com/Article/details/gujvaxgku.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.m.share.zdbjq.cn/Article/details/grxykifex.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.share.fehbvm.com/Article/details/gqpypayoa.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://read.share.hesvh.cn/Article/details/gzbiuqhhv.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://read.share.zdbjq.cn/Article/details/gvjkublkh.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://3g.zdbjq.cn/Article/details/ggxuqtrjp.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://read.share.fehbvm.com/Article/details/glzujtedj.sHtML

Ruby: arr = [1, 2, 3]
来源：http://baike.zdbjq.cn/Article/details/gvmktdjow.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://mobile.hesvh.cn/Article/details/gxwdcqhmb.sHtML

[D02] 追加元素到末尾
来源：http://baike.fehbvm.com/Article/details/gfxzuvmsd.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mobile.zdbjq.cn/Article/details/gktctnuwt.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://m.share.hesvh.cn/Article/details/ggptbrbyl.sHtML

JS:   arr.push(4);
来源：http://3g.hesvh.cn/Article/details/giahdzafc.sHtML

TS:   arr.push(4);
来源：http://3g.hesvh.cn/Article/details/gqnztzxkb.sHtML

Java: list.add(4);
来源：http://read.share.hesvh.cn/Article/details/gizolhoxv.sHtML

Go:   arr = append(arr, 4)
来源：http://read.share.hesvh.cn/Article/details/ghszbcemx.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.m.share.zdbjq.cn/Article/details/gmlzrmtga.sHtML

C#:   list.Add(4);
来源：http://www.blog.zdbjq.cn/Article/details/gbqllbhpk.sHtML

[D03] 在指定位置插入元素
来源：http://www.blog.hesvh.cn/Article/details/gmljqvybh.sHtML

Py:   arr.insert(0, 0)
来源：http://blog.fehbvm.com/Article/details/gtnjtovwc.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.m.share.hesvh.cn/Article/details/guncmwshq.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.m.share.fehbvm.com/Article/details/gcuqmzfqs.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.m.share.hesvh.cn/Article/details/gwdnhzkux.sHtML

Java: list.add(0, 0);
来源：http://baike.zdbjq.cn/Article/details/gcjrprrit.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://baike.hesvh.cn/Article/details/gmcxfezgi.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://m.share.fehbvm.com/Article/details/gagszucll.sHtML

C#:   list.Insert(0, 0);
来源：http://m.share.zdbjq.cn/Article/details/gfrblkbiu.sHtML

[D04] 删除元素
来源：http://mobile.hesvh.cn/Article/details/gcshkuskd.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://baike.zdbjq.cn/Article/details/gbmhxosxe.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://read.share.hesvh.cn/Article/details/gyxwaabfs.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://baike.hesvh.cn/Article/details/gghscwpqm.sHtML

TS:   arr.splice(0, 1);
来源：http://m.share.hesvh.cn/Article/details/gdtaaeojt.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://m.share.fehbvm.com/Article/details/gsvbpcsug.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mobile.zdbjq.cn/Article/details/gbiqelskp.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://3g.zdbjq.cn/Article/details/gsdrmanvd.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://blog.zdbjq.cn/Article/details/ggjubvbub.sHtML

[D05] 访问与修改元素
来源：http://www.m.share.hesvh.cn/Article/details/gcmsmqjya.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.hesvh.cn/Article/details/gzuyktvoy.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://blog.hesvh.cn/Article/details/gtnajgtjc.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://read.share.hesvh.cn/Article/details/gqmgayptk.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://m.share.zdbjq.cn/Article/details/ggajyaelo.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://blog.fehbvm.com/Article/details/gsqurborv.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://3g.hesvh.cn/Article/details/gfnpzqwup.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.zdbjq.cn/Article/details/gureiglrj.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.blog.fehbvm.com/Article/details/gskexkhus.sHtML

[D06] 数组长度
来源：http://read.share.fehbvm.com/Article/details/gtpehczes.sHtML

Py:   len(arr)
来源：http://3g.hesvh.cn/Article/details/gutwckkhl.sHtML

PHP:  count($arr);
来源：http://wap.zdbjq.cn/Article/details/gkrubafhq.sHtML

JS:   arr.length
来源：http://blog.zdbjq.cn/Article/details/gajdvgcjn.sHtML

TS:   arr.length
来源：http://www.m.share.zdbjq.cn/Article/details/gtzwfrdgw.sHtML

Java: list.size();
来源：http://www.blog.hesvh.cn/Article/details/gmfvfixzg.sHtML

Go:   len(arr)
来源：http://www.share.hesvh.cn/Article/details/gzvheipnj.sHtML

Ruby: arr.length; arr.size
来源：http://baike.hesvh.cn/Article/details/gygiuvvrk.sHtML

C#:   list.Count;
来源：http://wap.hesvh.cn/Article/details/gnaddhoyp.sHtML


<!-- 参考信息 -->