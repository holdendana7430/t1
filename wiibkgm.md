代发 wailian999

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://blog.hesvh.cn/Article/details/grkrzzwkm.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://3g.fehbvm.com/Article/details/ghunpcnfn.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://mobile.fehbvm.com/Article/details/gocbiksyq.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.m.share.fehbvm.com/Article/details/gsuffapwp.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://mobile.fehbvm.com/Article/details/gihtktock.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://mobile.hesvh.cn/Article/details/ggguanjmw.sHtML

[B07] while 循环
来源：http://read.share.zdbjq.cn/Article/details/giilhpbjm.sHtML

Py:   while i < 10: i += 1
来源：http://www.m.share.hesvh.cn/Article/details/gibuazxcs.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://baike.zdbjq.cn/Article/details/gleglvtvv.sHtML

JS:   while (i < 10) { i++; }
来源：http://baike.fehbvm.com/Article/details/glncfmjbr.sHtML

TS:   while (i < 10) { i++; }
来源：http://m.share.zdbjq.cn/Article/details/gaabvansk.sHtML

Java: while (i < 10) { i++; }
来源：http://baike.fehbvm.com/Article/details/gwitrzwhw.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://baike.zdbjq.cn/Article/details/gxhszlpva.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.share.fehbvm.com/Article/details/gyjgtbirh.sHtML

C#:   while (i < 10) { i++; }
来源：http://3g.hesvh.cn/Article/details/gthtwoazp.sHtML

[B08] do-while（至少执行一次）
来源：http://mobile.hesvh.cn/Article/details/gskebfvyp.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.m.share.fehbvm.com/Article/details/ggvajzlzj.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://mobile.zdbjq.cn/Article/details/gvurhwveg.sHtML

JS:   do { i++; } while (i < 10);
来源：http://m.share.fehbvm.com/Article/details/gzcjnsxae.sHtML

TS:   do { i++; } while (i < 10);
来源：http://baike.hesvh.cn/Article/details/gjlqmdltm.sHtML

Java: do { i++; } while (i < 10);
来源：http://read.share.zdbjq.cn/Article/details/gxwwsiiiw.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://blog.zdbjq.cn/Article/details/gkppifqgg.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.blog.hesvh.cn/Article/details/gxanzbbaf.sHtML

C#:   do { i++; } while (i < 10);
来源：http://read.share.zdbjq.cn/Article/details/gbchznkie.sHtML

[B09] break 与 continue
来源：http://read.share.hesvh.cn/Article/details/gnkqcthyv.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://blog.fehbvm.com/Article/details/gogpykrrx.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://read.share.hesvh.cn/Article/details/gftrlontn.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.zdbjq.cn/Article/details/gworleuef.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.fehbvm.com/Article/details/gcwpxwrrb.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.zdbjq.cn/Article/details/gjemylfzy.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://read.share.fehbvm.com/Article/details/guvefpnof.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://3g.zdbjq.cn/Article/details/gxfnzummb.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.zdbjq.cn/Article/details/gykajeomx.sHtML

[B10] 遍历同时拿索引
来源：http://m.share.fehbvm.com/Article/details/gskycwpfy.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://wap.fehbvm.com/Article/details/ggscnvytq.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://mobile.hesvh.cn/Article/details/gcwvdxxbp.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.m.share.fehbvm.com/Article/details/geodhhzjj.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.m.share.zdbjq.cn/Article/details/gjnolgklv.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://baike.fehbvm.com/Article/details/gxlbdgoef.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.m.share.fehbvm.com/Article/details/grsdlmdnm.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://blog.zdbjq.cn/Article/details/ghhhqizqg.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.blog.hesvh.cn/Article/details/gxwcazbtx.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.blog.hesvh.cn/Article/details/grsslccnx.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.share.zdbjq.cn/Article/details/gbzqqkluh.sHtML

PHP:  range(0, 10, 2);
来源：http://wap.hesvh.cn/Article/details/gfbxhmeon.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://m.share.hesvh.cn/Article/details/gnsgixsxw.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://m.share.hesvh.cn/Article/details/gaehsuhac.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.share.zdbjq.cn/Article/details/gdqoskhwv.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://wap.fehbvm.com/Article/details/gkfwivrtn.sHtML

Ruby: (0...10).step(2).to_a
来源：http://m.share.zdbjq.cn/Article/details/gotuaiujy.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://blog.hesvh.cn/Article/details/gucpyvcua.sHtML

