代发 wailian999

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2jldjvllc.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2mysekmrh.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2uwcgptwk.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2fbyhzcph.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2tigxsxix.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2pyhcplwx.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2zwlkfgtm.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2pvtdbtlm.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2butkuvwt.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2cpslqrtn.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2pvcruifj.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2pwoxdlvp.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2dfgauicn.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2rlyudbwx.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2czyuglxw.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2nqamyluz.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2euwcjjwx.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2pafrixst.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2zimnvgpj.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2vnxrxafx.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2qmbnepvj.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2hllvqwap.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2ixyiztvu.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2zpvennwe.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2ajjhehsg.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2uablmspp.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2dfctrfxa.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2qrwwwaau.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2ethikakv.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2jqujuusl.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2vmvjncbv.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2bkcxrgmi.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2mubvxdin.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2edlfkcfi.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2taxfpylf.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2agdcsgcs.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2xsvknsdl.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2rlvyynjx.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2jhuhluga.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2ecpsjujk.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2rfwjcpvn.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2grrnkzsi.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2kommepnb.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2dfuavbrg.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2bawchnng.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2qbyvvwnf.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2qflafrkg.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2hcxhorrd.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2bgpztqtc.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2sdpyhizy.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2tqgpyegq.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ssigryww.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ugtcrusc.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2qxgzccks.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2ooalylct.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2suuqwyiw.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2zkcfemtp.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2ukwieoep.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2xvvcafgt.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2yphxymaz.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2skanujrn.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2qqmwzcvt.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2lddqggjb.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2kxpoxedb.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2jwdprfaq.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2rhcbzhhb.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2asgonlja.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2mrjwjizp.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2emebcrtb.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2qpvduotn.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2vaeolwcq.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2xvdlgejb.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2kykompxf.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2mytmkoxw.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2ibfmycim.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2csbgvrbj.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2wbteklit.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2bprgqmdx.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2tkvxjkto.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2drnggrdq.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2vzpyhpvd.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2htumjgcf.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2sjhtrbdh.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2afypbojg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dhbootjx.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2loqdqkmw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zyplfejk.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2qnrejgfl.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2oimrwhms.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2fjklrkxm.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2xpskfoza.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2kpnohhil.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2qsdhhyxx.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2dqqopqgp.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2svkqwljy.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2wiznbeac.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2exxtizsb.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2ijqwqyic.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2cepwgftm.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2baofhnta.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2fbpaxkww.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2ujehqehx.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2hkqyhimy.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2rqeepvfc.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2opfashsb.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2sashakcu.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2glamorjk.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2ghallyen.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2pszvsgjy.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2diraeyve.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2iscgrhhd.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2tanyiiut.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2wdhrklxf.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2epeghuuz.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2jusiflzv.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2rcqjovcj.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2dbiplgug.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2rjfuslbj.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2nasyirzz.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2ttioqote.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2thrdoufi.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2bhnfehhy.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2akmpvbgy.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2sjgfrfsx.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2vcuweewd.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2wvxelmrs.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2pquraumj.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2fwyxvaqx.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2jeitdxes.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2gwkblelz.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2evmwcidq.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2hkukvevk.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2fhfecqjh.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2cjhyitsj.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2npxiqdhm.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2lwiynuln.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2niccfqwu.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2evygiwnu.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2flbvmuaa.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2oxydcxwo.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2vgrvyyfp.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2yaqiyvpk.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2dnbarzjh.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2kdhzvgbb.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2zufkxwqk.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2twdwlnlt.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2vjipadqo.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2lpmyiqwy.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2lixclioy.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2vgyrbbsn.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2cajigtvo.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2qqecxogh.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2sigclioh.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2kyipsxdx.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2zsfhvhca.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2vqjnfmmv.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2lisowxjp.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2jhmjestp.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2vjwoapmr.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2gpxqpzzj.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2pqvzxjpe.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2sbrimbjb.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2okuxgcui.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2xwudbhqz.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2phnposgc.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2cqhzphdh.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2wmlswyor.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2yonfljds.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2lgyyioyh.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2xjzgwblc.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2dnxfxprs.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2yimvokln.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2xgqomszu.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2zohlunlq.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2kciypscn.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2tlpupovt.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2dhwbqsdx.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2krqmbbsi.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2jvogqmsj.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2yhfhdhun.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2jcghpuwn.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2wmangqac.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2sicyingj.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2nvbpblkg.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2kyheqaww.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2icamrqrq.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2vkfouhja.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2kfmuclfn.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2ooiwsazf.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2iqkgwaip.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2qstybcon.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2vltpjfnu.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2rcuramcc.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2effocapw.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2coavicpg.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2smkxaxfh.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2uqsrolac.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2enmnfiur.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2hpjshlek.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2yezwjvlx.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2ilxkokjm.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2osaasobf.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2dporvwqh.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2mszjciji.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2hsclhpnr.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2wtwnabsg.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2wrglkswy.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2afhekkkq.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2ndcvdpis.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2gzkobebx.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2ymsaezrz.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2xeuelqpw.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2nmauegou.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2jntgmayq.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2orlypdcx.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2bubqgkjq.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ubjpxjtz.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2aowwmfiu.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2qlbksndf.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2nqrrucpa.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2aofplhcl.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2zahbacsm.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2nqeqkfyh.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2zcpkfqba.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2shpxlwah.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2vatnidee.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2vhugrngd.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2iicjesph.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2apwiekkt.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2kmzuswno.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jjcthbhg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wknslmrb.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2btfhgmig.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ekpjytlm.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2woiugjac.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2adzbypta.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2hntmktmf.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2zqeszghu.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2funnitvt.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2rzjcgreu.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2esyhhivi.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2cttwjtkk.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2ukoztent.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2ryumedcd.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2ioejlsdy.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2ryianpbp.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2ncerpyfb.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2srlkraxb.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2otzjklfv.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2xqorrlzk.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2xzhbbosr.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2durhfwxt.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2opmlbwmj.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2oaswtgcs.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2zbazlneh.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2zvzxthja.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2ynumkbro.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2mkpqtddw.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2xattltoc.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2qkhikvre.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2moxogfow.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2jidkgimf.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2dwmlodoz.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2qyvwjrgi.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2wbpducdh.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2qvfcsffw.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2deebkgfx.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2auyvjlxw.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2qpkthrbi.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2vdjvudlp.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2ajwozhxb.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2rcligvot.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2rmmbwucy.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2yjrpecfr.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2lahlvgrr.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2ctxhuunh.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2nojevlhm.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2eewkfxgk.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2dbgrgnst.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2vzhyuwlm.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2mobukhjf.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2wqgeamsq.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2pvdiypvv.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2sqkmnazr.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2urdyhidj.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2wrklqiux.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2wjqxttss.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2ltaagdrj.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2cngnvfvo.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2zvtcehgm.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2jiqofcao.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2birmjuqa.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2qovyqvfi.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2dvknzsoo.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2reveucqh.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2sqkwgxfy.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2veycnset.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2gpiwgmkv.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2ptixbfwp.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2fcmcafvi.html


<!-- 参考信息 -->