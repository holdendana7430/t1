代发 wailian999

Py:   # 无 do-while：用 while True + break
来源：http://mobile.fehbvm.com/Article/details/gqxomkrtj.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.share.fehbvm.com/Article/details/giglvyzbz.sHtML

JS:   do { i++; } while (i < 10);
来源：http://mobile.fehbvm.com/Article/details/gcbajtuhf.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.share.hesvh.cn/Article/details/gjvopfvtb.sHtML

Java: do { i++; } while (i < 10);
来源：http://wap.hesvh.cn/Article/details/gayuusozf.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://3g.hesvh.cn/Article/details/gsahaxsci.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.share.zdbjq.cn/Article/details/gljsmghjc.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.share.hesvh.cn/Article/details/ghbuwvnfa.sHtML

[B09] break 与 continue
来源：http://www.blog.fehbvm.com/Article/details/gmeglhmrp.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.m.share.fehbvm.com/Article/details/gjkczqsea.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://baike.fehbvm.com/Article/details/gjxjxqnet.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.zdbjq.cn/Article/details/gumnqpwex.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.hesvh.cn/Article/details/gaatdikxq.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.hesvh.cn/Article/details/gvyxtiekm.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.share.hesvh.cn/Article/details/gnyeubwyr.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.share.zdbjq.cn/Article/details/ggcfeenyl.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.zdbjq.cn/Article/details/glabyjerh.sHtML

[B10] 遍历同时拿索引
来源：http://m.share.fehbvm.com/Article/details/gcipxfxju.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://blog.hesvh.cn/Article/details/goniqwgwj.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gjanudwah.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://blog.fehbvm.com/Article/details/gnmawityz.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://read.share.fehbvm.com/Article/details/glgvhynxx.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://wap.fehbvm.com/Article/details/giafsyngn.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://wap.hesvh.cn/Article/details/gcltwhvwo.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.m.share.fehbvm.com/Article/details/ghcfnlnjm.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://blog.zdbjq.cn/Article/details/gxojjynbv.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.blog.hesvh.cn/Article/details/gicjyrfby.sHtML

Py:   list(range(0, 10, 2))
来源：http://baike.fehbvm.com/Article/details/geccvotvz.sHtML

PHP:  range(0, 10, 2);
来源：http://baike.zdbjq.cn/Article/details/gxyapvvax.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.zdbjq.cn/Article/details/gctyosxwy.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://m.share.hesvh.cn/Article/details/gnrnecjvj.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://wap.fehbvm.com/Article/details/gedyidnlu.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://read.share.zdbjq.cn/Article/details/grmpypmct.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.share.fehbvm.com/Article/details/gleylnewt.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://wap.hesvh.cn/Article/details/gwiosqlng.sHtML

[B12] 跳出多层循环
来源：http://m.share.hesvh.cn/Article/details/ggozkwfcg.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://wap.fehbvm.com/Article/details/girfnxnvr.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.share.fehbvm.com/Article/details/gybzqfzdl.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://read.share.fehbvm.com/Article/details/gspwspzqr.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.zdbjq.cn/Article/details/gxwpockgt.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://read.share.fehbvm.com/Article/details/gjhbtazec.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://blog.hesvh.cn/Article/details/gjaidgwda.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://wap.zdbjq.cn/Article/details/gnactcvdb.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.share.hesvh.cn/Article/details/gpirtvjli.sHtML

[B13] 判断是否为数字
来源：http://baike.hesvh.cn/Article/details/gnbeaiviy.sHtML

Py:   isinstance(x, (int, float))
来源：http://3g.hesvh.cn/Article/details/gfjuunmbo.sHtML

PHP:  is_numeric($x)
来源：http://read.share.fehbvm.com/Article/details/gofhuhpun.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.fehbvm.com/Article/details/gefectrek.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.hesvh.cn/Article/details/gksiynxlt.sHtML

Java: x instanceof Number
来源：http://www.share.fehbvm.com/Article/details/grtegjycu.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://3g.zdbjq.cn/Article/details/gazuwuwwv.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.share.zdbjq.cn/Article/details/gqsvtaute.sHtML

C#:   x is int or double or decimal
来源：http://www.m.share.hesvh.cn/Article/details/gjmxszlzi.sHtML

