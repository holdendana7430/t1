代发 wailian999

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.blog.zdbjq.cn/Article/details/gxuwpxsqn.sHtML

[B06] 遍历字典 / 对象
来源：http://www.m.share.hesvh.cn/Article/details/gphpwtqur.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://m.share.fehbvm.com/Article/details/gzxnmqmyu.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://3g.fehbvm.com/Article/details/glfismztb.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://m.share.zdbjq.cn/Article/details/gfgjrgjzk.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://baike.fehbvm.com/Article/details/gefaikxxt.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.blog.hesvh.cn/Article/details/geqtsgije.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://wap.hesvh.cn/Article/details/gqektzune.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://read.share.zdbjq.cn/Article/details/gzifpgwwv.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://wap.fehbvm.com/Article/details/gofoqtiqc.sHtML

[B07] while 循环
来源：http://read.share.fehbvm.com/Article/details/ghbuivbdb.sHtML

Py:   while i < 10: i += 1
来源：http://www.share.zdbjq.cn/Article/details/gdrdovubt.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.m.share.zdbjq.cn/Article/details/gdnqprgxb.sHtML

JS:   while (i < 10) { i++; }
来源：http://mobile.hesvh.cn/Article/details/gdsddqhxw.sHtML

TS:   while (i < 10) { i++; }
来源：http://m.share.fehbvm.com/Article/details/gadxjhevn.sHtML

Java: while (i < 10) { i++; }
来源：http://m.share.fehbvm.com/Article/details/gfiidixfk.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://blog.zdbjq.cn/Article/details/gedlqtktu.sHtML

Ruby: while i < 10; i += 1; end
来源：http://m.share.hesvh.cn/Article/details/glwqfnoyf.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.share.fehbvm.com/Article/details/ghcfypfbj.sHtML

[B08] do-while（至少执行一次）
来源：http://mobile.hesvh.cn/Article/details/gbnrkwkux.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://3g.hesvh.cn/Article/details/gtipjdgfm.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://mobile.fehbvm.com/Article/details/gxpajzgjg.sHtML

JS:   do { i++; } while (i < 10);
来源：http://m.share.fehbvm.com/Article/details/gjhzfkdsw.sHtML

TS:   do { i++; } while (i < 10);
来源：http://mobile.hesvh.cn/Article/details/gxoacsvyo.sHtML

Java: do { i++; } while (i < 10);
来源：http://3g.zdbjq.cn/Article/details/geluxgnbg.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://baike.zdbjq.cn/Article/details/gztsxvtuo.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://3g.zdbjq.cn/Article/details/gitfjgsez.sHtML

C#:   do { i++; } while (i < 10);
来源：http://mobile.fehbvm.com/Article/details/gkfuhijxq.sHtML

[B09] break 与 continue
来源：http://read.share.fehbvm.com/Article/details/glackxxws.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.m.share.fehbvm.com/Article/details/gjwsmkoku.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.m.share.zdbjq.cn/Article/details/gkhzlpfus.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.hesvh.cn/Article/details/getmyrbei.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.fehbvm.com/Article/details/gamtupabd.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.hesvh.cn/Article/details/gnmlwqxdd.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.m.share.fehbvm.com/Article/details/gvzzxbvdi.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://m.share.hesvh.cn/Article/details/gvysqqlof.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.fehbvm.com/Article/details/gaslzzcne.sHtML

[B10] 遍历同时拿索引
来源：http://www.m.share.hesvh.cn/Article/details/gekzxtpzz.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://mobile.zdbjq.cn/Article/details/gzwrtqhxy.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://3g.hesvh.cn/Article/details/gyjaametz.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://wap.zdbjq.cn/Article/details/gqzvzjvwr.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://baike.hesvh.cn/Article/details/gvmtvigve.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://read.share.hesvh.cn/Article/details/grcqbfksx.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.share.zdbjq.cn/Article/details/gkreaemdt.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://m.share.hesvh.cn/Article/details/goqqvpsxn.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://mobile.fehbvm.com/Article/details/grpgengcy.sHtML

[B11] 生成数字序列 / 区间
来源：http://baike.fehbvm.com/Article/details/gtucywyqa.sHtML

Py:   list(range(0, 10, 2))
来源：http://read.share.fehbvm.com/Article/details/gtqhefsnr.sHtML

