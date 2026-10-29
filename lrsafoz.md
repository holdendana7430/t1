代发 wailian999

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://read.share.hesvh.cn/Article/details/gggdkwgly.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://read.share.fehbvm.com/Article/details/gwtjwhhrk.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://mobile.hesvh.cn/Article/details/grdkozjbq.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.m.share.fehbvm.com/Article/details/gvfoepeqg.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://3g.hesvh.cn/Article/details/gwfelsjxd.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://mobile.hesvh.cn/Article/details/ggdowdtrv.sHtML

[B07] while 循环
来源：http://www.m.share.fehbvm.com/Article/details/gxtnlktxu.sHtML

Py:   while i < 10: i += 1
来源：http://www.share.hesvh.cn/Article/details/goppyjtbn.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://wap.zdbjq.cn/Article/details/gunjpnadu.sHtML

JS:   while (i < 10) { i++; }
来源：http://baike.zdbjq.cn/Article/details/gdnjjexem.sHtML

TS:   while (i < 10) { i++; }
来源：http://read.share.fehbvm.com/Article/details/gfeykszku.sHtML

Java: while (i < 10) { i++; }
来源：http://www.m.share.fehbvm.com/Article/details/gffxawmuv.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.m.share.fehbvm.com/Article/details/gjxuuqmpz.sHtML

Ruby: while i < 10; i += 1; end
来源：http://baike.zdbjq.cn/Article/details/giuehpcmt.sHtML

C#:   while (i < 10) { i++; }
来源：http://blog.hesvh.cn/Article/details/gbjkyqoas.sHtML

[B08] do-while（至少执行一次）
来源：http://mobile.zdbjq.cn/Article/details/gmlzpyump.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://m.share.zdbjq.cn/Article/details/gwwwspqjy.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://baike.hesvh.cn/Article/details/gwjgysloq.sHtML

JS:   do { i++; } while (i < 10);
来源：http://wap.zdbjq.cn/Article/details/gretetgly.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.share.fehbvm.com/Article/details/gxbtdcihv.sHtML

Java: do { i++; } while (i < 10);
来源：http://read.share.zdbjq.cn/Article/details/geqrnhdqm.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://mobile.zdbjq.cn/Article/details/ggzgbkgdr.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.share.fehbvm.com/Article/details/gsssndwzd.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.share.hesvh.cn/Article/details/grmzrercs.sHtML

[B09] break 与 continue
来源：http://m.share.hesvh.cn/Article/details/gxzszjnnt.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://read.share.fehbvm.com/Article/details/gsjiznbpg.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://blog.zdbjq.cn/Article/details/gkfwstnop.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.zdbjq.cn/Article/details/gqpdalzwc.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.hesvh.cn/Article/details/gatwcftme.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.fehbvm.com/Article/details/gvfpefxru.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://m.share.fehbvm.com/Article/details/gxfjcpcwe.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://baike.hesvh.cn/Article/details/gpgdaknwg.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.zdbjq.cn/Article/details/gzhfpvjub.sHtML

[B10] 遍历同时拿索引
来源：http://www.m.share.fehbvm.com/Article/details/gklfuxbxx.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://wap.hesvh.cn/Article/details/gacihzmnn.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://3g.fehbvm.com/Article/details/genvidtfv.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://mobile.zdbjq.cn/Article/details/guycijaua.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://read.share.fehbvm.com/Article/details/gjajswlql.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://baike.fehbvm.com/Article/details/gbjymzlpz.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://read.share.zdbjq.cn/Article/details/gnkhgmwua.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.share.zdbjq.cn/Article/details/gkxtnwtwj.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://m.share.fehbvm.com/Article/details/gpjmerxio.sHtML

[B11] 生成数字序列 / 区间
来源：http://m.share.fehbvm.com/Article/details/gdimuhkgf.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.share.zdbjq.cn/Article/details/gdmgxqffm.sHtML

PHP:  range(0, 10, 2);
来源：http://mobile.hesvh.cn/Article/details/gcutedoae.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mobile.hesvh.cn/Article/details/gryotnwgp.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://3g.zdbjq.cn/Article/details/gztruvufm.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://wap.zdbjq.cn/Article/details/gylunyijt.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://wap.hesvh.cn/Article/details/grcixummt.sHtML

Ruby: (0...10).step(2).to_a
来源：http://m.share.fehbvm.com/Article/details/gwhannotm.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://read.share.zdbjq.cn/Article/details/gukivmldt.sHtML

