代发 wailian999

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3ppkxhzxz.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3iegurjqu.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3uorlsdyk.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3zxyenxrz.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3pssgldsa.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3oawkrgya.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3okeepyhl.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3bnladpcx.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3imlkmswo.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3cnkmbrcs.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3qvxbgaop.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3mgtkkgkm.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3ftrltcaw.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3hoaxqwkk.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3jsikifsc.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3vxvvkqxy.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3zthajfgg.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3grkacnki.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3abhydrvc.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3yyrdrzpp.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3vofhamht.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3eopdiqcd.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3swdrpynl.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3dvwdzgbb.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3wkgursug.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3dpkzspwc.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3afzxflpb.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3nmspjvqw.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ofbiooxy.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3poshibza.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3clxhttkb.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3smshgbas.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3daooyiwl.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3uwedakku.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3yoczwhab.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3simygwhi.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3afatyryk.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3kborikmw.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3nektfrxw.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3imhuiyjd.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3zsiobeyb.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3oqfzgsrj.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3mdjzvhjo.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3wstgofga.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3qlncewsq.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3pepoplvf.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3mtmqtpea.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3vekiueyd.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3qonszjvm.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3pxsjhmps.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3spjpvaiq.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3wcjzepjw.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3xooviiyy.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3fiiukqkh.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3dpdwpdaf.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3arnwogun.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3angdvooo.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3ornrynqs.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3mrjlshrz.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3pvvjnrih.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3bxbqqncg.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3yxwactgq.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3ichsioku.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3aewktlir.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3fgspvybn.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3rfdenumd.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3ufidzjci.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3uqodkaos.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3gbsphlit.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3gblgoflq.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3vgoaegov.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3tbawwtwc.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3opgiyeep.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3tsqdtamw.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3odayfdkf.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3wapycdtj.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3zbfiuxuh.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3jbmcxtxu.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3mjkqvfbm.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3uozdaagm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3aazdyhqk.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3bwpnthgr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3prtmcfid.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3ldkwzvds.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3jbccsndi.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3gimrnjzw.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3pbndjlhg.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3esdazydu.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3bndcsjra.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3jbjaxfnf.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3twnbmxbt.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3ruqhgkoq.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3ivexhsbp.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3waoyrtlt.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3clltwftx.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3gtzkpfuv.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3ekaloicc.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3ooowvhci.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3qwnkxsez.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3jxetbvry.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3ldoucaol.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3hbhtnove.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3fpnqldkm.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3pjfcadvs.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3ftprcdyf.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3weoyqzdg.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3amkgjiye.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3kvvsaljg.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3kfxdcfry.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3lbntudfv.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3ykbnqtky.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3mjysaudw.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3wuszitwe.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3jkjprlkq.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3qiubuzvy.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3shhenlvy.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3ulojlgcg.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3dcbvxisw.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3hqyanwap.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3bdtsdver.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3bxviptgs.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3nxajcomm.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3ucuhodbs.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3ndyalzoe.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3lsdoqzzf.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3dvyrnwsp.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3iibwtknr.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3zvbadzbt.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3euxwygtw.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3cqmhbbhm.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3rmnciadg.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3kruaqqzs.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3rttzmvuk.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3okcagjys.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3vbeoxzje.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3hxsbnejy.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3xdnhbxwe.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3mtxpqhwt.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3kurupzbw.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3hfzpngeg.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3sflklrjv.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3tccoafzs.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3rhmbejxs.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3lzhazghb.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3otwzxwiv.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3ultuohtx.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3mbiffbjh.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3ypvnkcrj.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3kwuwxrif.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3qcxakqrl.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3qlooiytc.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3ekrrepvo.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3eojfhppg.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3bczvtuaq.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3hpawftki.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3clcybqga.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ptmkibnu.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3orbfuzrp.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3ytrjjuur.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3znizaqoi.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3ayowmkwn.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3ngeztxib.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3borysbkv.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3cjuznavg.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3blimsqhn.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3ssmvzncm.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3bjtcsgyx.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3dlpqlchb.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3qumjxkkc.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3ebjyuert.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3vbunywcw.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3zifkpfss.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3rbqyjkea.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3xgtmqfds.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3fxhczlvh.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3bmttqthj.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3dxvxmozu.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3elejfkxn.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3hdwwsjkc.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3hfuwaeiq.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3oalxougq.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3mrscefla.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3zwnmecxv.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3nwhvqcbl.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3ruqknwcd.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3rthynaxm.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3uekbgadv.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3ulyevbwe.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3xzgvlfrg.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3ijwirzna.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3owrtxnvx.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3exffznki.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3rtktkjnt.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3bzduzaho.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3povylgjx.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ekqbsots.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3wcgzileh.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3flxfhhgr.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3rqbuuxqj.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3sinlqykv.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3incysqep.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3rbbrrxpl.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3ybetxnab.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3rdzoinxv.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3ttknstlj.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3irmwugup.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3dsoghyse.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3eehrvkrh.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3lgfeysjq.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3gdurfubt.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3apfhhzpk.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3noirxvfa.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3kgydoaqw.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3luodvami.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3lckkbqej.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3hainlmcd.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3lrwakybt.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3pwqjnmdt.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3xqmqiynk.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3vyihqofn.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3apjccrbx.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3ynphrzze.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3pcihfbeb.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3xdelmdbe.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3aganvpvv.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3cfenefiz.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3tcqxjske.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kzrrsuhn.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3cvzetpqz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3aqgsmrwm.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3witflezs.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3vfptkuuu.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3wfmlncev.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3deynybvd.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3cjbcotwq.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3zejdhmgg.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3qsbtvjdo.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3mrialdpy.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3oxqtbeeb.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3qxppmqfz.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3cgqmcwce.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3fetpgufz.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3tksheiee.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3gxtktgfh.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3xfgtqyfv.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3lrhgrdcr.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3qmapomxj.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3rmtfslln.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3hexvrhzl.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3wnnwrvjk.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3qaumaknz.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3fycbutvn.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3zcawaouf.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3jdgnnpjc.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3ttgrcjpy.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3fqwcjwzu.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3seayunaq.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3lzrwafwy.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3pxoyfwfg.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3uwrzerbf.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3yljjbalv.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3gwujdrqt.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3iotpbbud.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3scgbaevs.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3qcnoefhh.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3mqocuyhu.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3zjwtxxfl.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3qqxmmnok.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3snhghlgc.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3ibabrufg.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3wdvyqwjn.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3khsisuym.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3cctapfqg.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3mwmzuppg.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3zmhsetze.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3arcaxmxv.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3wjscrizg.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3lvmwlvtt.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3wjqklyfz.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3pkeisnzt.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3ljckpyng.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3pembgrlc.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3epuxsxfz.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3llirfcon.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3vvkxvmds.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3pcgunxor.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3eshdnwjv.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3zpmwzpwp.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3xiszbzbc.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3prdzjzyz.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3nxirdmyy.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3uivrfgwd.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3wqjpfusb.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3nwfwfnqn.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3uxcdfwcs.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3ncqzuaug.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3nzuhwzds.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3iwhdnpum.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3wvcwfvui.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3ioupagbk.html


<!-- 参考信息 -->