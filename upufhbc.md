代发 wailian999

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://baike.hesvh.cn/Article/details/gdtciwjra.sHtML

[B06] 遍历字典 / 对象
来源：http://www.share.hesvh.cn/Article/details/gyuhsoskw.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.share.fehbvm.com/Article/details/gllkooegz.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://3g.fehbvm.com/Article/details/gdvhcxmkw.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.blog.zdbjq.cn/Article/details/gcxluwzsf.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://3g.fehbvm.com/Article/details/gdjtliyky.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://wap.zdbjq.cn/Article/details/gtluwqvoi.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://wap.hesvh.cn/Article/details/gkjemjuom.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://3g.hesvh.cn/Article/details/glyyqxzbv.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://wap.fehbvm.com/Article/details/gfsdkitjo.sHtML

[B07] while 循环
来源：http://mobile.hesvh.cn/Article/details/gsuzfehru.sHtML

Py:   while i < 10: i += 1
来源：http://read.share.fehbvm.com/Article/details/gsxsuonoj.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.blog.zdbjq.cn/Article/details/gpyzxjjaa.sHtML

JS:   while (i < 10) { i++; }
来源：http://wap.hesvh.cn/Article/details/gxkijxexk.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.blog.hesvh.cn/Article/details/ggjrfqfan.sHtML

Java: while (i < 10) { i++; }
来源：http://www.share.fehbvm.com/Article/details/gfzxevxcd.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.blog.fehbvm.com/Article/details/gazdxuumf.sHtML

Ruby: while i < 10; i += 1; end
来源：http://mobile.hesvh.cn/Article/details/glytabide.sHtML

C#:   while (i < 10) { i++; }
来源：http://baike.hesvh.cn/Article/details/gwmhddfqp.sHtML

[B08] do-while（至少执行一次）
来源：http://m.share.hesvh.cn/Article/details/girfosypv.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.m.share.fehbvm.com/Article/details/glhssnrfv.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://wap.zdbjq.cn/Article/details/gowwtxenw.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.share.zdbjq.cn/Article/details/greomuwov.sHtML

TS:   do { i++; } while (i < 10);
来源：http://3g.hesvh.cn/Article/details/gddnggscq.sHtML

Java: do { i++; } while (i < 10);
来源：http://read.share.zdbjq.cn/Article/details/gryjvdcrh.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://wap.hesvh.cn/Article/details/gvqiaiaml.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://3g.zdbjq.cn/Article/details/gixchnwtr.sHtML

C#:   do { i++; } while (i < 10);
来源：http://read.share.zdbjq.cn/Article/details/gpwdentyv.sHtML

[B09] break 与 continue
来源：http://3g.hesvh.cn/Article/details/gymhcrawk.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://m.share.fehbvm.com/Article/details/gpqzxbfei.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://m.share.fehbvm.com/Article/details/gptjrjqwo.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.zdbjq.cn/Article/details/gxzguuiiw.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.fehbvm.com/Article/details/gqtooovih.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.zdbjq.cn/Article/details/gimnsufkd.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://m.share.zdbjq.cn/Article/details/glwzrqxpt.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.share.zdbjq.cn/Article/details/glbvlppgr.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.hesvh.cn/Article/details/gcbqqjlqg.sHtML

[B10] 遍历同时拿索引
来源：http://baike.hesvh.cn/Article/details/gdchihocc.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://blog.fehbvm.com/Article/details/gyhrqwuos.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.blog.fehbvm.com/Article/details/ghvxidrbe.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://wap.zdbjq.cn/Article/details/gygjyslcc.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://mobile.hesvh.cn/Article/details/gpmcchgou.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://blog.zdbjq.cn/Article/details/ginxqmlov.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://mobile.hesvh.cn/Article/details/gvadtoefx.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://m.share.hesvh.cn/Article/details/gijjfnuhl.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://read.share.fehbvm.com/Article/details/gjwdpzzlx.sHtML

[B11] 生成数字序列 / 区间
来源：http://m.share.hesvh.cn/Article/details/gbvbqdkyg.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.m.share.fehbvm.com/Article/details/gwejmzkvk.sHtML

PHP:  range(0, 10, 2);
来源：http://www.blog.zdbjq.cn/Article/details/gmqzqilcs.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://baike.zdbjq.cn/Article/details/ggqqhvjht.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.blog.fehbvm.com/Article/details/gsljantdd.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.blog.fehbvm.com/Article/details/gltrkrclp.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://baike.hesvh.cn/Article/details/gyajffhcg.sHtML