[B14] 判断值是否在集合内
来源：http://read.share.fehbvm.com/Article/details/gnuhmemfd.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://baike.zdbjq.cn/Article/details/gznqqczxz.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://3g.fehbvm.com/Article/details/gekxnfavt.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://3g.fehbvm.com/Article/details/gikowsrtk.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://read.share.hesvh.cn/Article/details/gzjpyhvck.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://wap.zdbjq.cn/Article/details/grczpmpir.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://read.share.fehbvm.com/Article/details/giqntgxgg.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.m.share.zdbjq.cn/Article/details/glpavlrav.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://blog.zdbjq.cn/Article/details/gzzetrprz.sHtML

[B15] 布尔运算与取反
来源：http://www.m.share.hesvh.cn/Article/details/gfvzowcbc.sHtML

Py:   a and b or not c
来源：http://www.blog.zdbjq.cn/Article/details/goceshliq.sHtML

PHP:  $a && $b || !$c
来源：http://read.share.fehbvm.com/Article/details/grnplgtaj.sHtML

JS:   a && b || !c
来源：http://mobile.hesvh.cn/Article/details/gcfgnyuuu.sHtML

TS:   a && b || !c
来源：http://mobile.fehbvm.com/Article/details/gztmgbcky.sHtML

Java: a && b || !c
来源：http://www.share.fehbvm.com/Article/details/gegmzxokl.sHtML

Go:   a && b || !c
来源：http://read.share.hesvh.cn/Article/details/gyuturhbi.sHtML

Ruby: a && b || !c
来源：http://mobile.hesvh.cn/Article/details/gqgorleom.sHtML

C#:   a && b || !c
来源：http://www.m.share.zdbjq.cn/Article/details/grufdlnec.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://wap.fehbvm.com/Article/details/gvoxlzjcf.sHtML

Py:   if not data: return
来源：http://baike.hesvh.cn/Article/details/gchaidrqv.sHtML

PHP:  if (!$data) { return; }
来源：http://www.m.share.hesvh.cn/Article/details/gkntpczbr.sHtML

JS:   if (!data) return;
来源：http://wap.zdbjq.cn/Article/details/glejxwlzv.sHtML

TS:   if (!data) return;
来源：http://blog.hesvh.cn/Article/details/gyadbhszm.sHtML

Java: if (data == null) return;
来源：http://3g.fehbvm.com/Article/details/gdzehfvjm.sHtML

Go:   if data == nil { return }
来源：http://www.m.share.zdbjq.cn/Article/details/govqetpya.sHtML

Ruby: return if data.nil?
来源：http://wap.fehbvm.com/Article/details/gxvsbjhco.sHtML

C#:   if (data == null) return;
来源：http://3g.fehbvm.com/Article/details/guxymtyjh.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gecvtgzas.sHtML

C. 函数与作用域
来源：http://read.share.zdbjq.cn/Article/details/gnckcrjot.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gyhglshuk.sHtML

[C01] 定义函数
来源：http://www.blog.zdbjq.cn/Article/details/gftorcafw.sHtML

Py:   def add(a, b): return a + b
来源：http://mobile.zdbjq.cn/Article/details/gnnajbuxh.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.zdbjq.cn/Article/details/gvpjhrzwt.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://m.share.hesvh.cn/Article/details/ggagfbgvu.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.fehbvm.com/Article/details/ghjullmhb.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.blog.hesvh.cn/Article/details/gmgkqaejy.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://wap.zdbjq.cn/Article/details/gbtklunzs.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.m.share.fehbvm.com/Article/details/gjmweblyc.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.m.share.hesvh.cn/Article/details/gwmokxceb.sHtML

[C02] 默认参数
来源：http://blog.zdbjq.cn/Article/details/ghmhlogok.sHtML

Py:   def greet(name="World"): return name
来源：http://m.share.fehbvm.com/Article/details/gngivevgn.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://mobile.fehbvm.com/Article/details/gacxgljzx.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.share.fehbvm.com/Article/details/gppwykxtb.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.share.fehbvm.com/Article/details/gzrjysenw.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://baike.hesvh.cn/Article/details/ggtuvelrp.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://read.share.hesvh.cn/Article/details/gqvckunki.sHtML

Ruby: def greet(name = "World") = name
来源：http://read.share.fehbvm.com/Article/details/ggzamqzim.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://read.share.zdbjq.cn/Article/details/gtwcppuno.sHtML

[C03] 可变参数
来源：http://3g.hesvh.cn/Article/details/gumdqvlrt.sHtML

