代发 wailian999

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2pbpstnpx.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2iavhmsbz.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2rtuvmfzm.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2wcrnlvsy.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2juxighta.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2idwniusj.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2cduzxbog.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2surzhekr.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2hdetslxy.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2sjpnpsgx.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2axnmjzdc.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2qgajmhrv.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2cifbieml.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2jvbbtvzl.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2napgnjsi.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2xeoxsdzj.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2kaflmbea.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2pturyrgf.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2ujbntksa.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2yhiwdiyw.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2sudiwnhw.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2sejwuhjs.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2jubdzjsn.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2htshquhz.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2wqvoczsh.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2illcajmj.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2yaszxzzo.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2zkwmoucz.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2vofdxlmg.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2ahsyimnc.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2bhnaxfao.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2fxnrqsen.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2dzngylcm.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2izpeziqe.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2psaxemdn.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2clfnaupp.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2nffdyjvw.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2gszecrur.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2aljgnmvn.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2lxmpwybq.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2beajsesu.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2yetxpqyn.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2wsobvsaj.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2tvsdayit.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2zaqmpgtv.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2zxyrwxhs.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2jejjqswr.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2njszypet.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2xlsqjyrt.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2irichwge.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2fggwgodl.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2evsqpimo.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2jrrmapyz.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2gdfglumf.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2dgpiwogx.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2oepjkohh.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2zzqnhpnq.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2zeprtppa.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2tavnqcaf.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2wmticdsk.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2whfcoodv.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2xokxiutg.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2vhzndgdc.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2vjpfcyqg.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2nzfyvpdc.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2obeaqqwr.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2aowrewfh.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2fhyafxru.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2icbtvorp.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2voilumgu.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2bmezblcd.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2lzuwobeg.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2zqxtlkph.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2ymkwgyon.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2bunxwjzy.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2ogrirxix.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2iddrxrnc.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2aktjoceo.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2sdwtaycu.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2lhhuzxaz.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2yofvvbdp.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2kdywgism.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2ijjeotip.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2saajcfoy.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2rwybrfas.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2lukdmqka.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2qdxpqogu.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2lhzgjxwd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nwslfqsf.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2yhuohgas.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2sbiruoeb.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2oebaomck.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2wmlplylp.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2edpnzsts.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2fgayddhy.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2adirnlev.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2cbbnhpjx.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2iubcjvyt.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2syjjiahc.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2fnbikjry.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2uolodvsd.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2meftsisr.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2uthermae.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2kkvfetki.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2plnbuesx.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2ypmkqmfu.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2vzlnicew.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2kfhotuds.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2jxdemjxd.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2fnfevzxe.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2fceardcm.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2qdxgisfc.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2elxoraym.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2srbrblpb.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2djfytpos.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2bqpbuvsc.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2xilgkety.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2pybfmdef.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2tvgcxfyj.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2wqfohhzu.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2aowdtzdj.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mpjkxhsf.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2bullhvay.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2nrvtdfht.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2fdtskkkl.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2xrkbwjft.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2xzkgnpxw.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2fjrlxaig.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2mcgkwkdg.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2swjhnotd.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2kibqmtdy.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2oxkiynym.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2eexttpui.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2djljqmkp.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2nizexmar.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2thtpzswl.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2hrsvcfvm.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2psekchkg.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2gwytxvyz.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2oluhmdug.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2aqkfdcjc.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2sxvzgvsa.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2mqzhgpnp.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2hsvzhaaq.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2seneaorg.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2qijtlhav.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2sshvocda.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2vqujbymw.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2spklkanj.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2yhpidzjr.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2lcdtoabe.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2msrhkvsq.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2othiabru.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2xgwgugtd.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2vlpdpusj.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2viqhycpc.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2rhedqjae.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2dbkfyzpr.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2lfafvfhs.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2ihybqrnn.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2zdncuiwy.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2easzyfns.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2awknjbcs.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2txuqmqkt.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2mqyfegpk.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2mybgwbia.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2rbadfswk.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2xhkeqqmt.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2wdwxbdtt.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2zxxdxgaz.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2xfdylbyo.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2ydfyjgte.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2xguqlftk.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2ahlbbiiu.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2abfbszwo.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2kpzxjubp.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2pbqtdryt.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2pytesrph.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2teaickss.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2waeasaak.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2kcuxcrch.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2bahoyatz.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2xmhksxye.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2aryyqwed.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2kmvovlef.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2xbhlrkbf.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2lenakbpd.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2llttznej.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2edjrehni.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2gfeyihcy.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2bmhezxbo.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2uqdeuoya.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2faymxpbc.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2pnerajjn.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2ibogkvcs.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2qejsttun.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2jyzpeuip.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2atejwwlb.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2yododncp.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2jbeeqqbw.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2htxsztei.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ioqzkjoj.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2rzbxgckm.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2fpwbtwnh.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2tzsdbmqf.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2ghykxdnb.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2ipfuwidy.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2zxyvmsne.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2fxhwguav.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2ejjsrjev.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2hxtirjos.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2ezajvxik.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2hjzblusu.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2bjascycp.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2sbrieequ.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2gfetwzli.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2egwefxid.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2qwhgwmkx.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2cokzjgip.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2tjfitqdn.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zkdapsrw.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2dfhyqkrn.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2gafyvxcd.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2ncsjatka.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2fmamyvqf.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2mpamfwny.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2eawnwvlc.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2vieowjwx.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2vacnjcmh.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2eylsdszq.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2xmwhywcz.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2sxejsldb.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2iujqonzt.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2eybbyquw.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2ozdsrdlv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yihyjqqc.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2ioxftkqc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lpyxpqdg.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2hldpqjfj.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2nzwyllks.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2vpoaqndp.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2opzntaex.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2yffgtkln.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2wvhbpfbi.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2movvepvb.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2fwqhdocc.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2cjlgcvhw.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2vmlwnoxk.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2nlfbmznh.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2tnfbebyu.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2lytjnmuw.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2gmvhiatt.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2wbcmlmwb.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2wrhdjrwt.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2vpagdxpm.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2uzhnxjkj.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2jlaajlmn.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2keqjlllw.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2soyrtqtl.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2sxtvlexd.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2gqagmkuo.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2witbswri.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2ifxjubve.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2swwdzajs.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2obsgbgbp.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2rjwabupz.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2obttsqdn.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2lvmferps.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2valmzvrn.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2bhwfobrg.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2tisdppcj.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2ooqwgdfq.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2ysmqxzfi.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2dnemsosp.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2iepxjmew.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2yxahdxul.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2tesqddlg.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2qatvmoux.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2exnwcnig.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2izjteofv.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2lurvaphe.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2jlpleush.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2huvrxkiy.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2zaihbjjz.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ltvmvzjo.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2lplydlgu.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2osrdisma.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2sbanmasr.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2yiekqqld.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2hdvljkyr.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2nqhasgyk.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2akzjneoj.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2pndjumha.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2expkgbhb.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2auziutnn.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2xpnnmrth.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2pbaissdk.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2kwrznoea.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2gcnnwnzl.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2exoyjkbw.html


<!-- 参考信息 -->