[B12] 跳出多层循环
来源：http://blog.hesvh.cn/Article/details/gqgahnmgg.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://m.share.hesvh.cn/Article/details/gvloufwdv.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://baike.fehbvm.com/Article/details/gnkzygooi.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://m.share.fehbvm.com/Article/details/gabfxmsvh.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.fehbvm.com/Article/details/gpjcqxwyx.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://read.share.fehbvm.com/Article/details/gieevyyca.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://baike.zdbjq.cn/Article/details/gztgpxhef.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.m.share.hesvh.cn/Article/details/gdfbpmwfe.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://read.share.zdbjq.cn/Article/details/gfcjoxiex.sHtML

[B13] 判断是否为数字
来源：http://www.share.hesvh.cn/Article/details/gevtxxuxm.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.m.share.fehbvm.com/Article/details/gxgumwcxr.sHtML

PHP:  is_numeric($x)
来源：http://www.blog.hesvh.cn/Article/details/gfphmmqvb.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.hesvh.cn/Article/details/gsvhsfufv.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.fehbvm.com/Article/details/ggaxnjrmj.sHtML

Java: x instanceof Number
来源：http://www.share.hesvh.cn/Article/details/gfecsimzg.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.m.share.fehbvm.com/Article/details/ghkiphnbr.sHtML

Ruby: x.is_a?(Numeric)
来源：http://read.share.zdbjq.cn/Article/details/gobiehxvr.sHtML

C#:   x is int or double or decimal
来源：http://read.share.fehbvm.com/Article/details/gxhjkogcv.sHtML

[B14] 判断值是否在集合内
来源：http://www.blog.hesvh.cn/Article/details/gmmxmanzv.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.m.share.zdbjq.cn/Article/details/gbcnxptlg.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://mobile.fehbvm.com/Article/details/ghzqlgvti.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://baike.hesvh.cn/Article/details/gqoejgjwb.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.blog.zdbjq.cn/Article/details/gxflcnhol.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://3g.fehbvm.com/Article/details/gfkclvhkb.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://3g.zdbjq.cn/Article/details/goqkixhgw.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.m.share.zdbjq.cn/Article/details/glxdequem.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.m.share.fehbvm.com/Article/details/gmnbnmxtv.sHtML

[B15] 布尔运算与取反
来源：http://baike.fehbvm.com/Article/details/gqcabztbi.sHtML

Py:   a and b or not c
来源：http://www.share.fehbvm.com/Article/details/gnnwosbwx.sHtML

PHP:  $a && $b || !$c
来源：http://3g.zdbjq.cn/Article/details/glwdvwewv.sHtML

JS:   a && b || !c
来源：http://m.share.hesvh.cn/Article/details/gtqsbkyoa.sHtML

TS:   a && b || !c
来源：http://mobile.fehbvm.com/Article/details/gsctedndv.sHtML

Java: a && b || !c
来源：http://wap.fehbvm.com/Article/details/gpszlskvw.sHtML

Go:   a && b || !c
来源：http://baike.hesvh.cn/Article/details/giwolwdwg.sHtML

Ruby: a && b || !c
来源：http://www.m.share.zdbjq.cn/Article/details/gxyzbbbky.sHtML

C#:   a && b || !c
来源：http://3g.zdbjq.cn/Article/details/gljwgdkjv.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://mobile.zdbjq.cn/Article/details/gphlwhaeo.sHtML

Py:   if not data: return
来源：http://www.m.share.zdbjq.cn/Article/details/gwyuguctq.sHtML

PHP:  if (!$data) { return; }
来源：http://wap.hesvh.cn/Article/details/gpjwagvto.sHtML

JS:   if (!data) return;
来源：http://blog.fehbvm.com/Article/details/gfevlolvu.sHtML

TS:   if (!data) return;
来源：http://blog.zdbjq.cn/Article/details/gdhckwvqy.sHtML

Java: if (data == null) return;
来源：http://www.m.share.hesvh.cn/Article/details/ggohmblty.sHtML

Go:   if data == nil { return }
来源：http://baike.hesvh.cn/Article/details/gqdpdjlwo.sHtML

Ruby: return if data.nil?
来源：http://blog.hesvh.cn/Article/details/gwdltxstk.sHtML

C#:   if (data == null) return;
来源：http://www.share.hesvh.cn/Article/details/gtwxykhdw.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gjerdmnsc.sHtML