PHP:  range(0, 10, 2);
来源：http://wap.fehbvm.com/Article/details/gmgwumpjj.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.zdbjq.cn/Article/details/gjicltvoy.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://m.share.hesvh.cn/Article/details/gzawrpibt.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://baike.zdbjq.cn/Article/details/gxknldrsn.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.blog.fehbvm.com/Article/details/gsuhgujql.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.m.share.fehbvm.com/Article/details/gtrocotkx.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://m.share.hesvh.cn/Article/details/gzjudgpol.sHtML

[B12] 跳出多层循环
来源：http://read.share.zdbjq.cn/Article/details/guinrimlz.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://3g.fehbvm.com/Article/details/gaunummre.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://m.share.zdbjq.cn/Article/details/gpwsfctdn.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.fehbvm.com/Article/details/gqykorqsr.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://read.share.hesvh.cn/Article/details/grasjvtae.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.zdbjq.cn/Article/details/ginklotky.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.blog.hesvh.cn/Article/details/gqicfxhsy.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.share.fehbvm.com/Article/details/gyukybrmq.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.m.share.hesvh.cn/Article/details/gazjrxirr.sHtML

[B13] 判断是否为数字
来源：http://www.share.hesvh.cn/Article/details/guvqgxyqx.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.m.share.zdbjq.cn/Article/details/grslnwbkb.sHtML

PHP:  is_numeric($x)
来源：http://www.blog.zdbjq.cn/Article/details/gckjcetcj.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.fehbvm.com/Article/details/gcouifeml.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://blog.hesvh.cn/Article/details/gbispkddg.sHtML

Java: x instanceof Number
来源：http://m.share.zdbjq.cn/Article/details/gfilcfzpi.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://3g.hesvh.cn/Article/details/gvlhhvldv.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.blog.fehbvm.com/Article/details/gijlocigb.sHtML

C#:   x is int or double or decimal
来源：http://3g.zdbjq.cn/Article/details/gnscqsdvc.sHtML

[B14] 判断值是否在集合内
来源：http://mobile.hesvh.cn/Article/details/gnbfgvmvn.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.share.zdbjq.cn/Article/details/gkmwysysd.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.blog.fehbvm.com/Article/details/gejqarvvv.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://read.share.hesvh.cn/Article/details/gdnimpgnu.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.share.zdbjq.cn/Article/details/gqoozatac.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.m.share.fehbvm.com/Article/details/gkvxjtema.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://baike.zdbjq.cn/Article/details/gjiusmonp.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.blog.hesvh.cn/Article/details/ghmgotipt.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://mobile.fehbvm.com/Article/details/glbqaiktr.sHtML

[B15] 布尔运算与取反
来源：http://3g.hesvh.cn/Article/details/gmeoecvdx.sHtML

Py:   a and b or not c
来源：http://m.share.fehbvm.com/Article/details/gdtaohhcg.sHtML

PHP:  $a && $b || !$c
来源：http://3g.hesvh.cn/Article/details/ghipwvfzl.sHtML

JS:   a && b || !c
来源：http://www.m.share.fehbvm.com/Article/details/gskwflmeh.sHtML

TS:   a && b || !c
来源：http://blog.zdbjq.cn/Article/details/gtxrmiotf.sHtML

Java: a && b || !c
来源：http://read.share.hesvh.cn/Article/details/gmtucpjnu.sHtML

Go:   a && b || !c
来源：http://www.share.hesvh.cn/Article/details/glexqamvy.sHtML

Ruby: a && b || !c
来源：http://wap.fehbvm.com/Article/details/gvirbicfz.sHtML

C#:   a && b || !c
来源：http://mobile.fehbvm.com/Article/details/gcpabhhmh.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://blog.fehbvm.com/Article/details/guypgfabi.sHtML

Py:   if not data: return
来源：http://wap.fehbvm.com/Article/details/gdzbncubt.sHtML

PHP:  if (!$data) { return; }
来源：http://blog.zdbjq.cn/Article/details/gbiknowma.sHtML

JS:   if (!data) return;
来源：http://read.share.zdbjq.cn/Article/details/glklqcvkk.sHtML

TS:   if (!data) return;
来源：http://mobile.zdbjq.cn/Article/details/gatkswdkw.sHtML

Java: if (data == null) return;
来源：http://read.share.zdbjq.cn/Article/details/gdglrziir.sHtML

Go:   if data == nil { return }
来源：http://blog.hesvh.cn/Article/details/gtrxresdj.sHtML

