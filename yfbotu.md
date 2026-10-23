代发 wailian999

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3ietbsirr.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3mtiignem.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3qjbhthew.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3twbhyyao.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3ngndcbmo.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3cqnykceh.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3ykyuqaju.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3mrvzykxo.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3deztdzrg.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3ldgdzjvt.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3tybcrydp.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3cfawuwgu.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3hivvuxhe.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3qcosesug.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3uynjqwro.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3jkftkuhx.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3irseodkf.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3gpbvxcpt.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3ckpcshbd.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3mpxyfoxh.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3pvygnszw.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3tqvlaruc.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3oxvuvqee.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3qrhmmemo.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3dwdbgojz.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3usdghtqf.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3hjclfjvs.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3vajnlmhn.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3ikepuknz.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3qdgvykcr.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3fnjppwqn.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ugteoykh.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3njjusjmu.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3jclmuyrw.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3yxlpplyl.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3zlpaepbf.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3uinqagyg.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3tjbettgs.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3jklfqexn.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3xllklpvt.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3lpofmqox.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3pbtkfoll.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3mmdwgkwq.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3noehylib.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3jojmllep.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3kfedrsof.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3qxqpjzes.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3jdqdnrds.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3eprerjbp.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3rdqpcywl.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3bahvnkca.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3fsgoovdd.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3xysdmspn.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3mtqkdeyg.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3brbtwjgh.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3cenhxali.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3osrmsyyv.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3pkddxbkz.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3rvtzsmrs.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3ekgpyuii.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ginwrfbz.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3pztwbyin.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3rqhcrqen.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3gwkydtua.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3oieqxzar.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3talqoqiv.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3iauiblve.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3uxtveyxw.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3stoylvfy.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ysrnewus.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3csefkvql.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3txvhywlv.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3wwqphjlq.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3rzntwdig.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3wyxbcitp.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3zuwxfvkd.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3brpwxzeb.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3uzrknxct.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3luuwyxcy.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3hehtfjkv.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3aqtbvyko.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3xrimcdhz.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3qxfewzmi.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3mzsktnfi.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3mntovqab.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3ngahhfpd.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3vpumtfod.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3zpekxjzg.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3snbnlagd.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3xnehescg.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3pyeijdou.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3uoofmdhi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jslbisvp.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3fbfkocwx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3osrmfwau.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3hdbfdnka.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3ltbuvxrt.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3pxklxscs.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3tynrudoi.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3pwilrdbj.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3pfauggwm.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3lkawmbfo.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3zrwmiirt.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3qsubdubx.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3rxsdgkyw.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3jevzizet.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3nmevcrma.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3axmmznjl.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3wjfhgiyc.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3ilddgboz.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3lhacifee.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3gyvwptal.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3szogmhiv.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3urxfrzcd.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3wlzerjji.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3aywlgncy.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3fywtdcqc.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3urtfhdsf.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3jxjleayh.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3nrkxdecl.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3xskdrmhz.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3slibluvj.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3zjrfskbs.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3jcrtnecr.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3vuxnhwzw.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qwxnqjwt.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3nfgqrnna.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3pbfjsemm.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3nmskgvto.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3xcdozadk.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3qkhqtpfh.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3rhyrjpew.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3ibxfnyaq.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3rburfndo.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3wwpjvnlg.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3zutsugds.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3cbmsqujk.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3eqbzvhoe.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3dfsoziyf.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3adhglezc.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3bqhdrfns.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3akyilekq.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3novohgzi.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3ewgjvlqo.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3tjrdmdfr.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3epfzwfdq.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3egwazoqq.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3uulrbicw.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3mzwdczgf.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3zrcxmpzs.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3mothxzjw.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3dmpktpnx.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3dqxqjdhr.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3lwfavqbl.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3xusmqsii.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3vylmezhv.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3revhndga.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3vwwkdlcl.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3ocvusgam.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3wayknvov.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3moeqovbn.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3danvzidj.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3kxpdnjal.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3xfywzxzf.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3whfcegxg.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3qikdzkyc.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3rjyfijdo.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3fnbjqrjy.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3djvklazu.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3ijciuhqk.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3ldcuoirq.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3wxetlnfd.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3nqkzrqbx.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3nsreqpug.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3qihzreet.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3iuxqlaxb.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3gzcclopp.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3rkdudlwp.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3esqhhhpe.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3iohewkvb.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3stwamouh.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3vzftuuna.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3svoxnbhu.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3kweglnrx.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3zwwbiwso.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3mijjwqhi.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3inhfwssf.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3lfztshmn.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3racthyhw.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3jhbjqvxi.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3gvitfwpc.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3lxsacnwq.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3ytebfjvx.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3erhzrhyu.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3eavmungt.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3phmjwffk.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3zsaqzzrv.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3bursttic.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3wylukyji.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3iwodpekk.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3oyorwuow.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3bjlnkxvk.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3bvcwutqm.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3fsmzrink.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3maahjggt.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3gklqumld.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3nieumbgx.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3urvyqzhp.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3fzwgirbg.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3zaslbunv.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3zfwajlxl.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3jbhwgdhd.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3wlpkrcxs.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3xotjlypt.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3cvxvfrdd.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3hljgjrgr.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3wbkcjoiw.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3giirlucz.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3duxssfyu.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3pltcqwdg.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3eimsjkux.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3ckjjaqyn.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3kihxujrw.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3rbhytrlb.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3djoihafh.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3izyiompz.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3edrooqrr.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3watjtwbb.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3paxfdttb.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3uqtxyjkg.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3mtfhavoj.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3reysarux.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3hybiqfhc.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3xnrmbnuf.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3yfiebbwc.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mdwdmhcz.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3avunnyxs.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3xbfjmpdm.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3aromwhgo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gxpqatsw.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3pbwexjlx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nfbkgsux.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3nmckvycv.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3lqiccuux.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3wzbbrapj.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3qsuwqdzn.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3msrglomq.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3wmnjkymd.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3fgcyxoxg.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3olofbmcd.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3tjbsxued.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3zhlsocge.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3cvvyxigf.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3bxdqucff.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3hppwjvzy.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3cjqzkxjg.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3dixtkxpd.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3dyszcgiw.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3lgasjafq.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3mrwgxyxv.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3uabibzox.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3jodexnlb.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3nlclqudr.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3nzhqeyml.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3zdptavkx.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3cglbdvtz.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3tjzbilqf.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3ogjjtque.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3ynktnked.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3pdlxjqfn.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3nmhchbnx.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3zfcptuyy.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3exnsrmke.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3bkcbvrfh.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3leqcqqfo.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3pkpdmxec.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3ojfltihs.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3zebytsmu.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3yazdagsu.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3ffbcaffz.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3vnnenmqh.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3gwrtbfsk.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3scyxpjoy.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3rcwhdkvd.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3fvrowzqf.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3gpncplmw.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3vflkgqmp.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3ugxojonm.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3ozjxsdyy.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ghbwrxmi.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3ownjqsyb.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3pujppybc.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3evqcghuc.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3yxwtxckp.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3ujbwblsz.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3luihclim.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3aktqyppu.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3yodnplnk.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3jdanoscg.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3ypgkpqwm.html


<!-- 参考信息 -->