[B12] 跳出多层循环
来源：http://mobile.hesvh.cn/Article/details/gdzqidope.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://read.share.hesvh.cn/Article/details/gmctilqcd.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://m.share.hesvh.cn/Article/details/gfghiioej.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.fehbvm.com/Article/details/gzgirtcet.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.hesvh.cn/Article/details/gunzdaosw.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://blog.zdbjq.cn/Article/details/gcbxvzrow.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://baike.hesvh.cn/Article/details/gjnnuveko.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://wap.zdbjq.cn/Article/details/gxatwyzym.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.m.share.hesvh.cn/Article/details/gcjburbjo.sHtML

[B13] 判断是否为数字
来源：http://m.share.zdbjq.cn/Article/details/gvrcgoyln.sHtML

Py:   isinstance(x, (int, float))
来源：http://wap.fehbvm.com/Article/details/gprctwxgk.sHtML

PHP:  is_numeric($x)
来源：http://wap.hesvh.cn/Article/details/gluqzwpgs.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.zdbjq.cn/Article/details/ggbnkozvv.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.fehbvm.com/Article/details/gwuunmutv.sHtML

Java: x instanceof Number
来源：http://read.share.hesvh.cn/Article/details/gqjxluncn.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://baike.hesvh.cn/Article/details/gwakijqks.sHtML

Ruby: x.is_a?(Numeric)
来源：http://blog.fehbvm.com/Article/details/gvsnjhqwe.sHtML

C#:   x is int or double or decimal
来源：http://mobile.zdbjq.cn/Article/details/gkkocjnld.sHtML

[B14] 判断值是否在集合内
来源：http://blog.zdbjq.cn/Article/details/gtndabwpv.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.m.share.zdbjq.cn/Article/details/gdknnxpxs.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://read.share.hesvh.cn/Article/details/glwakvkjc.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://mobile.zdbjq.cn/Article/details/gbccvzgfn.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://read.share.hesvh.cn/Article/details/gxacyvoki.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://baike.fehbvm.com/Article/details/gidhfbqqr.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.blog.fehbvm.com/Article/details/gtaqqsfth.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://read.share.zdbjq.cn/Article/details/gegnnfkra.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://3g.zdbjq.cn/Article/details/gmqqtuwdb.sHtML

[B15] 布尔运算与取反
来源：http://wap.zdbjq.cn/Article/details/gvytragxn.sHtML

Py:   a and b or not c
来源：http://www.m.share.zdbjq.cn/Article/details/gdiyyqhjj.sHtML

PHP:  $a && $b || !$c
来源：http://blog.zdbjq.cn/Article/details/gcvzyvifj.sHtML

JS:   a && b || !c
来源：http://blog.hesvh.cn/Article/details/ghhikkzkk.sHtML

TS:   a && b || !c
来源：http://www.share.zdbjq.cn/Article/details/glttxygwz.sHtML

Java: a && b || !c
来源：http://read.share.hesvh.cn/Article/details/gvfjzbzju.sHtML

Go:   a && b || !c
来源：http://baike.zdbjq.cn/Article/details/gpajmkntp.sHtML

Ruby: a && b || !c
来源：http://www.blog.zdbjq.cn/Article/details/gxtmanues.sHtML

C#:   a && b || !c
来源：http://www.blog.zdbjq.cn/Article/details/gdhzevupm.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.blog.fehbvm.com/Article/details/gssqsyynw.sHtML

Py:   if not data: return
来源：http://wap.hesvh.cn/Article/details/gficqyxco.sHtML

PHP:  if (!$data) { return; }
来源：http://blog.hesvh.cn/Article/details/ghyqntxja.sHtML

JS:   if (!data) return;
来源：http://baike.zdbjq.cn/Article/details/gklqzanfd.sHtML

TS:   if (!data) return;
来源：http://www.blog.hesvh.cn/Article/details/gewaxneui.sHtML

Java: if (data == null) return;
来源：http://mobile.hesvh.cn/Article/details/getyyexef.sHtML

Go:   if data == nil { return }
来源：http://www.share.zdbjq.cn/Article/details/ggodnedna.sHtML

Ruby: return if data.nil?
来源：http://baike.hesvh.cn/Article/details/gremlyodx.sHtML

C#:   if (data == null) return;
来源：http://wap.fehbvm.com/Article/details/gvgwbnbcj.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gznnnnlim.sHtML

C. 函数与作用域
来源：http://3g.zdbjq.cn/Article/details/glvmhdewp.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gklsqohns.sHtML