Ruby: return if data.nil?
来源：http://www.share.hesvh.cn/Article/details/gepmmkpaa.sHtML

C#:   if (data == null) return;
来源：http://read.share.zdbjq.cn/Article/details/gqzfcbzim.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/goxtrfcoh.sHtML

C. 函数与作用域
来源：http://blog.zdbjq.cn/Article/details/ggjxekkvp.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gerawovmp.sHtML

[C01] 定义函数
来源：http://read.share.hesvh.cn/Article/details/grgjcajyk.sHtML

Py:   def add(a, b): return a + b
来源：http://www.share.fehbvm.com/Article/details/gjesozhyn.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.zdbjq.cn/Article/details/geavxwprq.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://wap.hesvh.cn/Article/details/gyqkmgxnv.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.fehbvm.com/Article/details/glxchnvys.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://mobile.zdbjq.cn/Article/details/gjlujxwss.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.m.share.zdbjq.cn/Article/details/ggrvzndfw.sHtML

Ruby: def add(a, b); a + b; end
来源：http://3g.zdbjq.cn/Article/details/ggdqbqcwm.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://wap.zdbjq.cn/Article/details/gqqvumhte.sHtML

[C02] 默认参数
来源：http://3g.fehbvm.com/Article/details/gwpwqscdx.sHtML

Py:   def greet(name="World"): return name
来源：http://m.share.hesvh.cn/Article/details/gttmegkhd.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://m.share.zdbjq.cn/Article/details/ggztfugds.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://mobile.fehbvm.com/Article/details/gfeorgrgh.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://blog.zdbjq.cn/Article/details/gogtovlrw.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.m.share.zdbjq.cn/Article/details/gsjhtsqse.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://mobile.zdbjq.cn/Article/details/glqcxihlh.sHtML

Ruby: def greet(name = "World") = name
来源：http://read.share.fehbvm.com/Article/details/gdngryagm.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.m.share.hesvh.cn/Article/details/gsieiinsp.sHtML

[C03] 可变参数
来源：http://3g.hesvh.cn/Article/details/gruvijndx.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.m.share.hesvh.cn/Article/details/gxfunotal.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.blog.hesvh.cn/Article/details/ghznhorsu.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.hesvh.cn/Article/details/gejxadubs.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.zdbjq.cn/Article/details/gahyilukk.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://wap.zdbjq.cn/Article/details/gdoeyfpfo.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.m.share.fehbvm.com/Article/details/gmilfyqwk.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://baike.zdbjq.cn/Article/details/gqdqsbjsl.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.m.share.zdbjq.cn/Article/details/gqaxvuwii.sHtML

[C04] 命名参数 / 关键字参数
来源：http://3g.zdbjq.cn/Article/details/gooyueocr.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://baike.hesvh.cn/Article/details/gtbgrddyz.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://wap.hesvh.cn/Article/details/gqwyictjt.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://m.share.zdbjq.cn/Article/details/ggjpwaush.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://m.share.zdbjq.cn/Article/details/gwvnfaarq.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://baike.hesvh.cn/Article/details/gaskghlec.sHtML

Go:   // 无：用配置结构体参数
来源：http://read.share.zdbjq.cn/Article/details/glbtoqdgd.sHtML

Ruby: f(a: 1, b: 2)
来源：http://wap.zdbjq.cn/Article/details/gocjkoovq.sHtML

C#:   f(a: 1, b: 2)
来源：http://baike.fehbvm.com/Article/details/guxkkhsvo.sHtML

[C05] 返回多个值
来源：http://read.share.hesvh.cn/Article/details/gqmlqmqlg.sHtML

Py:   return a, b
来源：http://blog.fehbvm.com/Article/details/gfdatuurd.sHtML

PHP:  return [$a, $b];
来源：http://www.share.zdbjq.cn/Article/details/gngppubps.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://3g.hesvh.cn/Article/details/gtenjhlvk.sHtML

TS:   return { a, b };
来源：http://3g.zdbjq.cn/Article/details/ghmvvzyjm.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.blog.fehbvm.com/Article/details/guuqysaal.sHtML

Go:   return a, b
来源：http://3g.hesvh.cn/Article/details/gbmfgpznf.sHtML

Ruby: return a, b
来源：http://www.blog.zdbjq.cn/Article/details/giymxcoqg.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://wap.zdbjq.cn/Article/details/gksgnpylc.sHtML