Py:   def total(*args): return sum(args)
来源：http://blog.zdbjq.cn/Article/details/ggpibuysp.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://read.share.zdbjq.cn/Article/details/gwmvoyflk.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.hesvh.cn/Article/details/gufrkgmtn.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.hesvh.cn/Article/details/gtjiuchum.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://baike.hesvh.cn/Article/details/gbyerzrtf.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://wap.fehbvm.com/Article/details/gqfuwjbsy.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://mobile.hesvh.cn/Article/details/gvzzrdgfs.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://read.share.fehbvm.com/Article/details/ghrxqslmi.sHtML

[C04] 命名参数 / 关键字参数
来源：http://3g.zdbjq.cn/Article/details/gesbwpmen.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.share.hesvh.cn/Article/details/gekxywths.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.blog.hesvh.cn/Article/details/gltkegjwh.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://wap.hesvh.cn/Article/details/glpsobsry.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.blog.zdbjq.cn/Article/details/gowavybhb.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.blog.zdbjq.cn/Article/details/gkrsabshj.sHtML

Go:   // 无：用配置结构体参数
来源：http://read.share.hesvh.cn/Article/details/gpxeljvlj.sHtML

Ruby: f(a: 1, b: 2)
来源：http://mobile.hesvh.cn/Article/details/gzjlrcxtg.sHtML

C#:   f(a: 1, b: 2)
来源：http://baike.fehbvm.com/Article/details/giwmzmcqt.sHtML

[C05] 返回多个值
来源：http://www.blog.zdbjq.cn/Article/details/glvkxfrkq.sHtML

Py:   return a, b
来源：http://read.share.hesvh.cn/Article/details/gbjjajegs.sHtML

PHP:  return [$a, $b];
来源：http://mobile.zdbjq.cn/Article/details/gxwzbagry.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://blog.fehbvm.com/Article/details/gmwjboiwk.sHtML

TS:   return { a, b };
来源：http://baike.zdbjq.cn/Article/details/gyrxgpcez.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.m.share.hesvh.cn/Article/details/gumihdyjt.sHtML

Go:   return a, b
来源：http://3g.hesvh.cn/Article/details/gmzqibcbb.sHtML

Ruby: return a, b
来源：http://wap.hesvh.cn/Article/details/gpbyswvtm.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://wap.fehbvm.com/Article/details/gvzksuppl.sHtML

[C06] 匿名函数 / lambda
来源：http://mobile.fehbvm.com/Article/details/gqhzmarxr.sHtML

Py:   square = lambda x: x * x
来源：http://www.blog.zdbjq.cn/Article/details/gjijggfcs.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://baike.hesvh.cn/Article/details/gludbawec.sHtML

JS:   const square = x => x * x;
来源：http://read.share.hesvh.cn/Article/details/gynjmddwb.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://read.share.hesvh.cn/Article/details/gyslcsqwm.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://mobile.hesvh.cn/Article/details/gsbpzqhfn.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.share.fehbvm.com/Article/details/gdkxmmrbl.sHtML

Ruby: square = ->(x) { x * x }
来源：http://m.share.zdbjq.cn/Article/details/goopxbovy.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://mobile.hesvh.cn/Article/details/grcrgqehs.sHtML

[C07] 把函数作为参数传入
来源：http://3g.hesvh.cn/Article/details/gzjsvqqbi.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://blog.hesvh.cn/Article/details/gjdqlbfuj.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gqiiiqqfl.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://baike.hesvh.cn/Article/details/grqoezfhm.sHtML

TS:   arr.map(String)
来源：http://3g.fehbvm.com/Article/details/gzdogewsi.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://m.share.zdbjq.cn/Article/details/gjcpydstg.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://m.share.zdbjq.cn/Article/details/gidmupwxl.sHtML

Ruby: arr.map(&:upcase)
来源：http://3g.fehbvm.com/Article/details/glbkixjgw.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://wap.hesvh.cn/Article/details/gvkxqtzzt.sHtML

[C08] 闭包
来源：http://www.share.fehbvm.com/Article/details/glojocevo.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://read.share.zdbjq.cn/Article/details/gzvmgbhvz.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://mobile.zdbjq.cn/Article/details/gropgqfzs.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://m.share.hesvh.cn/Article/details/gjwvwmtor.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.share.zdbjq.cn/Article/details/gugnohafc.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://3g.hesvh.cn/Article/details/gghaobtxz.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://baike.hesvh.cn/Article/details/gtkjvpqky.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://m.share.fehbvm.com/Article/details/gwczmcszn.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mobile.zdbjq.cn/Article/details/gfwdcygcw.sHtML