Ruby: (0...10).step(2).to_a
来源：http://mobile.hesvh.cn/Article/details/gjqaqfeta.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://3g.fehbvm.com/Article/details/gldncxpdx.sHtML

[B12] 跳出多层循环
来源：http://mobile.hesvh.cn/Article/details/gewujuusb.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://read.share.zdbjq.cn/Article/details/gcezzqsxj.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://baike.zdbjq.cn/Article/details/gtgscocvs.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://read.share.zdbjq.cn/Article/details/gfpgdaehx.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://3g.fehbvm.com/Article/details/gknnaydxz.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.zdbjq.cn/Article/details/glhqmjlje.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://m.share.fehbvm.com/Article/details/ghbvoolxu.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://baike.fehbvm.com/Article/details/gorekbkje.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://blog.fehbvm.com/Article/details/gabicqkke.sHtML

[B13] 判断是否为数字
来源：http://blog.zdbjq.cn/Article/details/ghrezajnb.sHtML

Py:   isinstance(x, (int, float))
来源：http://baike.hesvh.cn/Article/details/gtydlanev.sHtML

PHP:  is_numeric($x)
来源：http://baike.fehbvm.com/Article/details/gueipcvaf.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://3g.hesvh.cn/Article/details/gzhkxqavh.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.blog.zdbjq.cn/Article/details/gweemlcko.sHtML

Java: x instanceof Number
来源：http://www.blog.hesvh.cn/Article/details/gyhpeushg.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://m.share.hesvh.cn/Article/details/gnjisbiyx.sHtML

Ruby: x.is_a?(Numeric)
来源：http://read.share.zdbjq.cn/Article/details/gerbceuum.sHtML

C#:   x is int or double or decimal
来源：http://www.share.hesvh.cn/Article/details/gkwxuazny.sHtML

[B14] 判断值是否在集合内
来源：http://read.share.hesvh.cn/Article/details/gfrhujkct.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.share.zdbjq.cn/Article/details/gegwmokkk.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://wap.hesvh.cn/Article/details/glrwpenjg.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.blog.fehbvm.com/Article/details/gcqakzfat.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://baike.zdbjq.cn/Article/details/guwhijeqb.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://baike.fehbvm.com/Article/details/gfylthdrt.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://read.share.zdbjq.cn/Article/details/gwbmkhlyj.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.m.share.hesvh.cn/Article/details/gnbtpobej.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://baike.hesvh.cn/Article/details/gfjblnkqp.sHtML

[B15] 布尔运算与取反
来源：http://www.share.zdbjq.cn/Article/details/gnauvdfeb.sHtML

Py:   a and b or not c
来源：http://mobile.fehbvm.com/Article/details/gxpoizqxe.sHtML

PHP:  $a && $b || !$c
来源：http://read.share.hesvh.cn/Article/details/gwzmrgzwn.sHtML

JS:   a && b || !c
来源：http://3g.hesvh.cn/Article/details/gejkxihku.sHtML

TS:   a && b || !c
来源：http://m.share.fehbvm.com/Article/details/gvkhsoaow.sHtML

Java: a && b || !c
来源：http://baike.fehbvm.com/Article/details/gdamhdwts.sHtML

Go:   a && b || !c
来源：http://baike.fehbvm.com/Article/details/gxnceofdo.sHtML

Ruby: a && b || !c
来源：http://blog.zdbjq.cn/Article/details/glshxznkd.sHtML

C#:   a && b || !c
来源：http://wap.hesvh.cn/Article/details/glgedqgrc.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://3g.fehbvm.com/Article/details/gzhrxeplq.sHtML

Py:   if not data: return
来源：http://mobile.hesvh.cn/Article/details/gdjyzbnzk.sHtML

PHP:  if (!$data) { return; }
来源：http://blog.hesvh.cn/Article/details/gbsxkcsvr.sHtML

JS:   if (!data) return;
来源：http://www.blog.zdbjq.cn/Article/details/glszjahrq.sHtML

TS:   if (!data) return;
来源：http://baike.zdbjq.cn/Article/details/gwuwfqijq.sHtML

Java: if (data == null) return;
来源：http://read.share.fehbvm.com/Article/details/gowvbcqfb.sHtML