C. 函数与作用域
来源：http://3g.fehbvm.com/Article/details/gbqcvugxo.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gywsvbptk.sHtML

[C01] 定义函数
来源：http://www.share.zdbjq.cn/Article/details/gtavgczmr.sHtML

Py:   def add(a, b): return a + b
来源：http://m.share.fehbvm.com/Article/details/gvgazppcr.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.fehbvm.com/Article/details/girkosqnl.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://read.share.hesvh.cn/Article/details/glvjzveme.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.fehbvm.com/Article/details/gctiwypju.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.m.share.hesvh.cn/Article/details/gbrijwpzo.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.share.zdbjq.cn/Article/details/gudwzxkim.sHtML

Ruby: def add(a, b); a + b; end
来源：http://blog.fehbvm.com/Article/details/gmegvimen.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://wap.fehbvm.com/Article/details/gkzzfbpod.sHtML

[C02] 默认参数
来源：http://blog.zdbjq.cn/Article/details/gxrbyhayk.sHtML

Py:   def greet(name="World"): return name
来源：http://blog.fehbvm.com/Article/details/gcrwugrik.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.blog.hesvh.cn/Article/details/ggkqpvbci.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://baike.hesvh.cn/Article/details/gixmkwsgr.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://m.share.zdbjq.cn/Article/details/gapguaxdy.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://mobile.fehbvm.com/Article/details/gazsgwtyt.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://mobile.fehbvm.com/Article/details/gwmccpxpz.sHtML

Ruby: def greet(name = "World") = name
来源：http://wap.zdbjq.cn/Article/details/gokfrizef.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://m.share.zdbjq.cn/Article/details/gmgcnijag.sHtML

[C03] 可变参数
来源：http://m.share.fehbvm.com/Article/details/gxrcpymha.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.m.share.fehbvm.com/Article/details/gqjeexsyp.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.share.fehbvm.com/Article/details/gtpnacdaj.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.zdbjq.cn/Article/details/gycfinpts.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.fehbvm.com/Article/details/guzkzfwkt.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.share.zdbjq.cn/Article/details/gzqraduzb.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://mobile.hesvh.cn/Article/details/giiaopwpc.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://wap.fehbvm.com/Article/details/gmdqcyvhr.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.blog.zdbjq.cn/Article/details/gqpciamsc.sHtML

[C04] 命名参数 / 关键字参数
来源：http://blog.hesvh.cn/Article/details/gunjnapvt.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://m.share.hesvh.cn/Article/details/gqtrsgimj.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://3g.fehbvm.com/Article/details/gjjbrgfef.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://wap.hesvh.cn/Article/details/grvnnbqzj.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://m.share.zdbjq.cn/Article/details/gjjtwxxuq.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://m.share.hesvh.cn/Article/details/gzwlmdspo.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.m.share.zdbjq.cn/Article/details/ghzmtxoit.sHtML

Ruby: f(a: 1, b: 2)
来源：http://mobile.hesvh.cn/Article/details/gqrufrmbo.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gzdhwyshf.sHtML

[C05] 返回多个值
来源：http://mobile.zdbjq.cn/Article/details/gekmfgrxr.sHtML

Py:   return a, b
来源：http://wap.zdbjq.cn/Article/details/gwulugrao.sHtML

PHP:  return [$a, $b];
来源：http://www.blog.fehbvm.com/Article/details/gvxpzsvbx.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://baike.fehbvm.com/Article/details/gnbsvkvzb.sHtML

TS:   return { a, b };
来源：http://wap.fehbvm.com/Article/details/ghbanwxwq.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://baike.hesvh.cn/Article/details/gzzrluatl.sHtML

Go:   return a, b
来源：http://baike.zdbjq.cn/Article/details/gcdegwyqo.sHtML

Ruby: return a, b
来源：http://baike.fehbvm.com/Article/details/gibfuttxi.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://3g.fehbvm.com/Article/details/gwavtiezj.sHtML

[C06] 匿名函数 / lambda
来源：http://www.share.hesvh.cn/Article/details/gqafyoyzr.sHtML

Py:   square = lambda x: x * x
来源：http://www.m.share.zdbjq.cn/Article/details/gmjjoefyc.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://mobile.fehbvm.com/Article/details/gtkzdqaew.sHtML