[C09] 递归
来源：http://www.m.share.zdbjq.cn/Article/details/gekczzfhh.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.blog.zdbjq.cn/Article/details/gudhlmngp.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://read.share.fehbvm.com/Article/details/gudjhrltq.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.zdbjq.cn/Article/details/gsiewqssw.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.fehbvm.com/Article/details/gpbfzkejb.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.share.hesvh.cn/Article/details/gtkbpvusm.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://3g.hesvh.cn/Article/details/gcqrwqsob.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mobile.hesvh.cn/Article/details/gkhhldpfz.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://baike.zdbjq.cn/Article/details/gzfhxjhzg.sHtML

[C10] 变量作用域
来源：http://3g.hesvh.cn/Article/details/ghdqeeqaq.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://m.share.zdbjq.cn/Article/details/gykbkhgtz.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.blog.zdbjq.cn/Article/details/gfxzjavae.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.share.fehbvm.com/Article/details/guypahzmo.sHtML

TS:   同 JS
来源：http://wap.fehbvm.com/Article/details/gtkrtvnbj.sHtML

Java: 方法内为块级作用域
来源：http://read.share.hesvh.cn/Article/details/ggmakgdml.sHtML

Go:   花括号块级作用域
来源：http://www.blog.zdbjq.cn/Article/details/gqmjrvjcl.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.m.share.zdbjq.cn/Article/details/ggtjagasd.sHtML

C#:   块级作用域
来源：http://www.m.share.zdbjq.cn/Article/details/gwcnjrtms.sHtML

[C11] 模块导入与导出
来源：http://www.share.zdbjq.cn/Article/details/gshuphtjs.sHtML

Py:   from module import func
来源：http://3g.zdbjq.cn/Article/details/geajzcsij.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://wap.zdbjq.cn/Article/details/gzhdhhlqe.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://read.share.hesvh.cn/Article/details/gjregwkpf.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://mobile.hesvh.cn/Article/details/gmryrzbhg.sHtML

Java: import java.util.List;
来源：http://www.blog.fehbvm.com/Article/details/gefofrvbq.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://m.share.fehbvm.com/Article/details/gdzdkndck.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://3g.fehbvm.com/Article/details/gqeauyxag.sHtML

C#:   using System.Text;
来源：http://baike.fehbvm.com/Article/details/gvbvdqwel.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.m.share.hesvh.cn/Article/details/gqduqpktl.sHtML

Py:   (lambda: print("run"))()
来源：http://www.blog.hesvh.cn/Article/details/gwuozdxfh.sHtML

PHP:  (function () { echo "run"; })();
来源：http://baike.hesvh.cn/Article/details/glywmmeoq.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.m.share.fehbvm.com/Article/details/gotixjshf.sHtML

TS:   (() => { console.log("run"); })();
来源：http://3g.zdbjq.cn/Article/details/gnstvycsj.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wap.hesvh.cn/Article/details/gjrjtcoun.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://baike.fehbvm.com/Article/details/gsbzzhpux.sHtML

Ruby: -> { puts "run" }.call
来源：http://wap.fehbvm.com/Article/details/grtrlpmok.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://wap.zdbjq.cn/Article/details/gsvmyhbwb.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.blog.hesvh.cn/Article/details/gtfdhdkvw.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://blog.zdbjq.cn/Article/details/gptegqfim.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.fehbvm.com/Article/details/gdfpnelcu.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://read.share.fehbvm.com/Article/details/glwwtlrvd.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.fehbvm.com/Article/details/gyiytwjkp.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://read.share.zdbjq.cn/Article/details/gjzqrvvak.sHtML

Go:   func add(a, b int) int
来源：http://www.m.share.zdbjq.cn/Article/details/gtsczdfgu.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.m.share.hesvh.cn/Article/details/gdqtqvmtg.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://3g.hesvh.cn/Article/details/gxepgmmra.sHtML

[C14] 泛型函数
来源：http://baike.zdbjq.cn/Article/details/gsdxdcygf.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.blog.fehbvm.com/Article/details/gtdluduwe.sHtML

PHP:  // 无泛型
来源：http://m.share.fehbvm.com/Article/details/gihlwugpp.sHtML

JS:   // 无泛型
来源：http://3g.fehbvm.com/Article/details/gvimfrwnw.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://mobile.zdbjq.cn/Article/details/glcghxcrh.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wap.zdbjq.cn/Article/details/gjrlocjdx.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://blog.zdbjq.cn/Article/details/gjyubcsju.sHtML