[C01] 定义函数
来源：http://blog.fehbvm.com/Article/details/gqbcfuvqe.sHtML

Py:   def add(a, b): return a + b
来源：http://read.share.hesvh.cn/Article/details/gizjyjlun.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.hesvh.cn/Article/details/ghubzhbwl.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://baike.fehbvm.com/Article/details/gxlocwgvl.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.zdbjq.cn/Article/details/ghruiiskr.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.blog.hesvh.cn/Article/details/ganhhiiyz.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://mobile.zdbjq.cn/Article/details/gkzxhekmv.sHtML

Ruby: def add(a, b); a + b; end
来源：http://wap.hesvh.cn/Article/details/gamrpyjqf.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.blog.fehbvm.com/Article/details/gziphnlvh.sHtML

[C02] 默认参数
来源：http://www.m.share.zdbjq.cn/Article/details/gyilklvzf.sHtML

Py:   def greet(name="World"): return name
来源：http://read.share.zdbjq.cn/Article/details/gzdagvqay.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://m.share.fehbvm.com/Article/details/gaixsljhd.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.m.share.hesvh.cn/Article/details/gctlixfga.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://wap.zdbjq.cn/Article/details/gvmiqdaev.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://3g.zdbjq.cn/Article/details/ggdgtwsba.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.m.share.zdbjq.cn/Article/details/gkxmwopko.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.share.hesvh.cn/Article/details/gtxxxvzwv.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.blog.zdbjq.cn/Article/details/gwxwifvek.sHtML

[C03] 可变参数
来源：http://3g.zdbjq.cn/Article/details/gwqgjinsu.sHtML

Py:   def total(*args): return sum(args)
来源：http://read.share.fehbvm.com/Article/details/gbznyzanx.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://baike.fehbvm.com/Article/details/grwjvkzfh.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.hesvh.cn/Article/details/ggcivpfpw.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.fehbvm.com/Article/details/gpnsfnnzf.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://wap.fehbvm.com/Article/details/gjafclybj.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://baike.fehbvm.com/Article/details/ggvbgsgsc.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://read.share.fehbvm.com/Article/details/groeyjpdo.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://wap.fehbvm.com/Article/details/gpiwktiou.sHtML

[C04] 命名参数 / 关键字参数
来源：http://3g.zdbjq.cn/Article/details/gxdlxlrzv.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://3g.hesvh.cn/Article/details/gsyyxqqba.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.blog.fehbvm.com/Article/details/gllhpwjsn.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.share.hesvh.cn/Article/details/gorsfwusd.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.blog.fehbvm.com/Article/details/geggkmxjs.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.blog.zdbjq.cn/Article/details/gllpuotpe.sHtML

Go:   // 无：用配置结构体参数
来源：http://wap.fehbvm.com/Article/details/gypxpench.sHtML

Ruby: f(a: 1, b: 2)
来源：http://mobile.hesvh.cn/Article/details/glwlluzrc.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.m.share.fehbvm.com/Article/details/gsnhqufqr.sHtML

[C05] 返回多个值
来源：http://m.share.hesvh.cn/Article/details/gcyglxaaj.sHtML

Py:   return a, b
来源：http://www.blog.fehbvm.com/Article/details/gtxfadgrs.sHtML

PHP:  return [$a, $b];
来源：http://www.blog.hesvh.cn/Article/details/guihrfwkz.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://mobile.fehbvm.com/Article/details/gedgncbdf.sHtML

TS:   return { a, b };
来源：http://mobile.hesvh.cn/Article/details/grfhehgfy.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.m.share.hesvh.cn/Article/details/gspghixgv.sHtML

Go:   return a, b
来源：http://www.blog.zdbjq.cn/Article/details/geniufoxs.sHtML

Ruby: return a, b
来源：http://m.share.zdbjq.cn/Article/details/gisuwiufg.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://blog.hesvh.cn/Article/details/gterlbnin.sHtML

[C06] 匿名函数 / lambda
来源：http://3g.zdbjq.cn/Article/details/gfkbwxeqp.sHtML

Py:   square = lambda x: x * x
来源：http://www.blog.zdbjq.cn/Article/details/gkkzxanpv.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://baike.hesvh.cn/Article/details/geoydobyd.sHtML

JS:   const square = x => x * x;
来源：http://wap.hesvh.cn/Article/details/gjjucdhyv.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://mobile.zdbjq.cn/Article/details/gqytttxwm.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://mobile.zdbjq.cn/Article/details/gdjjateem.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://wap.fehbvm.com/Article/details/gjrwwcuhv.sHtML