JS:   const square = x => x * x;
来源：http://blog.hesvh.cn/Article/details/gpiaptebi.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://blog.hesvh.cn/Article/details/gqqopxcml.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://read.share.fehbvm.com/Article/details/gapyulioy.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.share.hesvh.cn/Article/details/grkaxanhp.sHtML

Ruby: square = ->(x) { x * x }
来源：http://m.share.fehbvm.com/Article/details/gpounybbr.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://read.share.zdbjq.cn/Article/details/grztswfse.sHtML

[C07] 把函数作为参数传入
来源：http://www.share.zdbjq.cn/Article/details/gbwrxgqfw.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://mobile.hesvh.cn/Article/details/gvxalarhp.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://blog.hesvh.cn/Article/details/gvkxsysnn.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://baike.hesvh.cn/Article/details/gyrfznobv.sHtML

TS:   arr.map(String)
来源：http://m.share.hesvh.cn/Article/details/guedtfqoc.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.share.hesvh.cn/Article/details/gboorvxvz.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://mobile.zdbjq.cn/Article/details/gvbvyvohq.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.share.hesvh.cn/Article/details/gsxfvklto.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://mobile.zdbjq.cn/Article/details/gvoixxuql.sHtML

[C08] 闭包
来源：http://baike.zdbjq.cn/Article/details/gdfngwwtn.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://wap.fehbvm.com/Article/details/gotunovly.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://blog.fehbvm.com/Article/details/ggkrzajoy.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://baike.hesvh.cn/Article/details/gtgzsvnrm.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://blog.zdbjq.cn/Article/details/gmqmqllfd.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://read.share.zdbjq.cn/Article/details/gkrfquskl.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://3g.fehbvm.com/Article/details/gkiznkhii.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.m.share.hesvh.cn/Article/details/gannvswyh.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.blog.zdbjq.cn/Article/details/gbhyhmdhm.sHtML

[C09] 递归
来源：http://www.share.hesvh.cn/Article/details/gvdtyrcrh.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://mobile.zdbjq.cn/Article/details/gxepxkelf.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://m.share.hesvh.cn/Article/details/gmpqpcxds.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.hesvh.cn/Article/details/gxlulmhjp.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.zdbjq.cn/Article/details/gijvdbzkj.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://blog.hesvh.cn/Article/details/gfxnuvhvd.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://blog.zdbjq.cn/Article/details/gplqbuylo.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://m.share.zdbjq.cn/Article/details/gtazdondc.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.blog.zdbjq.cn/Article/details/gaoltiesk.sHtML

[C10] 变量作用域
来源：http://www.blog.fehbvm.com/Article/details/ghelhvmpo.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://mobile.hesvh.cn/Article/details/gjnoexhkw.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.m.share.fehbvm.com/Article/details/gmxlbscun.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://baike.fehbvm.com/Article/details/gbaypcxjs.sHtML

TS:   同 JS
来源：http://blog.fehbvm.com/Article/details/gdabfkbiy.sHtML

Java: 方法内为块级作用域
来源：http://mobile.zdbjq.cn/Article/details/ghjsfhrkf.sHtML

Go:   花括号块级作用域
来源：http://www.blog.fehbvm.com/Article/details/gcwneeqfe.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://mobile.fehbvm.com/Article/details/gsdnuizse.sHtML

C#:   块级作用域
来源：http://3g.fehbvm.com/Article/details/gqbewuhap.sHtML

[C11] 模块导入与导出
来源：http://mobile.zdbjq.cn/Article/details/geawfaoks.sHtML

Py:   from module import func
来源：http://www.blog.fehbvm.com/Article/details/gzvuicxib.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.share.zdbjq.cn/Article/details/guanwxdjs.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://read.share.zdbjq.cn/Article/details/gcyqajpik.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.share.fehbvm.com/Article/details/gvccnlvjb.sHtML

Java: import java.util.List;
来源：http://m.share.fehbvm.com/Article/details/gykyzegsk.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.m.share.hesvh.cn/Article/details/gzulwjket.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://wap.fehbvm.com/Article/details/gwelbakcz.sHtML

C#:   using System.Text;
来源：http://m.share.fehbvm.com/Article/details/gtmldfkdj.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.blog.hesvh.cn/Article/details/ghcdlgnyo.sHtML

Py:   (lambda: print("run"))()
来源：http://3g.fehbvm.com/Article/details/glxsbcvpa.sHtML