Ruby: # 无泛型
来源：http://read.share.fehbvm.com/Article/details/guticqwiu.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://3g.fehbvm.com/Article/details/gzzofmdeq.sHtML

[C15] 解构 / 展开参数
来源：http://blog.zdbjq.cn/Article/details/glfpwsnrf.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.m.share.zdbjq.cn/Article/details/gijyxxptr.sHtML

PHP:  [$a, $b] = $pair;
来源：http://blog.fehbvm.com/Article/details/gqtrdzeyv.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://3g.zdbjq.cn/Article/details/gbllknzcj.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.m.share.fehbvm.com/Article/details/gdhcyslgx.sHtML

Java: // 无解构
来源：http://read.share.hesvh.cn/Article/details/gcttcplqp.sHtML

Go:   // 无解构
来源：http://read.share.hesvh.cn/Article/details/gvxwtziha.sHtML

Ruby: a, b = pair
来源：http://www.share.hesvh.cn/Article/details/gqjpyydaw.sHtML

C#:   var (a, b) = pair;
来源：http://www.blog.hesvh.cn/Article/details/gthidzxcc.sHtML

[C16] 函数 / 方法重载
来源：http://www.m.share.fehbvm.com/Article/details/grxxekeug.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://mobile.zdbjq.cn/Article/details/gyilllmxo.sHtML

PHP:  // 无重载
来源：http://www.share.fehbvm.com/Article/details/gjzlvkjau.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://m.share.fehbvm.com/Article/details/ggyduiype.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://read.share.zdbjq.cn/Article/details/gpxsbnbfn.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://3g.hesvh.cn/Article/details/gvdaofamf.sHtML

Go:   // 无重载：用不同函数名
来源：http://m.share.fehbvm.com/Article/details/graparzue.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.share.hesvh.cn/Article/details/goqoosifw.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://read.share.hesvh.cn/Article/details/gjqzacnaq.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gpyumyxfq.sHtML

D. 数组 / 列表 / 集合
来源：http://mobile.fehbvm.com/Article/details/gmiqxahwl.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gwgdbygbi.sHtML

[D01] 创建数组 / 列表
来源：http://read.share.zdbjq.cn/Article/details/gerrnmmnr.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://wap.hesvh.cn/Article/details/gpnzivwqp.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.share.hesvh.cn/Article/details/gtomrxfpa.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wap.zdbjq.cn/Article/details/giqjeggxm.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://mobile.zdbjq.cn/Article/details/gwfygldzc.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://blog.zdbjq.cn/Article/details/guysurfpt.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://m.share.zdbjq.cn/Article/details/gjqycspbe.sHtML

Ruby: arr = [1, 2, 3]
来源：http://baike.fehbvm.com/Article/details/grzgxdqxh.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://baike.zdbjq.cn/Article/details/gdkhcabap.sHtML

[D02] 追加元素到末尾
来源：http://wap.hesvh.cn/Article/details/gxrotqxwp.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://blog.zdbjq.cn/Article/details/gsygvjwfr.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://m.share.hesvh.cn/Article/details/givznnlws.sHtML

JS:   arr.push(4);
来源：http://www.m.share.hesvh.cn/Article/details/giejrsxfk.sHtML

TS:   arr.push(4);
来源：http://wap.fehbvm.com/Article/details/gcceqbidu.sHtML

Java: list.add(4);
来源：http://www.m.share.zdbjq.cn/Article/details/gkibqfsrs.sHtML

Go:   arr = append(arr, 4)
来源：http://www.m.share.zdbjq.cn/Article/details/gcrodurmx.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://m.share.hesvh.cn/Article/details/gwplmicln.sHtML

C#:   list.Add(4);
来源：http://wap.zdbjq.cn/Article/details/gvsxknulu.sHtML

[D03] 在指定位置插入元素
来源：http://mobile.zdbjq.cn/Article/details/gdegaoirg.sHtML

Py:   arr.insert(0, 0)
来源：http://m.share.fehbvm.com/Article/details/galuzbwje.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://m.share.hesvh.cn/Article/details/gposfmrij.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://baike.hesvh.cn/Article/details/gyzhzpapg.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.m.share.zdbjq.cn/Article/details/gvvkniufp.sHtML