Ruby: square = ->(x) { x * x }
来源：http://read.share.zdbjq.cn/Article/details/gsnirstfh.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://m.share.hesvh.cn/Article/details/glzjxbfeu.sHtML

[C07] 把函数作为参数传入
来源：http://blog.zdbjq.cn/Article/details/gnohelitx.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://baike.hesvh.cn/Article/details/gadpjsjjm.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://read.share.fehbvm.com/Article/details/gdyghirue.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://3g.fehbvm.com/Article/details/gbkcxjlpm.sHtML

TS:   arr.map(String)
来源：http://m.share.hesvh.cn/Article/details/gsqmjhskv.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://read.share.fehbvm.com/Article/details/gygjnrjxl.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://blog.hesvh.cn/Article/details/gtwnfycou.sHtML

Ruby: arr.map(&:upcase)
来源：http://m.share.zdbjq.cn/Article/details/gdzgbsgos.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://m.share.hesvh.cn/Article/details/gzxgoctkx.sHtML

[C08] 闭包
来源：http://blog.zdbjq.cn/Article/details/gobmzpptz.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://3g.zdbjq.cn/Article/details/gfwxyzfjp.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://mobile.hesvh.cn/Article/details/grtiwdruu.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://3g.fehbvm.com/Article/details/gbfemhmxo.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://m.share.hesvh.cn/Article/details/ggxigussm.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://read.share.zdbjq.cn/Article/details/gdyiufmaa.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://3g.fehbvm.com/Article/details/geffbhnoz.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://3g.zdbjq.cn/Article/details/gyiexzjib.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://blog.zdbjq.cn/Article/details/gwazlswox.sHtML

[C09] 递归
来源：http://blog.fehbvm.com/Article/details/gnfhovvtd.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://baike.fehbvm.com/Article/details/gybtvdbma.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://blog.hesvh.cn/Article/details/gfwelfuyz.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.fehbvm.com/Article/details/gfqkyhnar.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.fehbvm.com/Article/details/gpdzkwnwr.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://3g.zdbjq.cn/Article/details/givzfphjk.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.m.share.zdbjq.cn/Article/details/gwyiycphq.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.share.fehbvm.com/Article/details/gwszbwjrq.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://3g.zdbjq.cn/Article/details/gjzapwtlf.sHtML

[C10] 变量作用域
来源：http://www.share.hesvh.cn/Article/details/gbduwqiqz.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.share.fehbvm.com/Article/details/ghsszbpei.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://baike.fehbvm.com/Article/details/gfacbvnmc.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.blog.hesvh.cn/Article/details/gwnvfmaem.sHtML

TS:   同 JS
来源：http://www.share.zdbjq.cn/Article/details/gsdcwkkvs.sHtML

Java: 方法内为块级作用域
来源：http://www.blog.zdbjq.cn/Article/details/ghlaytcgp.sHtML

Go:   花括号块级作用域
来源：http://mobile.zdbjq.cn/Article/details/gstoxcsto.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://read.share.hesvh.cn/Article/details/gmmiwzbch.sHtML

C#:   块级作用域
来源：http://www.blog.hesvh.cn/Article/details/gwdjnrmqe.sHtML

[C11] 模块导入与导出
来源：http://read.share.zdbjq.cn/Article/details/gebhaodjy.sHtML

Py:   from module import func
来源：http://www.blog.fehbvm.com/Article/details/gogmzczmg.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://mobile.hesvh.cn/Article/details/gkedldtsh.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://m.share.fehbvm.com/Article/details/gplkiegla.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.m.share.hesvh.cn/Article/details/ggeyrsclm.sHtML

Java: import java.util.List;
来源：http://www.share.fehbvm.com/Article/details/gzhatsesq.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://blog.fehbvm.com/Article/details/gkgeoekdf.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.share.zdbjq.cn/Article/details/gstvnsafo.sHtML

C#:   using System.Text;
来源：http://www.m.share.zdbjq.cn/Article/details/ggpfnpgsw.sHtML

[C12] 立即执行函数 IIFE
来源：http://mobile.fehbvm.com/Article/details/gfxbpzvws.sHtML

Py:   (lambda: print("run"))()
来源：http://mobile.zdbjq.cn/Article/details/ggppsntmg.sHtML

PHP:  (function () { echo "run"; })();
来源：http://3g.zdbjq.cn/Article/details/gnzdketud.sHtML

