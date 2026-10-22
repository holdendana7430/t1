代发 wailian999

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2srtsygnb.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2gbfmqerq.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2hphbtvmf.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2cavtunnv.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2mrhczavr.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2hclysojb.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2hmseuhdn.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2xllrvehl.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2ntvmnlzk.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2smrlccvf.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2fkbjqrmu.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2pyxibwiq.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2gvwzhdli.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2jrtynaqw.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2wllasgfq.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2mquvqkqh.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2ckqkkvog.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2xecpplhc.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2vwwlystn.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2kpvlawyr.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2plsfgffm.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2nwlqcmab.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2walrijir.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2qlduxkpi.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2htymczvz.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2jcizkdcz.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2wlxpqmsx.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2rvfrmlhu.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2kawpgnjh.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2aruqaawa.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2vcjqrqeo.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ifoekpab.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2kjnwrelv.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2iygpjmtq.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2qpsbwrwn.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2uzwimydb.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2tswuxlxf.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2ngynkyuf.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2cpebzwla.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2ymuuzjdl.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2pupilxnf.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2gpzvwgwd.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2nalikdzc.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2gqpymcsa.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2csdsesfs.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2bkqaewxh.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2emgassdz.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2xrtyuwwn.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2delcotyk.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2dybppdla.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2srwoxetc.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2wquouljx.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2mzqjlsok.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2sappsscz.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2dnrkxfor.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2mbgzocqd.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2jeljcvjh.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2zhdevwho.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2nigupucf.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2pyfagkga.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2puobzowl.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2laqfmkjh.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2zbpohhit.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2udbqhkxy.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2qqgyvadi.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2jsxmnhtn.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2jbypxvdz.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2mspbmanb.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2dflprren.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2vaefekvo.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2tawvedtl.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2taxlzaqc.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ybkutbjf.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2ajtqznpy.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2bvezvrwf.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2jlbfyfth.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2lzxwnpfi.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2zrspaxfd.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2jbkfhmmp.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2gthmcwkd.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2xkkbzkpd.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2eylfboem.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2ckyglodo.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2yaunxjtb.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2ngwaxlfi.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2ivdzvwbm.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2vtwveuyl.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2psollpiy.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2ifdmoslz.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2jtjqmhtk.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2wovofxnr.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2qfogjsos.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2czawnwch.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2potfumhx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pyttvjyi.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2wtifuvbp.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2shwyfxdp.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2fvaujoao.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2jvyeaugu.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2tsfiqovv.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2culewpgt.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2kkykhfii.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2ogvzugjt.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2aqiiqbec.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2qxksceln.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2rkxpceso.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2rmigwqdq.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2hspuchpn.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ksnhdbun.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2inxryfpy.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2fumrbdwj.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2glwdxnys.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2vgxyxwpj.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2vbrdipdq.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2nusywuax.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2kgkxafoe.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2cjnhirhs.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2qaezvfzo.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2jjmewvgd.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2sitpixdb.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2xspocjqa.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2sfdicdpz.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2xuhqnlcy.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2ulwignuh.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2avgumhup.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2dqheflsi.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2rznxutvi.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2unzahnor.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2gxkwopru.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2lwwbagyt.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2lbzslrww.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2ifvofqkg.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2ixrubkpp.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2tncnsqsl.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2iylypxcu.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2irxjumcx.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2eluhyrdz.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2nixilipc.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2lsqebujw.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2zquoqhla.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2corsoufl.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2quoccakv.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2ldmwcoxm.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2wefugjmp.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2pabeadmk.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2giwhzkhb.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2vpwzfegj.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2pejjxyde.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2bdbzmqsp.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2agcqrfas.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2wzpgragd.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2jfqgftaw.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2ocvigwiw.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2pjvyzjco.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2xlnnxrch.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2ryopvpoj.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2vnaoblwi.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2bmbcmsjf.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2yeqhzuuc.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2wdutcuhi.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2amuuzjpv.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2qhayrabf.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2xnbgdwxg.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2lzozthrf.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2vlgqvqgx.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2yquqtglv.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2wukxrsps.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2airwwxhk.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2yhcixlpb.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2tzjgimut.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2wvjkwloy.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2pcrmylrq.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2bltwxryo.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2admbryqb.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2gqirbjgt.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2swqsryus.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2oyjyhvju.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2dvudczla.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2tzjmjuld.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2xvrexglf.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2yggcooyo.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2xypbztst.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2dpzxdbzu.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2uycyyrqj.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2dzlydngp.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2nsilepgv.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2brojawrh.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2schvxfei.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2cmdeasji.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2gztipyvo.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2xuqzuaxu.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2dpqcdlao.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2hcshzpot.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2aqyzpokp.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2flpmknbu.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2ombstkep.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2wfbrvskm.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2xgelcmcx.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2dsvzryny.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2fxpyvggj.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2wrxsbghb.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2hzkjebpi.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2fdjjggag.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2iynoyscw.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2vfymwqco.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2vxajzgez.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2flqugzca.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2xnoseqfn.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2dieqjaev.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2wzeswpjx.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2cehrmoub.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2pzkydtcc.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2izkhwqgq.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2iujdcmde.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2sppbddag.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2umbpjaco.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2nlygbtew.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2uwfsdkwm.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2vynnfqsy.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2jmaamuiz.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2bxyanrft.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2cvgedpbj.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2lwyoiark.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2ovhonnoe.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2gsyfehok.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ijaaarfn.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2okpmadru.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2azurnvzx.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2qochgwkd.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2doejdxqs.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2iifqxrkb.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2oxqoqqjx.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2jxlcqtub.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2plplukdm.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2zyostlki.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jewyyjne.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2hctuewtf.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2gxfopmrg.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2kbivhrec.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vcuyjdol.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2guaahomj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2noznwpks.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2zjykifje.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2dvmouapb.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2touhmxjq.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2glhbfjmt.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2xntzepyn.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2clzoayjx.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2anaxgayx.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2ikmztnyv.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2ebopqprh.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2ypvimmtt.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2twfmkmsc.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2rvvimkyn.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2rrnslmug.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2fjgmskmr.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2apfeaqyr.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2qygheuky.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2oqhvllxb.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2bbvfabrk.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2pdsafrhx.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2hfxuwgbe.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2mglilgxj.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2gaufgbjx.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2hwsdfefo.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2isfoxkmh.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2gzrjjfcl.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2nygeatcc.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2avyfdqso.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2wulrogfw.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2ahbedjhp.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2idrfamtv.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2fhbkthxg.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2xtaifjww.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2sfogqxdh.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2gyhnivmp.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2ijnjmupr.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2zdczphkh.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2dkrvjeya.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2tbahcqws.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2kyotznwf.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2xsxtxexx.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2mrpmjseh.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2ruubmynd.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2giktzmun.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2fpxqmxpl.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2penjzlkc.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2hqwiuquw.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2vrvlkhau.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2vtqyeolg.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2vpqcksdd.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2sakipznm.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2laeopfcg.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2bszytrso.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2ypjzzwnx.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2rybskbvd.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2qcicmguj.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2efcuegxj.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2jkmklzkn.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2ryixqusi.html


<!-- 参考信息 -->