[C06] 匿名函数 / lambda
来源：http://www.blog.hesvh.cn/Article/details/glzbberwd.sHtML

Py:   square = lambda x: x * x
来源：http://www.m.share.fehbvm.com/Article/details/gjgyykepu.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.share.fehbvm.com/Article/details/gzlfmkzoa.sHtML

JS:   const square = x => x * x;
来源：http://3g.hesvh.cn/Article/details/gkazcbcwc.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.m.share.zdbjq.cn/Article/details/ggrzdkjsu.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://blog.zdbjq.cn/Article/details/gypbnwzsa.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.m.share.fehbvm.com/Article/details/gnkgfdudm.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.m.share.fehbvm.com/Article/details/grnmdeynb.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.m.share.hesvh.cn/Article/details/gxcqyywek.sHtML

[C07] 把函数作为参数传入
来源：http://www.blog.zdbjq.cn/Article/details/geukybgph.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://wap.fehbvm.com/Article/details/gbsdjdtha.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.share.fehbvm.com/Article/details/gwgutujba.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.blog.fehbvm.com/Article/details/gsfilmzes.sHtML

TS:   arr.map(String)
来源：http://wap.hesvh.cn/Article/details/gjazqepdr.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://wap.hesvh.cn/Article/details/gpftaddrs.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://wap.fehbvm.com/Article/details/gecvpkdty.sHtML

Ruby: arr.map(&:upcase)
来源：http://m.share.hesvh.cn/Article/details/gieuidhdp.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://wap.zdbjq.cn/Article/details/gcmleghbm.sHtML

[C08] 闭包
来源：http://3g.hesvh.cn/Article/details/gdhuoqdrb.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.m.share.hesvh.cn/Article/details/gndqkodoa.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://3g.hesvh.cn/Article/details/gkodlnxuz.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.blog.hesvh.cn/Article/details/gokrhusew.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://wap.fehbvm.com/Article/details/geaawzupt.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://wap.fehbvm.com/Article/details/ggkcavkhl.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://3g.zdbjq.cn/Article/details/gsvbitfqz.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://read.share.fehbvm.com/Article/details/gkoqgktuz.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.m.share.fehbvm.com/Article/details/gpcgictij.sHtML

[C09] 递归
来源：http://www.m.share.zdbjq.cn/Article/details/gmssybtjw.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://baike.fehbvm.com/Article/details/gljqlilkt.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://m.share.hesvh.cn/Article/details/gxlppyolo.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.zdbjq.cn/Article/details/gzpiistrq.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.fehbvm.com/Article/details/gfavjaxgn.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.m.share.hesvh.cn/Article/details/gpgjeckuq.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://m.share.fehbvm.com/Article/details/gylmshlhl.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://m.share.fehbvm.com/Article/details/gtrenkrcy.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://wap.hesvh.cn/Article/details/gaqrulznm.sHtML

[C10] 变量作用域
来源：http://mobile.zdbjq.cn/Article/details/gvzrksicl.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wap.zdbjq.cn/Article/details/gvwerudad.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.m.share.zdbjq.cn/Article/details/grbmyonwi.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.m.share.hesvh.cn/Article/details/gjojlpzqo.sHtML

TS:   同 JS
来源：http://blog.fehbvm.com/Article/details/grcyxvlxy.sHtML

Java: 方法内为块级作用域
来源：http://3g.fehbvm.com/Article/details/gugsjhwpg.sHtML

Go:   花括号块级作用域
来源：http://3g.zdbjq.cn/Article/details/gkqcfznvr.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://mobile.fehbvm.com/Article/details/gvaguhrqz.sHtML

C#:   块级作用域
来源：http://blog.zdbjq.cn/Article/details/gdippenyc.sHtML

[C11] 模块导入与导出
来源：http://read.share.hesvh.cn/Article/details/gqhdtgyra.sHtML

Py:   from module import func
来源：http://mobile.zdbjq.cn/Article/details/gyrwsmfsc.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://mobile.hesvh.cn/Article/details/guczmjnhi.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://mobile.hesvh.cn/Article/details/gllgfsxwd.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wap.fehbvm.com/Article/details/giigtyvtb.sHtML

Java: import java.util.List;
来源：http://blog.fehbvm.com/Article/details/grtfeorze.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://blog.hesvh.cn/Article/details/gibxwjzoy.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://3g.hesvh.cn/Article/details/gljhtfrjf.sHtML