Go:   if data == nil { return }
来源：http://3g.hesvh.cn/Article/details/gytrgfenr.sHtML

Ruby: return if data.nil?
来源：http://baike.zdbjq.cn/Article/details/gabrbmqju.sHtML

C#:   if (data == null) return;
来源：http://read.share.zdbjq.cn/Article/details/giuerctid.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gfzkaivyo.sHtML

C. 函数与作用域
来源：http://www.m.share.fehbvm.com/Article/details/glciuocbh.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gqqqputpi.sHtML

[C01] 定义函数
来源：http://wap.zdbjq.cn/Article/details/gsxhvablw.sHtML

Py:   def add(a, b): return a + b
来源：http://3g.zdbjq.cn/Article/details/gcwrenisz.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.zdbjq.cn/Article/details/giubqnhic.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.blog.hesvh.cn/Article/details/gkfknptbk.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.hesvh.cn/Article/details/gvvlxargt.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://m.share.fehbvm.com/Article/details/gmmkpfjxw.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://3g.hesvh.cn/Article/details/gbrppamwq.sHtML

Ruby: def add(a, b); a + b; end
来源：http://blog.zdbjq.cn/Article/details/gjgsxmbyz.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://blog.hesvh.cn/Article/details/gqmjyggoo.sHtML

[C02] 默认参数
来源：http://www.blog.hesvh.cn/Article/details/gtxckmhqo.sHtML

Py:   def greet(name="World"): return name
来源：http://baike.hesvh.cn/Article/details/gpfdljmrg.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://mobile.hesvh.cn/Article/details/gernxasgh.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://read.share.fehbvm.com/Article/details/gynwbwqin.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://m.share.fehbvm.com/Article/details/gspyyocex.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://baike.zdbjq.cn/Article/details/gjsnozicd.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wap.hesvh.cn/Article/details/gwwemwfcs.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.share.fehbvm.com/Article/details/gdjxghjib.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://mobile.fehbvm.com/Article/details/gtshoqhcl.sHtML

[C03] 可变参数
来源：http://read.share.fehbvm.com/Article/details/guetkxgpy.sHtML

Py:   def total(*args): return sum(args)
来源：http://3g.fehbvm.com/Article/details/gazvxuoqa.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://read.share.fehbvm.com/Article/details/gapekmlxm.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.zdbjq.cn/Article/details/gjnenzuka.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.zdbjq.cn/Article/details/gfebpfhwu.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://mobile.fehbvm.com/Article/details/guevnfode.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://read.share.zdbjq.cn/Article/details/gwrohgxbx.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://mobile.zdbjq.cn/Article/details/ghakxjjiv.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://read.share.hesvh.cn/Article/details/gsjnytzik.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.share.hesvh.cn/Article/details/guvkdqiic.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://read.share.zdbjq.cn/Article/details/grdxmddhq.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://m.share.zdbjq.cn/Article/details/ghersbbgc.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.share.hesvh.cn/Article/details/gbzbtkvsl.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.share.zdbjq.cn/Article/details/gbgdvkixh.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.m.share.hesvh.cn/Article/details/gnpfphinn.sHtML

Go:   // 无：用配置结构体参数
来源：http://blog.zdbjq.cn/Article/details/gbfumlwev.sHtML

Ruby: f(a: 1, b: 2)
来源：http://3g.hesvh.cn/Article/details/gyqdysolx.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.share.fehbvm.com/Article/details/gmpoflbxj.sHtML

[C05] 返回多个值
来源：http://blog.zdbjq.cn/Article/details/gnbjvcbsa.sHtML

Py:   return a, b
来源：http://mobile.hesvh.cn/Article/details/gaanyqyfz.sHtML

PHP:  return [$a, $b];
来源：http://mobile.zdbjq.cn/Article/details/geenzmlco.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://m.share.zdbjq.cn/Article/details/gbxqqfqxk.sHtML

TS:   return { a, b };
来源：http://mobile.zdbjq.cn/Article/details/gdclbnspe.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://wap.hesvh.cn/Article/details/gkfhlmszk.sHtML

Go:   return a, b
来源：http://mobile.zdbjq.cn/Article/details/gmrgtvwwc.sHtML

Ruby: return a, b
来源：http://wap.hesvh.cn/Article/details/gthyothmu.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://wap.zdbjq.cn/Article/details/gjcwyuobx.sHtML