JS:   (() => { console.log("run"); })();
来源：http://mobile.hesvh.cn/Article/details/gwteliczj.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.blog.hesvh.cn/Article/details/gsdumuipg.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wap.zdbjq.cn/Article/details/gldtofeyd.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://read.share.zdbjq.cn/Article/details/gguebkpxo.sHtML

Ruby: -> { puts "run" }.call
来源：http://read.share.fehbvm.com/Article/details/gdpfvaetu.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://blog.hesvh.cn/Article/details/gkgamrdmw.sHtML

[C13] 类型声明 / 类型注解
来源：http://3g.zdbjq.cn/Article/details/gvcumynov.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.blog.fehbvm.com/Article/details/gdmripudb.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.fehbvm.com/Article/details/gdwarwrst.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://blog.hesvh.cn/Article/details/gquehdufi.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.fehbvm.com/Article/details/ghbqiymki.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://3g.hesvh.cn/Article/details/gshtszmqw.sHtML

Go:   func add(a, b int) int
来源：http://m.share.fehbvm.com/Article/details/gfurvvhzv.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://m.share.fehbvm.com/Article/details/gnbmbpxxd.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://blog.hesvh.cn/Article/details/gjwlcnxho.sHtML

[C14] 泛型函数
来源：http://mobile.zdbjq.cn/Article/details/ggdyanjux.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://3g.zdbjq.cn/Article/details/gsecdqlhs.sHtML

PHP:  // 无泛型
来源：http://3g.hesvh.cn/Article/details/glgrynaum.sHtML

JS:   // 无泛型
来源：http://www.m.share.hesvh.cn/Article/details/gazxeoqeg.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://read.share.zdbjq.cn/Article/details/gjsvovvjg.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.m.share.hesvh.cn/Article/details/gxsvzmvfe.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mobile.hesvh.cn/Article/details/ggxyqozrj.sHtML

Ruby: # 无泛型
来源：http://blog.fehbvm.com/Article/details/gljzopfhx.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.blog.fehbvm.com/Article/details/glzlqfvvk.sHtML

[C15] 解构 / 展开参数
来源：http://baike.hesvh.cn/Article/details/gkrifdihn.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://mobile.fehbvm.com/Article/details/gqcskjbki.sHtML

PHP:  [$a, $b] = $pair;
来源：http://baike.hesvh.cn/Article/details/ghepskcem.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.blog.hesvh.cn/Article/details/geyygvbmd.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.m.share.fehbvm.com/Article/details/gshuyxrgo.sHtML

Java: // 无解构
来源：http://wap.fehbvm.com/Article/details/gzhavkwqt.sHtML

Go:   // 无解构
来源：http://www.share.fehbvm.com/Article/details/ggoamfmrk.sHtML

Ruby: a, b = pair
来源：http://wap.zdbjq.cn/Article/details/ganpucftc.sHtML

C#:   var (a, b) = pair;
来源：http://www.share.hesvh.cn/Article/details/gboqftcyp.sHtML

[C16] 函数 / 方法重载
来源：http://blog.hesvh.cn/Article/details/gfgggsktm.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://m.share.fehbvm.com/Article/details/gxvxlfqvy.sHtML

PHP:  // 无重载
来源：http://www.share.fehbvm.com/Article/details/ghftrmmsk.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://m.share.hesvh.cn/Article/details/gludnvfrs.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://blog.hesvh.cn/Article/details/ggayjuhbn.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://3g.hesvh.cn/Article/details/gytxdspyx.sHtML

Go:   // 无重载：用不同函数名
来源：http://wap.zdbjq.cn/Article/details/gsokylteb.sHtML

Ruby: # 无重载：靠动态参数
来源：http://read.share.hesvh.cn/Article/details/gttlgasys.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://wap.zdbjq.cn/Article/details/gflgdjaqq.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/guzzljdxc.sHtML

D. 数组 / 列表 / 集合
来源：http://www.share.zdbjq.cn/Article/details/gwyvczfhg.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gtsgoxktv.sHtML

[D01] 创建数组 / 列表
来源：http://wap.hesvh.cn/Article/details/gjnmeaisd.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://m.share.fehbvm.com/Article/details/goqvnberu.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.blog.zdbjq.cn/Article/details/glhjxnlio.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.m.share.fehbvm.com/Article/details/gfyzokppy.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.m.share.hesvh.cn/Article/details/gbivhsxst.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://read.share.hesvh.cn/Article/details/gxxlrraez.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://blog.zdbjq.cn/Article/details/gtlhbzcvp.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.blog.fehbvm.com/Article/details/guftiitnk.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://wap.fehbvm.com/Article/details/gacdbaifp.sHtML

