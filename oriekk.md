代发 wailian999

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3txnyoptg.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3bzfezump.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3aziodrzc.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3ayogsndn.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3dkqejvey.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3jnofeadk.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3yicmstge.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3ddlectld.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3puzrykin.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3cjdgngfp.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3doqacslp.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3anfrhvps.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3lbwizwvx.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3uvnbyinh.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3cvflvyhh.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3vgdqhpil.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3bqsarmgi.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3lqhwelxt.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3uqelxxxt.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3xtygequm.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3qkffxutx.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3zpxbnfwx.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3vevanfwb.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3rjwrprrq.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3bigmjbfd.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3nqkigqjj.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3pejjqbxl.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3atnoizcs.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3dbkakgsq.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3lwflfatz.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3gswgvspa.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3kwubymib.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3qvgonjch.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3bdhfnsth.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3utbfdrhq.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3zkipfror.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3evvxdozj.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3rnyychpq.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3dbcorlpf.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3uzitmaln.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3atqqrrnm.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3xpbwrodt.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3umyfzwnv.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3fxcgphse.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3ukseeilk.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3mprfskel.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3nesrrkcy.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3bmonbtwp.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3ngxcwvzu.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3emphngoh.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3ygdambja.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ibmwyecc.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3dtepshcl.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3srcmcguz.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3nfetntgr.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3pinpwszp.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3axdmfdco.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3yhklhscb.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3ovpsrxnl.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3uduexvcq.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3rneshpre.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3uvmsmrpd.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3hkzcjtsx.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3vofcoqeo.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3lvkeuwpq.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3nuqizvul.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3ehyxpwgi.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3huxhtpqm.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3uieikphz.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3axhtwgsd.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3tyhcsuyw.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3obrvokau.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3adznlvty.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3tssdhmvf.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3doxhlduc.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3fesolczv.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3cfrwyfiw.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3ntssridk.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3xpqcejac.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3kvfewbtn.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3ofejqhqr.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3rhlyvyes.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3pheafbkb.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3jypezigt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xivjwuql.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3dxxzhlck.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ajwlljot.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3bqealgtq.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3jdtnhafj.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3zxqnczyx.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3kuxbacuz.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3aazmcbqy.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3ygfnuvtk.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3shmnqfiv.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3jwoyphtb.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3xijkposv.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3lcamfhbe.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3vubtojjw.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3yusrmkow.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3axvsbezr.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ouzaknkm.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3diinvurh.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3jghuccrz.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3qrsuudfj.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3kzcjuurp.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3mpazgrxr.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3dftbuqyy.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3eloqadue.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3rdtphamk.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3egatzuze.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3bjomrhoj.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3kfxcbhjp.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3uucgqbao.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3xsdksuys.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3hemtcqqr.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3mprzerjp.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3sklkbqnf.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3pisodvkx.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3qpltqoat.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3xtamoqjo.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3mcuorqkw.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3uhcewwml.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3okskjhdi.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3gouyuflt.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3lehjknod.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3oeliefwy.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3idmjigbn.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3dasfpkqm.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3scaedmey.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3niyiahjj.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3wnzagxuw.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3wbakscxi.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3qikdubei.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3vknbhxjw.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3zdihmfwr.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3wkyejuwt.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3juivhmym.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3hgdypgpc.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3vldtrmqk.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3dkfoayrm.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3iwtzwrpb.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3bzsfcxuy.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3qfrmlxkt.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3dwstgwuu.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3rzzduiuk.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3qiaraout.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3omanyeeq.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3qrklmwhr.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3ljhmkwcg.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3axubuibc.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3ecctfqrj.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3bkdknvtn.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3oylzutld.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3hreofvcp.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3mfmkgglu.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3slvzlqef.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3yfvzfwxk.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3wlawnmzh.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3lrnthctr.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3muwylnnw.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3hihauxty.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3gjyqurgz.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3vdcppldm.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3xdnyxhkn.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3cypsryxh.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3ziigdgvx.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3lkdvnfbt.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3tnvqrycg.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3xihhjtef.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3kebaqocc.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3wmrvopfy.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3jvgbfztj.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3ldaqjesv.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3phjwgqfn.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3nsuzaszy.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3kjvgnlqr.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3ovnrnnsm.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3abxdlvfw.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3hbydnrqh.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3yaczzbna.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3unnrjxht.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3drytcmdq.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3xwpedtrj.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3hqscqnxo.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3wigqyzaj.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3wvhgpmgq.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3dnilwnop.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3dhfjhzzm.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3pzxjyfem.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3mdjcpfyw.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3swnobwej.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3iermxnyo.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3mxzavjnj.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3fvcguvhk.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3hxkowxja.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3kuocafiv.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3rmjxjjke.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3vajdernd.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3edypbxie.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3oxmuzdqz.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3lawwpzxc.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3lcwisvxd.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3othfhuom.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3juqyboqi.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3motatpzo.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3pgoqqkio.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3sjxcbeft.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3fwzjwutr.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3ldpovfbi.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3mvnziuml.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3dridjraq.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3wuotjzpq.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3bpvkroem.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3zlowpktv.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3jcbuvlqo.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3koloczxj.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3qazclyoe.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3athfsblp.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3gryvlgqq.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3gibleenr.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3ybixlvjp.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3clcfuxzl.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3zchhtzeg.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3pgntjjsx.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3vospcyuu.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3zkgsnipq.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3indbliff.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3fijzycko.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3tjveicwi.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3iykjubjh.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vpnufdby.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qfsiczcz.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3txkjtdns.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vdonxzuk.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3lffvicoq.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3egixhurz.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3ubkryelu.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3ocwbwmnx.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3zdkvhgio.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3voycspua.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3ywzqeplx.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3drhkbtzp.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3dwcaxcvw.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3oxzxuzvv.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3uulwxbdo.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3htmwmsut.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3rdfruiwm.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3apjcykgh.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3pouyuapb.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3putkgvsp.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3ojeczwqh.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3terobiyw.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3lmmaeiza.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3bddpmzll.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3pyruwatv.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3tdwvcusq.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3glnwrvcc.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3zptxfmhd.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3mddztnul.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3jzpzeiut.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3mgcetmjc.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3lkjybgfu.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3ayasfjrp.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3lybtyttw.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3lmrgrxhy.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3gppjjfct.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3pdbommlv.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3rroqjpih.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3bdqhixqp.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3ovdygqej.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3mihmfduz.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3gjkydujj.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3jtlwcxyn.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3rwgjrspm.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3ahbhhbvu.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3grfyyuip.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3gbzsceet.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3kwwrysmm.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3ecsxbhsv.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3lsmdrocg.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3mcsqzigq.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ijynhkrk.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3oyafbidm.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3jgozwgpm.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3gzporpss.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3hajylrpy.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3izqkjlcx.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3vcdwtduq.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3hdthzmyf.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3pyzyjicv.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3ycdwvbqx.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3yxojwljn.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3vbwdtdtd.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3mzqejnrd.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3szatsvwy.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3qlawzqho.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3hzigaqim.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3ujvovowf.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3lcfookef.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3tzccrzam.html


<!-- 参考信息 -->