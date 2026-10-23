代发 wailian999

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3ondhsnwn.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3mavdmqiz.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3qantbuvm.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3vgbqzvbx.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3zxzhdkgj.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3iwtbegcp.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3fdmrdebs.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3pqhcxqwg.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3ntjczwfe.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3binaeakq.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3xjqqdbcs.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3urqpoaxn.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3pxcjhcvi.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3rgqzukle.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3eddvifiz.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3qrdecxpn.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3ovfcnjqh.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3uxtatroo.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3tetxjlda.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3xucdxlje.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3stxnqaps.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3iycbztio.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3nkcvenjv.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3qkpozdud.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3crbunqof.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3jmshdtcd.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3qfgejanp.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3dkvsmldf.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3vzkjcrml.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3eticagyk.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3wnyddazi.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3hnhwjuyk.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3qkuvpzhp.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3yekcpudk.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3fsnfdeyk.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3qotmrfvz.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3qdnipjqz.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3auitjsmd.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3zbqsysqs.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3mpmcghic.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3ryslamjh.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3aqqtsdba.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3qejrnioo.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3ajebeawi.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3xwdyfpvy.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3hswbaayy.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3ncetzuks.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3aqtnhxfs.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3jfxxesuf.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3zejkhiyk.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3ounqmvbo.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3ndtpvclr.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3gwqstmcp.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3kebwbymn.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3eoojikvc.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3sibjydny.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3fnduinty.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3elfflulu.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3auowiqom.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3gdavcsjp.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3qblfsibf.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3ezukcbkc.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3ksmgekqp.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3zjgngsaj.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3hnjxsjdy.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3avmvqajs.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ifukugjl.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3xagjteof.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3febomkbw.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3chlmwzvl.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3drygevlo.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3jpznfisq.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3woqyozqa.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3zwwdprjg.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3ddwajdtd.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3pnkrhoua.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3iflmhgqq.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3zxfitdwn.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3kgnllxys.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3oxsdedbf.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3ggniyywq.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3ofwvkyos.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3yeruvgnw.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3kleomjfk.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3txxlrnqt.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3lmomqony.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3taldudlc.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3twmngdhp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mgwxoaih.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3owvwftbt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yqvsxjba.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3hkzuatso.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3wqijbije.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3sgigpyrf.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ttyqzhxr.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3rcubuauw.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3fgiljwzb.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3iuaqutav.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3mkecubut.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3xnxnxpix.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3sfdwaoqp.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3xwhsnjhl.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3vzchiigh.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3izpwjgfu.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3trzabgsu.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3pntnxrkx.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3dwnzysfa.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3vluhfyle.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3yllpcwyh.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3efnwynso.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3oxffbjdj.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3kethgxvl.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3unawriys.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3iafnalkg.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3iswmoonn.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3rngeusrn.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3dzllpfbc.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3oepzyejn.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3ltmslgse.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3hvrfkxdd.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3aubfjsum.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3nfsknnkx.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3gywypvjb.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3ohtjwwsu.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3dqrgulcp.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3ctacahpm.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ifljfonk.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3qatywxlc.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3jpbkowuf.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3ecurjpfk.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3wxgfutwk.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3pteokzlu.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3bjbzjuyc.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3cmrdkuut.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3bbsurhlp.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3imkocwun.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3uwlcognj.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3dzvmpizw.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3hjgurair.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3slgddksq.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3zqqpmoek.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3ykcoveja.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3whoksqvj.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3sexjcrgb.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3ikbnjgml.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3wwjbyidd.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3tggqmthk.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3iicposbf.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3grnapkcp.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3ddflquzn.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3ecgpqtmg.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3rqqspamn.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3ethxxvyd.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3bnzdoqzp.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3wxkqggpg.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3ovanwjey.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3glxdzbpv.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3dmzifwmp.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3sizgjpxu.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3txbonphc.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3sbhvkbiw.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3rqrsimdd.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3zmefouwe.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3waswuzsk.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3ahngbrps.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3wyrsibbo.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3rifevqai.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3upsishtt.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3zjblgyww.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3uwkhxtrt.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3oqfzheej.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3ewpvisgh.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3rfyzjbeg.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3vjgxpipf.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3fiprgnoq.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3nfcooaaz.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3bmssveub.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3xjozhaob.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3zoyinamc.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3tdthobic.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3tcpwcydi.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3gyygfysw.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3idakljox.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3mwovmyqw.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3tsxfhlof.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3cqnurywa.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3wsantzul.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3xzovkaen.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3tzzdzvpe.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3wuodyvze.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3ljdiveog.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3dmimewum.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3oadjdnjt.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3cipareiw.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3gfzrysbr.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3kdytqzer.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3wckfhskx.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3dsmivtry.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3szvuuhts.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3ikslxtvo.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3enitrlmu.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3varvrbzn.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3ihrqinyl.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3psajmjon.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3tfutriay.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3yfezvmwo.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3sodokloy.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3sqliwjfk.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3awoueuvl.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3suwmgfjr.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3iwgjcjxe.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3gmjhvhbq.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3zxmxjjjk.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3qxzsocts.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3dyfpeyng.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3nqnflpvr.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3uzozhtzk.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3jxuckmnq.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3urnutsai.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3kdhgilzg.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3otfajfqn.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3celpkbas.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3xuclklsw.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3sadwkkrv.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3kkdyztkg.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3jfbalfah.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3ctoczzon.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3iomofmxc.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3gtrqecma.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3uhlaitoo.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3ccrwchxb.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3nvlthgfn.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3uugupryt.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3fzukyvte.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3lazcrkcn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jfpgvqbr.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3xzosnrtl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3shrceuhg.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3tuczsphh.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3pdymvbxp.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3pqawltzc.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3gxqtsluv.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3dteehuck.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3djdehjkd.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3dgmaxdfp.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3oifigyrv.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3ygevcifg.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3mukmhkub.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3uwufjupp.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3lyaoggui.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3cnfkqcxe.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3xpbyowgo.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3oxoqdegi.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3oamsnpmw.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3pvjffbxw.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3zeslgyqr.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3dylseqta.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3xbpzaecs.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3sibnrchu.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3mxjebiqc.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3tqmfpdbs.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3tblniayp.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3zsnsqhzn.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3lsvknrpc.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ibcdwwee.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3gbajaszr.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3ulcavsbn.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3zltkyfym.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3megbdpci.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3bikkxzqt.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3caosyeii.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3hnkhrjvi.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3kweenrca.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3zepdpioa.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3savwptnh.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3vpbchkci.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3vitliotk.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3viguijxg.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3fdwxwuml.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3uzcxcxyc.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3ixmxcghg.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3osvjqtke.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3nxadkvwf.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3ugxftdqd.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3wxtroomw.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3qqwerlhg.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3ecvplezd.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3ebvrzwgc.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3gagtenux.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3bttungvl.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3teegrkyx.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3csblkxwq.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3dcvjkiar.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3nomxywpk.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3axkklxee.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3smxtosbc.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3kxfgscxr.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3cdtgsqlj.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3dgdlhbcw.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3wabwiffw.html


<!-- 参考信息 -->