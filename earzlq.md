代发 wailian999

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3uhwrfrms.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3mtnlpyho.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3efadqoqi.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3jtvpbusw.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3cacwckvf.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3ehofudgj.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3hwxlxzzl.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3jbyjbonc.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3cvkztsbo.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3twsncpjz.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3fzsfzche.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3mijedngh.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3brpyhnqy.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3zehzhoxc.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3fjwvjnvr.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3btxdgiph.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3txurenof.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3ytnsgdmb.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3polllick.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3afahyowm.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3peizuvgm.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3gpoghioj.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3mwaqkulq.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3gbdcywak.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3zuvujhfr.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3bldzniij.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3dgwaztbn.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3llenilib.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3gpkzgxxo.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3nfqbaxub.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3ulvzhahr.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3rubmyekg.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3alcxbqal.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3hxrdxysr.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3ruajapcj.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3wdfndxzs.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3zudwnutk.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3jafizkfo.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3fnvjnqlu.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3ynddpiym.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3mtphzkqb.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3szbrdhjk.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3erkneegj.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3qjyyytbt.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3wtrlbtub.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3rabbqiqq.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3glgglzuy.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3iuygykgv.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3wqeozoen.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3qhyokiru.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3znbmmcwi.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3zuckskny.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3woaunigd.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3rdupiffv.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3htfxoiba.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3hopjimlv.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3wnelhvly.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3vlelflmb.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3abugpqqq.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3rnhqrsfp.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3cnhcpwsy.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3bhapijic.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3sscbmxzl.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3ltdrqumw.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3adoexqoi.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3zdfioezg.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3iwpgtclb.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3zofxcjvo.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3gktultlj.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3qxvfnzsk.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3aougeonw.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3umtjjnlv.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3ufazdysz.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3ipijxjvx.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3iksbllca.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3rpjxpxec.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3ttqqidud.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3xylxxmhk.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3jljlzfzv.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3bcqokjie.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3txowrhqa.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3ndqjquea.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3ccwwpcmz.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3hhbnnvzy.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3hwklhamk.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3tnttqkuu.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3uoquqcsw.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3kuemzmyc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kxaxujsh.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3kszyfyur.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xnrpptwk.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3pxxidcwv.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3mlpimfkg.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3dpahzhke.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3zdqlntul.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3lfpxnwgh.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3bmoqgovv.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3vtfpxhxc.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3olxojhqu.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3gnbgktof.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3zhxnukze.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3jmmurfcr.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3mollrfqe.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3rggwplhi.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3ksghjiib.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3zyfhfapm.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3gtxswjov.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3hefutadw.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3poucxvfo.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3gesntcas.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3gdlsrzkd.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3kzleyppo.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3nrnwpqti.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3zniymzud.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3hfpahwyn.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3pebjoqqm.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3pmwryfab.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3asofhiaq.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3gyrtmxmy.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3iwtzeusq.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3wpsrubgh.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ybcehchg.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3uuemehyu.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3dbstmzqf.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3uztlgbab.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3yuhdfmbk.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3koagwtjx.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3yrpswwmc.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3fallpcdb.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3gmqckubk.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3peqbtfor.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3myesejzq.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3nbxzoivm.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3znzkhwkk.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3qeskxojh.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3dipoqafu.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3knlodqto.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3csfgnrue.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3dchjwbya.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3kuroaulr.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3kxycxgrn.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3gvnfehgg.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3wcwjlyzf.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3cqjwegtd.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3sixcerew.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3owribcqg.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3rbviwwbg.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3oynisfpm.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3luzjofgg.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3ixifrqlm.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3byyacvcx.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3kqjfywwh.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3uyxaknyv.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3hizmmrgw.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3mhknwmnf.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3mlehcxai.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3ybyowwrr.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3gmpmilgp.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3ysthsutc.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3ctmjgyqd.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3ihnmutpw.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3ypcpqwka.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3ywotrnqg.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3dclxizha.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3zqzqquxu.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3qmntwfbp.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3hugootdc.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3yszotppq.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3mnfsjiao.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3tqmsvkog.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3dgwhyxhs.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3cjabhgsm.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3fcpscwku.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3binxhbyq.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3uvsgpgjv.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3qbsyruea.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3pkxtaqhw.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3htegsznf.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3jubxfppp.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3melkorcb.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3ednpuaqn.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3ekztzkcb.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3coytulzt.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3wxelmfex.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3ynqlabvx.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3gfiwjdpq.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3hwnyqqow.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3bokmgdil.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3jqyuruop.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3grhhmxyb.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3ltjargxr.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3ltfjwdzq.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3dwqrckgn.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3dotfsndt.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3ypffxpbo.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3jfmptcby.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3bdyznjha.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3jzibvvnv.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3jjpmfpca.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3rypewpll.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3jaoljfdv.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3liowgjsv.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3qcoupisa.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3hxnzcydx.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3dguksjyo.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3tvhhaqif.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3pemewjub.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3msndofat.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3rjqbvobj.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3qscltkep.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3jptjrzcp.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3dpefhwfs.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3kwolbgel.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3wxlvkdoo.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3lhljldil.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3ozvymdkn.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3lalpktbc.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3uocgyazr.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3tisjqehk.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3fkkwndah.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3odqddjbz.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3muemisdo.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3aytyfrvp.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3zcwymwvl.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3wkynhwnl.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3veyhbnpb.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3rleaucrc.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3kdzdqxvz.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3ptvmhzpy.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3zevuymkv.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3pqymtwwt.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gjvnpvpr.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3hgaavxuy.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3gppwjhhv.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ewtiyvin.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gfpvwijq.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3snkndiyu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3afasvskb.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3ewlxbvdy.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3npthchfn.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3fwuytjss.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3yidmxyaw.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3frccysya.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3mvvawbcg.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3qejgnksm.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3mqlvcdjk.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3byqtebqy.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3vhxyhobo.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3zhixnajh.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3pwddnayb.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3dgdtecyy.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3thibxjgf.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3ziwwfqsh.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3kifxjfjd.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3zcwudbuk.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3qippsgyt.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3jflpfodo.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3vthyrzuf.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3sdtnqxwq.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3vxuprjrj.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3brhisweg.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3olzxellv.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3zhaagjso.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3imbkphza.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3izudijnn.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3ascizjzs.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3vknbmhkn.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3xzwaphah.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3aksdjhtk.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3cwjcgvqr.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3segbfhpb.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3eaodifri.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3mmqrzwid.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3gstgtngx.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3ahohggpl.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3rbcolzll.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3rbliidtg.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3tygzbzpg.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3xqqsxzqy.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3npurzgwe.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3ugqxvomi.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3lkafmuus.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3ffdzrhll.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3wxakuasv.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3mnbmrntx.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3zrtgzfui.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3lxexncfb.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3cjinrbqb.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3iebqaphs.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3rvaabqvd.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3vefoexbn.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3qbqnxxph.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3esezqkol.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3trmqezuy.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3btyrdefa.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3wdxabebj.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3zuvlynsz.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3ihhbcwyk.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3jpxaejga.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3fohodarf.html


<!-- 参考信息 -->