Java: list.add(0, 0);
来源：http://m.share.hesvh.cn/Article/details/gxfrxttpj.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.share.zdbjq.cn/Article/details/gjadfkzml.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://baike.fehbvm.com/Article/details/gjsnokotw.sHtML

C#:   list.Insert(0, 0);
来源：http://www.m.share.fehbvm.com/Article/details/gkpuktrsg.sHtML

[D04] 删除元素
来源：http://3g.hesvh.cn/Article/details/gnuaiyddn.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mobile.zdbjq.cn/Article/details/goquszblc.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://read.share.zdbjq.cn/Article/details/gvseqranj.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.blog.zdbjq.cn/Article/details/gsvioizxd.sHtML

TS:   arr.splice(0, 1);
来源：http://www.blog.zdbjq.cn/Article/details/gnzuflgxf.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mobile.fehbvm.com/Article/details/gcuyxelov.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.blog.hesvh.cn/Article/details/guxqfkceq.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.m.share.fehbvm.com/Article/details/grzgbmohm.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://m.share.zdbjq.cn/Article/details/gggfgswac.sHtML

[D05] 访问与修改元素
来源：http://baike.fehbvm.com/Article/details/gsizutltg.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.zdbjq.cn/Article/details/gpjcznfkd.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.share.fehbvm.com/Article/details/giqfcdszq.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://blog.hesvh.cn/Article/details/gsjrolyxt.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://m.share.zdbjq.cn/Article/details/gttvtezdp.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.share.fehbvm.com/Article/details/gjqtkpuyx.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://wap.fehbvm.com/Article/details/gtwdlphdh.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.hesvh.cn/Article/details/gkphpljsh.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.m.share.zdbjq.cn/Article/details/gisxotmfp.sHtML

[D06] 数组长度
来源：http://wap.zdbjq.cn/Article/details/gkjwwxadf.sHtML

Py:   len(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gsqwwpgrc.sHtML

PHP:  count($arr);
来源：http://blog.hesvh.cn/Article/details/gqfqgbtzz.sHtML

JS:   arr.length
来源：http://read.share.zdbjq.cn/Article/details/golssrhrk.sHtML

TS:   arr.length
来源：http://www.blog.fehbvm.com/Article/details/gofgiabun.sHtML

Java: list.size();
来源：http://3g.hesvh.cn/Article/details/gpxkrygyx.sHtML

Go:   len(arr)
来源：http://m.share.zdbjq.cn/Article/details/grfmsodtu.sHtML

Ruby: arr.length; arr.size
来源：http://mobile.fehbvm.com/Article/details/gfsykpwzs.sHtML

C#:   list.Count;
来源：http://3g.hesvh.cn/Article/details/gvvjyddgh.sHtML

[D07] 切片 / 取子数组
来源：http://3g.fehbvm.com/Article/details/gsxjqowdp.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://3g.hesvh.cn/Article/details/gjhqzjvyp.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://blog.hesvh.cn/Article/details/gkkuwundy.sHtML

JS:   arr.slice(1, 4);
来源：http://3g.fehbvm.com/Article/details/gahujsdmw.sHtML

TS:   arr.slice(1, 4);
来源：http://3g.zdbjq.cn/Article/details/gmnatyqlc.sHtML

Java: list.subList(1, 4);
来源：http://www.m.share.hesvh.cn/Article/details/gzvtzfzlo.sHtML

Go:   arr[1:4]
来源：http://m.share.fehbvm.com/Article/details/gixfxwslv.sHtML

Ruby: arr[1, 3]
来源：http://www.share.fehbvm.com/Article/details/gnqcxwgze.sHtML

C#:   list.GetRange(1, 3);
来源：http://blog.zdbjq.cn/Article/details/gmgtwmnco.sHtML

[D08] 合并两个数组
来源：http://read.share.fehbvm.com/Article/details/gejpxbttk.sHtML

Py:   a + b;  a.extend(b)
来源：http://baike.hesvh.cn/Article/details/gjodvvlbv.sHtML

PHP:  array_merge($a, $b);
来源：http://www.m.share.fehbvm.com/Article/details/gyueqeqya.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.share.zdbjq.cn/Article/details/grucszkbb.sHtML

TS:   [...a, ...b];
来源：http://www.blog.zdbjq.cn/Article/details/gyqbrmygv.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://m.share.hesvh.cn/Article/details/gnrjsuxpc.sHtML

Go:   append(a, b...)
来源：http://blog.fehbvm.com/Article/details/gioctxmsz.sHtML


<!-- 参考信息 -->