C#:   using System.Text;
来源：http://www.m.share.fehbvm.com/Article/details/gsjmdvlnl.sHtML

[C12] 立即执行函数 IIFE
来源：http://mobile.fehbvm.com/Article/details/gdgbbildn.sHtML

Py:   (lambda: print("run"))()
来源：http://www.blog.zdbjq.cn/Article/details/gfdyqjamn.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.blog.zdbjq.cn/Article/details/gihkgdqid.sHtML

JS:   (() => { console.log("run"); })();
来源：http://mobile.hesvh.cn/Article/details/gqzbkdxib.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.m.share.zdbjq.cn/Article/details/guefqvyvj.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wap.hesvh.cn/Article/details/gnumnclol.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.blog.hesvh.cn/Article/details/geqvehjpl.sHtML

Ruby: -> { puts "run" }.call
来源：http://wap.fehbvm.com/Article/details/ghbmxeqnd.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://blog.hesvh.cn/Article/details/gvuyfmeqz.sHtML

[C13] 类型声明 / 类型注解
来源：http://mobile.hesvh.cn/Article/details/gsvxznfki.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://blog.fehbvm.com/Article/details/gjohktmhh.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.zdbjq.cn/Article/details/gkpocyrke.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://wap.zdbjq.cn/Article/details/gmlbuekoo.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.hesvh.cn/Article/details/grwrwqowi.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.m.share.hesvh.cn/Article/details/glgtjuffd.sHtML

Go:   func add(a, b int) int
来源：http://mobile.hesvh.cn/Article/details/gtjcxymem.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.blog.hesvh.cn/Article/details/gkwostcex.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.share.zdbjq.cn/Article/details/gtnzzztpp.sHtML

[C14] 泛型函数
来源：http://read.share.hesvh.cn/Article/details/grmyeyzft.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.m.share.fehbvm.com/Article/details/gvkwgisyo.sHtML

PHP:  // 无泛型
来源：http://www.m.share.zdbjq.cn/Article/details/gzfdummno.sHtML

JS:   // 无泛型
来源：http://www.blog.hesvh.cn/Article/details/grxbmdtbp.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://blog.hesvh.cn/Article/details/gxcrmymui.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://baike.fehbvm.com/Article/details/gfhzwwaca.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://3g.fehbvm.com/Article/details/gzmyfblsm.sHtML

Ruby: # 无泛型
来源：http://www.m.share.fehbvm.com/Article/details/ggmuefdtv.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mobile.zdbjq.cn/Article/details/gtlognpxm.sHtML

[C15] 解构 / 展开参数
来源：http://www.blog.zdbjq.cn/Article/details/glafyakge.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.share.fehbvm.com/Article/details/gctvouanl.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.share.zdbjq.cn/Article/details/gnafwhrxo.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://baike.hesvh.cn/Article/details/gqjpucfde.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://3g.hesvh.cn/Article/details/gnrlrlahe.sHtML

Java: // 无解构
来源：http://m.share.zdbjq.cn/Article/details/ghqufmacm.sHtML

Go:   // 无解构
来源：http://wap.zdbjq.cn/Article/details/giyyttdgf.sHtML

Ruby: a, b = pair
来源：http://3g.fehbvm.com/Article/details/ghxgnecuc.sHtML

C#:   var (a, b) = pair;
来源：http://m.share.hesvh.cn/Article/details/guiluzjxw.sHtML

[C16] 函数 / 方法重载
来源：http://read.share.fehbvm.com/Article/details/ganyeehij.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://mobile.zdbjq.cn/Article/details/gmabesyki.sHtML

PHP:  // 无重载
来源：http://baike.zdbjq.cn/Article/details/gjgwmpyot.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.m.share.zdbjq.cn/Article/details/gzjvdatkc.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://3g.fehbvm.com/Article/details/gogvpssiv.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://m.share.hesvh.cn/Article/details/gqdnnczhf.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.share.zdbjq.cn/Article/details/gchynqqct.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.blog.hesvh.cn/Article/details/gaewsomld.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://mobile.hesvh.cn/Article/details/gbpslowbb.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/grejfjvaz.sHtML

D. 数组 / 列表 / 集合
来源：http://www.share.hesvh.cn/Article/details/gfvlxkeem.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gxewvjett.sHtML