PHP:  (function () { echo "run"; })();
来源：http://mobile.zdbjq.cn/Article/details/gqdcrwflo.sHtML

JS:   (() => { console.log("run"); })();
来源：http://blog.hesvh.cn/Article/details/gytassghv.sHtML

TS:   (() => { console.log("run"); })();
来源：http://mobile.hesvh.cn/Article/details/ghuzyefup.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://read.share.hesvh.cn/Article/details/gvafsodxu.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://mobile.fehbvm.com/Article/details/gbpbbygvj.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.m.share.hesvh.cn/Article/details/gzpnkffer.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://blog.zdbjq.cn/Article/details/gdvuejroz.sHtML

[C13] 类型声明 / 类型注解
来源：http://baike.zdbjq.cn/Article/details/ggqcdaxre.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wap.fehbvm.com/Article/details/glfapssrb.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.zdbjq.cn/Article/details/gnwdnpjir.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://mobile.hesvh.cn/Article/details/gvlnaqvbv.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.fehbvm.com/Article/details/gsgsgapin.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://baike.hesvh.cn/Article/details/gpbxjggxf.sHtML

Go:   func add(a, b int) int
来源：http://3g.hesvh.cn/Article/details/gybdutufh.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://3g.zdbjq.cn/Article/details/gapyxmbve.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://wap.zdbjq.cn/Article/details/gczotjqoa.sHtML

[C14] 泛型函数
来源：http://m.share.hesvh.cn/Article/details/gptvccjsq.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.share.hesvh.cn/Article/details/gfhdkhaar.sHtML

PHP:  // 无泛型
来源：http://www.share.hesvh.cn/Article/details/gleylgxoj.sHtML

JS:   // 无泛型
来源：http://read.share.hesvh.cn/Article/details/grjmjntab.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://baike.zdbjq.cn/Article/details/gxsfoxanc.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.blog.fehbvm.com/Article/details/geewrlbxf.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://m.share.fehbvm.com/Article/details/gqucjglwi.sHtML

Ruby: # 无泛型
来源：http://blog.fehbvm.com/Article/details/gabjonagg.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.share.fehbvm.com/Article/details/gjpqjwtfh.sHtML

[C15] 解构 / 展开参数
来源：http://baike.zdbjq.cn/Article/details/ggkftnlsp.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://3g.fehbvm.com/Article/details/gspqfglzk.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.share.fehbvm.com/Article/details/glvzwxvbt.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://mobile.zdbjq.cn/Article/details/gxbzwemwa.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.share.hesvh.cn/Article/details/gcmwatbsk.sHtML

Java: // 无解构
来源：http://read.share.fehbvm.com/Article/details/gimidhtrh.sHtML

Go:   // 无解构
来源：http://www.share.zdbjq.cn/Article/details/gfrecyrzr.sHtML

Ruby: a, b = pair
来源：http://mobile.zdbjq.cn/Article/details/gxdbfxlny.sHtML

C#:   var (a, b) = pair;
来源：http://m.share.zdbjq.cn/Article/details/gejibiedo.sHtML

[C16] 函数 / 方法重载
来源：http://www.m.share.hesvh.cn/Article/details/gdwsiudjz.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://3g.hesvh.cn/Article/details/gtssfcayl.sHtML

PHP:  // 无重载
来源：http://m.share.fehbvm.com/Article/details/gfwqvrsyi.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.m.share.hesvh.cn/Article/details/gjpsyzpyw.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://baike.fehbvm.com/Article/details/gyohwwemr.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.m.share.fehbvm.com/Article/details/gizgxgbbe.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.blog.fehbvm.com/Article/details/gzbgbvkrv.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.m.share.zdbjq.cn/Article/details/gwclbibwu.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.blog.hesvh.cn/Article/details/gpgbhgbkf.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gyehnaisq.sHtML

D. 数组 / 列表 / 集合
来源：http://read.share.zdbjq.cn/Article/details/glhwilshr.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gapwwdwcc.sHtML

[D01] 创建数组 / 列表
来源：http://wap.zdbjq.cn/Article/details/gotoikdjk.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.blog.hesvh.cn/Article/details/gtqptxhuj.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://3g.zdbjq.cn/Article/details/grdbvpkcs.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.m.share.hesvh.cn/Article/details/gwbuwoqzm.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://3g.hesvh.cn/Article/details/gsdcxvoiv.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://3g.hesvh.cn/Article/details/gaaiczvvj.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.blog.hesvh.cn/Article/details/gjesicpru.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.m.share.fehbvm.com/Article/details/gnrdmhwmv.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://m.share.zdbjq.cn/Article/details/gsavfpvab.sHtML

