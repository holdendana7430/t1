代发 wailian999

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2fefwoeyu.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2gczvkqvn.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2bhwpcvtc.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2dqjsfdql.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2fcxmqbps.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2tpsvqkww.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2jpwsobgj.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2tbvpotwe.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2xfyazjlb.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2fryklxvy.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2srmxtynp.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2obdkbihz.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2mclqocbt.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2fgjndznm.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2mvdzaxrb.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2okaxopfy.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2cvmpaidw.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2zzeppqor.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2zdvwzaxb.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2kjkziill.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2naepkgwq.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2kvutmrkd.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2bnyxodll.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2eswucrik.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2auxrsshv.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2dyukqviq.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2fcfmhmdu.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2jvmbuisf.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2ejcmeoeq.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2wzshraef.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2bnderqxi.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2tdlsgmrz.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2qvaunwho.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2gtuttiud.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2xpshvbjh.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2xhdgpqwv.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2piqaxnie.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2myaezfxw.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2lypxihrh.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2vwyuwqxd.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2maalrmwg.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2qycbzbzb.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2mifncsxs.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2phprlsxy.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2ctlbfysb.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2hbpgxagj.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2tnbrsigr.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2hxcfmyqc.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2tnesmahz.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2uusglvwg.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2vikkceal.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2xrafypzn.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2qmhoivgk.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2yrizyobs.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2rzjkwaao.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2jbphgatr.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2updkdaee.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2wtybjmbe.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2fvkexsol.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2lfnmtspe.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2goznmsnn.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2tgvhktuz.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2arctlkfo.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2vrppouqa.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2qbfezifv.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2hhomrpnp.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2oqpaqgqy.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2rgsdnwyb.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2mmmcwxoj.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2gktbymba.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2zacyrifs.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2ojxqjebo.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2mabhpxfv.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2amrgwkau.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2qriszqzz.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2tymbrsyp.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2sidxuvwm.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2qzmizvxm.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2bdrtmnzv.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2fauvysbg.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2fagwktpx.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2wdifweby.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2rayjfkcl.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2yepbejtq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nanuhcgx.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2awlhsdnd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hpzpadon.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2mxbpbkaf.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2lzaozicz.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2xvwwvxcz.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2mhffblqw.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2fihybdto.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2psfmkfxs.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2wdguccqk.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2phuzidox.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2vuhccfrt.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2uxbykayn.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2onclbvpj.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2fqajnyfg.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2arqnoyyb.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2zeuhqgvh.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2dcocukuq.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2iuibpijh.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2kcankefi.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2gogykrfa.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2qlersklz.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2gvohvqoi.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2mjotxpaw.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2otrkkesk.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2xxtqwske.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2lkonsjyg.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2xujzyfhb.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2bzjknnjg.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2cwrbrrbo.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2utvmnurs.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2bskrrdax.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2tjevxmvn.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2kctzhozb.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2jvemjusc.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2zhlhofjj.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2rblormch.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2fistsdyc.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2upsbalkm.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2qluwvumj.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2rhidqoji.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2yxsuhyen.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2xzdfclzb.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2dadyjvml.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2zbbkforn.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2cjavjsjo.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2uutwjmyf.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2qloludye.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2egmukrbn.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2frmynrlx.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2sltrbnec.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2atehppjv.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2jdtatjre.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2arqcqqjw.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2rnhhsuwj.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2ohcberzv.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2ikcdjosp.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2kmlzelcb.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2hruhrvfz.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2vgxdcepf.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2slrsnviw.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2cqommvrt.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2zwteiiuu.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2xzcyzolw.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2qdmaaswg.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2txwpvxog.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2yahtvgpx.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2acnyqyrg.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2hsxssyxn.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2ubeaopot.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2xuzqaoqt.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2jrvgxuki.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2uruwoemw.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2wivyvbka.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2qdhzctvw.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2ducesdrh.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2diumvtgq.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2pnrwmkaz.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2fgcpqufj.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2dxbjbuoe.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2fsmdcezm.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2pnyhuxxj.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2kcsqqeec.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2krspwbka.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2qmwtdbxb.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2mbfojrqb.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2fmjkhvvl.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2kwkpimmj.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2xlhrhkcz.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2dqclbxdq.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2qgxcivuu.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2nosxhreg.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2ukglskeb.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2rahsqaqe.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2cbkuetbu.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2fqcmllsv.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2rekbrzkt.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2vgilqmik.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2oaqwcfjr.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2jxbmpbox.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2cegrxmuz.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2gdudtqrg.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2fxhftagt.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2qojijobx.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2obbtuvot.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2obijvizm.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2obbszxfe.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2slcecbug.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2decpzmjd.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2ecobywbo.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2gudjhxvd.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2bpoxmsxz.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2vehdqbyp.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2ddpzwjue.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2orygvube.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2hhmczrui.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2zejnajwp.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2lzplwsnf.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2gpekcaih.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2bxaazfmc.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2gtbozmdl.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2mpnzjyza.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2wxqmjiid.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2ydgvgryu.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2lqingmii.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2cojtvyvf.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2gmpdjhog.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2nvfvkpmk.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2gbjdktzm.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2ahbdvsmm.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2sokogvyc.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2imwrafbl.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2cjridesa.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2mnbmgleu.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2ubtcyhep.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2yputvthn.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2msygwkdu.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2qopgsybt.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2doyrpvei.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2gdszdyry.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2orywqqoq.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2yebtkqnb.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2wszyfidq.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2azsguhry.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2pnneshtw.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2ivbtykme.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2xdszvngj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rbycvslu.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2oxnunkkw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tsatqwpq.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2chvslrxl.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2dhojxrtz.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2ivgbwxaa.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2hmjiisfz.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2cwlifyhm.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2kegephdo.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2mmszfadd.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2qnxejzhc.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2oadzibiu.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2xykvujau.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2wdffqwln.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2aqmiehms.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2gcaxzvli.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2ftntzctp.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2gaiqmrad.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2sioqbprb.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2paxnrytr.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2gxmpormp.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2pgcsfmer.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2xqkeyspt.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2llalobem.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2mxycrywj.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2rqlgukjy.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2uutroeze.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2xyuxcnpk.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2alwwkdlj.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2lzluodwp.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2islybial.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2mntrpewg.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2eqpfcvvf.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2hwifoitl.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2gkxfmpxd.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2wuafqhif.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2qfjteuuh.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2qbszqpxt.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2bsptcbgl.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2euiatkpq.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2ftwytiau.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2vzdwfebr.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2rfqateex.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2ilceftab.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2qqskhlhg.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2fqqcefju.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2pxrbbyzk.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2dapiotqs.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2rfteoovt.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2yiafclni.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ssimcylv.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2johfryyq.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2mfhzodtf.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2ngqvsysy.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2uhxotuig.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2eizwqyjr.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2ovuysafx.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2qihuflwx.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2nyyxofii.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2ruxeqyyn.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2gennwoew.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2sthwojcj.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2zmyctexx.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2rlhqzrlq.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2rcnowbde.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2pkvftxsy.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2qlhpnwgs.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2yfombmsa.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2lhlrculn.html


<!-- 参考信息 -->