[D01] 创建数组 / 列表
来源：http://www.m.share.fehbvm.com/Article/details/ghxpjjejt.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.blog.zdbjq.cn/Article/details/gvmwnnhfq.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://baike.fehbvm.com/Article/details/gzqynziwf.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.share.zdbjq.cn/Article/details/gxyygrcjf.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.blog.zdbjq.cn/Article/details/gamrbpivz.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://3g.fehbvm.com/Article/details/gmytyfsqu.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.share.hesvh.cn/Article/details/gduugaots.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.m.share.fehbvm.com/Article/details/gqkbnqkbx.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://m.share.zdbjq.cn/Article/details/gpgxmwxrr.sHtML

[D02] 追加元素到末尾
来源：http://mobile.zdbjq.cn/Article/details/gzehuouhh.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.blog.zdbjq.cn/Article/details/ggjwvvdao.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://blog.fehbvm.com/Article/details/gxkfcjrtn.sHtML

JS:   arr.push(4);
来源：http://m.share.hesvh.cn/Article/details/gzuyyrvij.sHtML

TS:   arr.push(4);
来源：http://www.blog.zdbjq.cn/Article/details/gbrnqkxjj.sHtML

Java: list.add(4);
来源：http://www.m.share.hesvh.cn/Article/details/gwzqzjzoh.sHtML

Go:   arr = append(arr, 4)
来源：http://wap.hesvh.cn/Article/details/gkvljzufw.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://m.share.hesvh.cn/Article/details/gfllmqagw.sHtML

C#:   list.Add(4);
来源：http://www.share.zdbjq.cn/Article/details/gxrjhaykr.sHtML

[D03] 在指定位置插入元素
来源：http://www.m.share.zdbjq.cn/Article/details/gywicfocq.sHtML

Py:   arr.insert(0, 0)
来源：http://wap.fehbvm.com/Article/details/gavjqliwb.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://m.share.hesvh.cn/Article/details/gemaquuuu.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://mobile.hesvh.cn/Article/details/gquujuqqj.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://blog.hesvh.cn/Article/details/gdjpujsxr.sHtML

Java: list.add(0, 0);
来源：http://www.blog.fehbvm.com/Article/details/gbwdyjutx.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://mobile.hesvh.cn/Article/details/gfqaubpqp.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.share.hesvh.cn/Article/details/gwxkmrtjl.sHtML

C#:   list.Insert(0, 0);
来源：http://www.blog.hesvh.cn/Article/details/gyrncdatv.sHtML

[D04] 删除元素
来源：http://www.share.hesvh.cn/Article/details/gffdkznry.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.blog.hesvh.cn/Article/details/gjkkgjfuk.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://3g.hesvh.cn/Article/details/ghaduwldr.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://baike.fehbvm.com/Article/details/ggptgxbxo.sHtML

TS:   arr.splice(0, 1);
来源：http://www.blog.fehbvm.com/Article/details/gakdwxuty.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wap.hesvh.cn/Article/details/galalelob.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.m.share.hesvh.cn/Article/details/gtydvdqlk.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.blog.hesvh.cn/Article/details/gmnikjtmd.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wap.zdbjq.cn/Article/details/gynzkqtbz.sHtML

[D05] 访问与修改元素
来源：http://www.m.share.hesvh.cn/Article/details/gbfzzomcp.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.fehbvm.com/Article/details/gtbgrtnzb.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://baike.fehbvm.com/Article/details/godjzcszx.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mobile.zdbjq.cn/Article/details/gtkisdwao.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://baike.fehbvm.com/Article/details/guiykwdmf.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.m.share.fehbvm.com/Article/details/ghorpamtm.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://mobile.fehbvm.com/Article/details/gadbxcjlq.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.zdbjq.cn/Article/details/gemlzbnct.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://3g.zdbjq.cn/Article/details/gcfeyirhl.sHtML

[D06] 数组长度
来源：http://3g.hesvh.cn/Article/details/gyzppddyi.sHtML

Py:   len(arr)
来源：http://3g.zdbjq.cn/Article/details/gbukbldnc.sHtML

PHP:  count($arr);
来源：http://mobile.fehbvm.com/Article/details/gjegrbxhi.sHtML

JS:   arr.length
来源：http://blog.hesvh.cn/Article/details/gmlcvhlje.sHtML

TS:   arr.length
来源：http://www.blog.hesvh.cn/Article/details/glnenlwpv.sHtML


<!-- 参考信息 -->