[C06] 匿名函数 / lambda
来源：http://baike.hesvh.cn/Article/details/gsdezilgr.sHtML

Py:   square = lambda x: x * x
来源：http://baike.fehbvm.com/Article/details/gragoeeqi.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.blog.zdbjq.cn/Article/details/gwwqhfava.sHtML

JS:   const square = x => x * x;
来源：http://blog.fehbvm.com/Article/details/gubmcrpqs.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://read.share.fehbvm.com/Article/details/gqaoeitme.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.share.fehbvm.com/Article/details/gfuavycvi.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.share.fehbvm.com/Article/details/gihasfkjg.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.share.fehbvm.com/Article/details/ggnrisxad.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://mobile.zdbjq.cn/Article/details/grjnlanma.sHtML

[C07] 把函数作为参数传入
来源：http://wap.fehbvm.com/Article/details/gighrezkh.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://read.share.zdbjq.cn/Article/details/gywklwlzj.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://read.share.zdbjq.cn/Article/details/gmhdqfkhd.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://read.share.hesvh.cn/Article/details/gjqjtjlxn.sHtML

TS:   arr.map(String)
来源：http://wap.zdbjq.cn/Article/details/govxwvzmp.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.m.share.fehbvm.com/Article/details/gqkovpyci.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.m.share.fehbvm.com/Article/details/gzwopbtao.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.share.hesvh.cn/Article/details/gccwzphwq.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://wap.hesvh.cn/Article/details/gqswrbvwy.sHtML

[C08] 闭包
来源：http://www.blog.hesvh.cn/Article/details/gpkywobfo.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://mobile.zdbjq.cn/Article/details/gcuudlusy.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.m.share.fehbvm.com/Article/details/gsqfpzspz.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.share.fehbvm.com/Article/details/gtmzfixgv.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://mobile.hesvh.cn/Article/details/gzyqpkbbq.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.share.fehbvm.com/Article/details/gqbejbrxt.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://baike.fehbvm.com/Article/details/gayomxrsk.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://mobile.fehbvm.com/Article/details/geoxogtqw.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.share.hesvh.cn/Article/details/gzjctzete.sHtML

[C09] 递归
来源：http://www.blog.fehbvm.com/Article/details/gaapsfiqm.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://wap.zdbjq.cn/Article/details/gytnftqhf.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://3g.zdbjq.cn/Article/details/gxfxfxdkk.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.zdbjq.cn/Article/details/glhauondp.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.fehbvm.com/Article/details/ggzyoxkqs.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://baike.hesvh.cn/Article/details/golwkokpo.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://3g.fehbvm.com/Article/details/gekiepsbt.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://blog.hesvh.cn/Article/details/gafhgyhcw.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://read.share.hesvh.cn/Article/details/gqlrsgngo.sHtML

[C10] 变量作用域
来源：http://www.blog.zdbjq.cn/Article/details/grymrkddj.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://mobile.zdbjq.cn/Article/details/gmbpqpztn.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://wap.fehbvm.com/Article/details/gbpyarpwk.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://blog.hesvh.cn/Article/details/gyfywpmqs.sHtML

TS:   同 JS
来源：http://www.share.fehbvm.com/Article/details/gakpumydg.sHtML

Java: 方法内为块级作用域
来源：http://www.share.zdbjq.cn/Article/details/gxxofrlxc.sHtML

Go:   花括号块级作用域
来源：http://m.share.zdbjq.cn/Article/details/gskrggsan.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.share.zdbjq.cn/Article/details/gyhikwqlc.sHtML

C#:   块级作用域
来源：http://www.share.fehbvm.com/Article/details/gioxnlazi.sHtML

[C11] 模块导入与导出
来源：http://www.m.share.fehbvm.com/Article/details/gzbuugdup.sHtML

Py:   from module import func
来源：http://mobile.zdbjq.cn/Article/details/gsvmeidjw.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://mobile.fehbvm.com/Article/details/geoqujbpt.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://m.share.fehbvm.com/Article/details/gaakbdldf.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://3g.zdbjq.cn/Article/details/gqtwemtyt.sHtML

Java: import java.util.List;
来源：http://www.share.hesvh.cn/Article/details/gmajilwnu.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.share.zdbjq.cn/Article/details/gyzxhgzyo.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://blog.fehbvm.com/Article/details/gwcefwwvb.sHtML

C#:   using System.Text;
来源：http://mobile.hesvh.cn/Article/details/gxekpsedr.sHtML