[D02] 追加元素到末尾
来源：http://www.m.share.hesvh.cn/Article/details/ghsliuwlp.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://blog.fehbvm.com/Article/details/geavnuohe.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://blog.zdbjq.cn/Article/details/gwbednzsj.sHtML

JS:   arr.push(4);
来源：http://3g.fehbvm.com/Article/details/gmfeiotnk.sHtML

TS:   arr.push(4);
来源：http://baike.fehbvm.com/Article/details/gpenjydif.sHtML

Java: list.add(4);
来源：http://baike.zdbjq.cn/Article/details/gqyfjkmpc.sHtML

Go:   arr = append(arr, 4)
来源：http://wap.fehbvm.com/Article/details/gfvaslmuk.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.m.share.fehbvm.com/Article/details/gotecuepf.sHtML

C#:   list.Add(4);
来源：http://wap.hesvh.cn/Article/details/gzcaqdbgm.sHtML

[D03] 在指定位置插入元素
来源：http://baike.zdbjq.cn/Article/details/gvvzmkbrf.sHtML

Py:   arr.insert(0, 0)
来源：http://blog.zdbjq.cn/Article/details/gxvazcglq.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.blog.hesvh.cn/Article/details/gngjlnfye.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://blog.zdbjq.cn/Article/details/gbtmaibgn.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.m.share.zdbjq.cn/Article/details/gibqdzfiz.sHtML

Java: list.add(0, 0);
来源：http://mobile.hesvh.cn/Article/details/gixlhodck.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://blog.zdbjq.cn/Article/details/gydjbcmbu.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://3g.hesvh.cn/Article/details/gwaqibyuq.sHtML

C#:   list.Insert(0, 0);
来源：http://m.share.fehbvm.com/Article/details/gofnplteh.sHtML

[D04] 删除元素
来源：http://www.m.share.hesvh.cn/Article/details/gvypiyxie.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://m.share.zdbjq.cn/Article/details/gmzhlaamx.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://3g.fehbvm.com/Article/details/gtyrbhiua.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wap.hesvh.cn/Article/details/gheikoqwz.sHtML

TS:   arr.splice(0, 1);
来源：http://baike.fehbvm.com/Article/details/gigcpbokl.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.m.share.hesvh.cn/Article/details/gkbzopbnj.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.m.share.zdbjq.cn/Article/details/gvapqlbxt.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://blog.hesvh.cn/Article/details/gynvujojg.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://baike.fehbvm.com/Article/details/ggoimvbqi.sHtML

[D05] 访问与修改元素
来源：http://www.blog.hesvh.cn/Article/details/ghksyquhi.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.fehbvm.com/Article/details/ggkksysne.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://mobile.zdbjq.cn/Article/details/gaqkblghw.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://blog.zdbjq.cn/Article/details/gsremxkws.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://blog.hesvh.cn/Article/details/gljqqakpe.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.m.share.zdbjq.cn/Article/details/gzorlviez.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://baike.hesvh.cn/Article/details/gvvxedubr.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.zdbjq.cn/Article/details/gjjcbgtdn.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wap.hesvh.cn/Article/details/gznhbbptu.sHtML

[D06] 数组长度
来源：http://wap.hesvh.cn/Article/details/gxvuozgzv.sHtML

Py:   len(arr)
来源：http://baike.zdbjq.cn/Article/details/gfwzsdhrg.sHtML

PHP:  count($arr);
来源：http://blog.hesvh.cn/Article/details/gnfqyeeac.sHtML

JS:   arr.length
来源：http://wap.zdbjq.cn/Article/details/gselpcedb.sHtML

TS:   arr.length
来源：http://baike.hesvh.cn/Article/details/gggrkwvpr.sHtML

Java: list.size();
来源：http://wap.fehbvm.com/Article/details/gshkshxyx.sHtML

Go:   len(arr)
来源：http://3g.hesvh.cn/Article/details/gfahbtppj.sHtML

Ruby: arr.length; arr.size
来源：http://blog.zdbjq.cn/Article/details/gtgiyakul.sHtML

C#:   list.Count;
来源：http://read.share.zdbjq.cn/Article/details/gxjrokbph.sHtML


<!-- 参考信息 -->