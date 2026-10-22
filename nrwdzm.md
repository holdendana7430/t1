代发 wailian999

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2qzspvdgy.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2nuoreuud.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2lidubeef.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2kephueas.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2rktamfzy.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2tsslzxkf.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2mxqavxtk.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2gtkaefpj.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2hlagjruu.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2fsqffxqd.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2ikvluayo.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2jgpdfucy.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2klbcfrau.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2cvjrjqii.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2daixgfxn.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2bamucxyf.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2gqdhqocg.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2mavdnhih.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2uroylxdd.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2zjsvwivs.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2yrmmwabx.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2ahlbcgsx.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2jdforeao.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2svfplozc.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2eymmjfew.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2fkrpiadm.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2whwjkjmi.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2xsldoziw.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2vtptmdzj.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2tsekhbcb.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2ridxtvzt.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2nnnjcwim.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2grmqzmdx.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2scihnsee.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ysdrphvn.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2ddayripv.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2mxanoybi.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2qhvzuhud.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2tdpjrhfo.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2erjkbwdy.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2zbugpigp.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2ntziyqdt.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2dknfwjfh.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2jabcswuf.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2dlzgmtwo.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2wfcgcpol.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2veyakzfa.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2qxfncbhf.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2pefkoick.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2zzcygdde.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2gwxgcwjv.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2kprbjqmv.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2rtqhwnbz.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2qbtutmqw.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2pdocvbgf.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2kosgpzew.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2lzfzyqpd.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2xnmqurjy.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2xcnkkzxc.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2sjbpcdgi.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2quidbgnt.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2tixgfdwy.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2umdtswqd.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2txjistos.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2tzgfxria.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2jktmaeih.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2xrdexccw.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2gjkgysjq.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2wwwdvrau.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2gfwzlfik.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2necklasz.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2gulpsvkp.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2eobgnlgr.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2ucrmjzho.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2yemtgnqu.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2wtowzzcl.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2jyjtnlsr.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2fcrlmvew.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2zecgrjkm.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2fpylsbyg.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2hqdihdit.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2dhcmbwbr.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2ipdavjme.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2ahupqfcs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lmwwirwg.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2chimqwhi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vgynioyy.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2nznfccst.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2ahadvdzp.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2byfcfpyv.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2jrtugheo.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2dtlzlofr.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2klpsoxbx.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2nsyzcbhp.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2aaebrpwm.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2jivityrp.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2jsiinuro.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2acwcjpqt.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2siyhnply.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2vamazsis.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2tmmknkdy.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2gqdhofbz.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2huubdsho.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2aebjyeat.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2qeezciya.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2wvjegslc.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2kwxfpbrz.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2oatcagti.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2oeygmzaq.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2tufrirvx.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2ondcrarl.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2wifbbicr.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2tmfepqsg.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2vodhzspc.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2qlmtqrrk.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2yjppjvwr.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2vtpbbasf.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tyrdeaun.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2pcilqutl.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2fqhujxpt.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2teuvnggx.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2gzfaqqgv.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2epeggycf.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2zvrppxjy.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2dsbfueeo.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2bdobkvrl.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2zvmsxjsn.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2wghmzkcw.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2gngiraqs.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2bznqtxnf.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2ueqmfhwu.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2qiuirfui.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2bapqejjo.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2lcjylzms.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2lggohzaz.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2bqgdhmnx.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2imqwkmhl.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2oykjqqqt.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2jmixqaht.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2exievrbj.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2zpvizkaw.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2nvmxzefh.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2gfcpxhuv.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2tmwdhnkc.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2hnlhqqpg.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2nvbrlwtr.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2clnyykzr.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2obgbuyul.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2ommleluv.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2ywqagvnx.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2gwyrmqfd.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2ulkdhxit.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2rqretzpu.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2ooftezkc.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2rqvnpmod.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2rjwghstx.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2ikenqtnu.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2kmsrbqtv.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2slqoozji.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2cuoitnwy.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2rnqvpcoc.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2gnowjqbv.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2uxtyhswa.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2rbbpwjmf.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2vmquilkt.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2wohkhrtu.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2ktpyxuni.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2znuewrjn.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2uouvisjf.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2vicwhjzn.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2dxhwywly.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2djtwattd.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2fbxnpiem.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2pvqsxxnv.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2pkavzhlj.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2fojpkenf.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2djofiuqc.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2mhbartzt.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2rouooaqm.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2ipvjngtg.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2trymtyvn.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2bnjfcglz.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2eojjbiml.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2faakzopc.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2ocyqjzja.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2luhbpusk.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2hmgabqks.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2oihwzahc.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2jgourprn.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2ilhoyrtb.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2gmnkgeum.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2whfazoha.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2ugeineoi.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2bgraglzw.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2ikisrtmp.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2xdyzirca.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2hfsihkhl.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ohvbjudv.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2reruuajk.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ccwvenpd.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2jqrsfchy.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2bphheiam.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2whvqkrju.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2qdwgtvmb.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2tqxmiejc.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2jhekkwdw.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2lzndxqtr.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2owqbgmtk.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2ltlpgyni.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2exiymweu.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2amljhjkk.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2pcfhthtx.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2bjstpttv.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2yacdgzxc.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2tdlstbvj.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2yfobwndm.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2cwfewxpn.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2gwhrvbfp.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2fwvxcick.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2uylwxvxf.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2qurkdeom.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2wcrebrlh.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2xbcmhlrm.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2analagnc.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2guqkkmko.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2bgzccpyt.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2waupzqag.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2ikvztizw.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2ilmpdigx.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2zhzbpaxd.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2kyjglxob.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hbkqwkul.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2wyyxxeby.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yakjvwka.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2tbssehtz.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2kokametn.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2xozfzusm.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2ypuprner.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2xwqcktim.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2xjshuwfw.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2enhlongh.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2wnaynayu.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2jsgxycte.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2hatwsjtd.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2gpmnpinc.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2ogzvxprh.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2arovzuvk.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2prsuphbe.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2qvdhwpob.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2hgxikpck.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2bqqkxggh.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2ggxfaojr.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2rjjfbccl.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2fnciwoth.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2urcvmhud.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2thxrutyl.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2auwhuzks.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2bgqthmwm.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2mfxkycxc.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2gsgmwpoc.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2opuzksqy.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2kfvswndd.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2qohvdkqw.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2wegltumq.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2etdqgldy.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2rbgzamal.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2jnkfjjnr.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2cfxugzgq.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2cfmjehjt.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2wauewwaw.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2uhvzhqvn.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2nlcxlbdg.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2zitdtwfd.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2fqokqorz.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2ykksdlxb.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2hjckqxye.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2kkqkogka.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2hzerrtkl.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2edhpnkqu.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2dlupfcsn.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2wrchunae.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2dzohowrx.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2zcsrblmm.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2wgtylpmo.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2whvtokum.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2hemeusci.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2qaegdrix.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2rgkggqlk.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2qkqqfcph.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2tdmurexi.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2gqgojqxj.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2teyqgwoh.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2sefmhukq.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2qalwgekb.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2cebwbuej.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2ouxltpsy.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2buokvhwg.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2guxtmjqm.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2uxqpgcvg.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2vwocalmb.html


<!-- 参考信息 -->