[C12] 立即执行函数 IIFE
来源：http://baike.zdbjq.cn/Article/details/gaxooqdzr.sHtML

Py:   (lambda: print("run"))()
来源：http://read.share.hesvh.cn/Article/details/gkpsfajny.sHtML

PHP:  (function () { echo "run"; })();
来源：http://m.share.hesvh.cn/Article/details/gvikbkgen.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.blog.fehbvm.com/Article/details/gyftzjhdo.sHtML

TS:   (() => { console.log("run"); })();
来源：http://wap.fehbvm.com/Article/details/gbjskupaz.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.blog.fehbvm.com/Article/details/gnvsryibx.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.blog.zdbjq.cn/Article/details/gxnfkljfx.sHtML

Ruby: -> { puts "run" }.call
来源：http://3g.fehbvm.com/Article/details/gxzizbizp.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://blog.zdbjq.cn/Article/details/gaijvvdsu.sHtML

[C13] 类型声明 / 类型注解
来源：http://3g.fehbvm.com/Article/details/goypsurtm.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://mobile.fehbvm.com/Article/details/gbhkkvris.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.fehbvm.com/Article/details/gjwodaqkh.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.share.hesvh.cn/Article/details/guvtcqvso.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.hesvh.cn/Article/details/ggmnqcttp.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://baike.fehbvm.com/Article/details/gydsrzryx.sHtML

Go:   func add(a, b int) int
来源：http://www.share.hesvh.cn/Article/details/gjrhubszs.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.m.share.zdbjq.cn/Article/details/gksjkorcb.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://baike.hesvh.cn/Article/details/glsicfqvu.sHtML

[C14] 泛型函数
来源：http://www.blog.hesvh.cn/Article/details/gubehryww.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://3g.hesvh.cn/Article/details/guchxqhbp.sHtML

PHP:  // 无泛型
来源：http://m.share.zdbjq.cn/Article/details/gdqpicflk.sHtML

JS:   // 无泛型
来源：http://blog.zdbjq.cn/Article/details/gchsxsxle.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.m.share.fehbvm.com/Article/details/gpwvgzeie.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.share.fehbvm.com/Article/details/gmtcndxjh.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.share.fehbvm.com/Article/details/gjiltokhc.sHtML

Ruby: # 无泛型
来源：http://baike.fehbvm.com/Article/details/gblwyumwr.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://read.share.zdbjq.cn/Article/details/gdayfzhew.sHtML

[C15] 解构 / 展开参数
来源：http://www.share.fehbvm.com/Article/details/gpjoozudl.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.blog.fehbvm.com/Article/details/gswlimsnq.sHtML

PHP:  [$a, $b] = $pair;
来源：http://blog.zdbjq.cn/Article/details/gjkrjsvsv.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.share.hesvh.cn/Article/details/gnzpbwztz.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gqvvqiqdl.sHtML

Java: // 无解构
来源：http://wap.zdbjq.cn/Article/details/gnrljarvk.sHtML

Go:   // 无解构
来源：http://m.share.fehbvm.com/Article/details/gdyiqdred.sHtML

Ruby: a, b = pair
来源：http://baike.fehbvm.com/Article/details/gnfodaoub.sHtML

C#:   var (a, b) = pair;
来源：http://wap.hesvh.cn/Article/details/gnbbmkixr.sHtML

[C16] 函数 / 方法重载
来源：http://www.blog.zdbjq.cn/Article/details/gyqkjsjab.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://mobile.fehbvm.com/Article/details/gogppeady.sHtML

PHP:  // 无重载
来源：http://read.share.hesvh.cn/Article/details/gklubhwws.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://baike.fehbvm.com/Article/details/gsyhryglk.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://m.share.hesvh.cn/Article/details/gklaewygx.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.m.share.fehbvm.com/Article/details/gugqnwdjy.sHtML

Go:   // 无重载：用不同函数名
来源：http://wap.fehbvm.com/Article/details/gwdarsclu.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.share.hesvh.cn/Article/details/gqempmmhq.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://mobile.zdbjq.cn/Article/details/gefralssq.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gplieeyqx.sHtML

D. 数组 / 列表 / 集合
来源：http://www.m.share.fehbvm.com/Article/details/gjonowdzb.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gaoxqkzij.sHtML