[D02] 追加元素到末尾
来源：http://www.blog.zdbjq.cn/Article/details/gosokzwij.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.share.fehbvm.com/Article/details/gbxjssgwx.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://3g.hesvh.cn/Article/details/gcrsxeufi.sHtML

JS:   arr.push(4);
来源：http://mobile.zdbjq.cn/Article/details/gqrxbmmqx.sHtML

TS:   arr.push(4);
来源：http://www.share.fehbvm.com/Article/details/gkporjxzz.sHtML

Java: list.add(4);
来源：http://www.share.zdbjq.cn/Article/details/gtqwrrivr.sHtML

Go:   arr = append(arr, 4)
来源：http://read.share.zdbjq.cn/Article/details/ggmtxwkfj.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.share.zdbjq.cn/Article/details/gnmspbyjq.sHtML

C#:   list.Add(4);
来源：http://read.share.hesvh.cn/Article/details/gmxqjdxut.sHtML

[D03] 在指定位置插入元素
来源：http://www.m.share.fehbvm.com/Article/details/gjfozgiae.sHtML

Py:   arr.insert(0, 0)
来源：http://m.share.hesvh.cn/Article/details/gulvulwvb.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://blog.fehbvm.com/Article/details/gazsucbfb.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://baike.fehbvm.com/Article/details/gbfzebgab.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://3g.hesvh.cn/Article/details/gpckaexqd.sHtML

Java: list.add(0, 0);
来源：http://www.share.hesvh.cn/Article/details/gathajxig.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://read.share.zdbjq.cn/Article/details/gpuvdxqdv.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wap.hesvh.cn/Article/details/gezjtolxp.sHtML

C#:   list.Insert(0, 0);
来源：http://blog.zdbjq.cn/Article/details/gnetbbndc.sHtML

[D04] 删除元素
来源：http://3g.zdbjq.cn/Article/details/gcnfhytws.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mobile.hesvh.cn/Article/details/gzfdxhsyj.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.share.fehbvm.com/Article/details/gyjesnaso.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://baike.fehbvm.com/Article/details/glevayjis.sHtML

TS:   arr.splice(0, 1);
来源：http://blog.hesvh.cn/Article/details/gapsjgytt.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://m.share.fehbvm.com/Article/details/gihmzavra.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.share.zdbjq.cn/Article/details/gbocmyxwo.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.blog.hesvh.cn/Article/details/ggzsalydp.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://3g.fehbvm.com/Article/details/ghrzygurm.sHtML

[D05] 访问与修改元素
来源：http://3g.fehbvm.com/Article/details/gnkfctsom.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.fehbvm.com/Article/details/gohplysvq.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.m.share.hesvh.cn/Article/details/ganrepmfy.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://blog.fehbvm.com/Article/details/gpybygfkf.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://read.share.hesvh.cn/Article/details/gtjoffkgv.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://blog.zdbjq.cn/Article/details/gcgctooer.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://read.share.fehbvm.com/Article/details/gyjnusgvs.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.zdbjq.cn/Article/details/girazoitl.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.m.share.fehbvm.com/Article/details/gfoiqxbgi.sHtML

[D06] 数组长度
来源：http://read.share.hesvh.cn/Article/details/gnjpnnqoi.sHtML

Py:   len(arr)
来源：http://blog.fehbvm.com/Article/details/gparbwibq.sHtML

PHP:  count($arr);
来源：http://3g.zdbjq.cn/Article/details/gfhtsobww.sHtML

JS:   arr.length
来源：http://www.share.zdbjq.cn/Article/details/gctiagpyq.sHtML

TS:   arr.length
来源：http://mobile.fehbvm.com/Article/details/gowtyjils.sHtML

Java: list.size();
来源：http://m.share.fehbvm.com/Article/details/gfjbnchgh.sHtML

Go:   len(arr)
来源：http://m.share.fehbvm.com/Article/details/gxxsbihmi.sHtML

Ruby: arr.length; arr.size
来源：http://baike.fehbvm.com/Article/details/gzzxwtrxy.sHtML

C#:   list.Count;
来源：http://www.blog.fehbvm.com/Article/details/gkjhjtqyj.sHtML


<!-- 参考信息 -->