[D01] 创建数组 / 列表
来源：http://m.share.zdbjq.cn/Article/details/grivfmyry.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://blog.zdbjq.cn/Article/details/gcklpyxqm.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://blog.fehbvm.com/Article/details/gudipviub.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://blog.hesvh.cn/Article/details/gyokhkjeb.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://wap.hesvh.cn/Article/details/gteszzjkv.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://read.share.zdbjq.cn/Article/details/gkbsgsrzw.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://wap.fehbvm.com/Article/details/gkolmyrkx.sHtML

Ruby: arr = [1, 2, 3]
来源：http://mobile.fehbvm.com/Article/details/gwnkucbbm.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://3g.hesvh.cn/Article/details/grlkzihuo.sHtML

[D02] 追加元素到末尾
来源：http://www.share.hesvh.cn/Article/details/gkirpqtje.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.share.zdbjq.cn/Article/details/gplbgjnbb.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.share.fehbvm.com/Article/details/gkjlqpghl.sHtML

JS:   arr.push(4);
来源：http://3g.hesvh.cn/Article/details/gchvdzhct.sHtML

TS:   arr.push(4);
来源：http://baike.fehbvm.com/Article/details/gbwsshhwb.sHtML

Java: list.add(4);
来源：http://m.share.fehbvm.com/Article/details/gbvtdqbrl.sHtML

Go:   arr = append(arr, 4)
来源：http://www.m.share.hesvh.cn/Article/details/gnjphdgua.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://m.share.zdbjq.cn/Article/details/giwcejuxf.sHtML

C#:   list.Add(4);
来源：http://wap.zdbjq.cn/Article/details/gvnwmfbfa.sHtML

[D03] 在指定位置插入元素
来源：http://www.m.share.zdbjq.cn/Article/details/guscguklb.sHtML

Py:   arr.insert(0, 0)
来源：http://3g.fehbvm.com/Article/details/glfyfepon.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://blog.fehbvm.com/Article/details/gachbqdyy.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://mobile.fehbvm.com/Article/details/gicpazmxu.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://read.share.hesvh.cn/Article/details/gcgswmkgv.sHtML

Java: list.add(0, 0);
来源：http://wap.fehbvm.com/Article/details/gghsljikm.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.blog.fehbvm.com/Article/details/giawwzmkn.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.m.share.zdbjq.cn/Article/details/gsyaztzuo.sHtML

C#:   list.Insert(0, 0);
来源：http://blog.hesvh.cn/Article/details/gbjcbjqbi.sHtML

[D04] 删除元素
来源：http://3g.zdbjq.cn/Article/details/gahtwrcyp.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://3g.fehbvm.com/Article/details/gsjblnqxv.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mobile.fehbvm.com/Article/details/ghqmgrodw.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mobile.hesvh.cn/Article/details/gsvhqfbsx.sHtML

TS:   arr.splice(0, 1);
来源：http://3g.hesvh.cn/Article/details/geagaglbt.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mobile.hesvh.cn/Article/details/govnroazx.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://m.share.zdbjq.cn/Article/details/gfszazbzv.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.m.share.zdbjq.cn/Article/details/gszopapfr.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.share.zdbjq.cn/Article/details/gvxomycwq.sHtML

[D05] 访问与修改元素
来源：http://m.share.fehbvm.com/Article/details/glqdwnixr.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.hesvh.cn/Article/details/gfrpinfdx.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.blog.fehbvm.com/Article/details/gdhaoxwxm.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://m.share.zdbjq.cn/Article/details/gvbgjmhbv.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://mobile.fehbvm.com/Article/details/grfueovay.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://baike.hesvh.cn/Article/details/gddalkkaq.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.blog.hesvh.cn/Article/details/gizvpwtis.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.fehbvm.com/Article/details/gicoetllu.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.m.share.hesvh.cn/Article/details/gsubcgfsd.sHtML

[D06] 数组长度
来源：http://www.blog.fehbvm.com/Article/details/ghgqjopyg.sHtML

Py:   len(arr)
来源：http://www.share.fehbvm.com/Article/details/gngcibppg.sHtML

PHP:  count($arr);
来源：http://www.blog.zdbjq.cn/Article/details/ghcaxcdct.sHtML

JS:   arr.length
来源：http://www.blog.zdbjq.cn/Article/details/gnciwzjnt.sHtML

TS:   arr.length
来源：http://mobile.fehbvm.com/Article/details/gfiphqhbm.sHtML


<!-- 参考信息 -->