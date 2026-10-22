代发 wailian999

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2doumaapz.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2sbbfiqlt.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2frjrqqzs.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2qhcrqdhq.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2nqlcumjf.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2swskybgy.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2rcxxadbz.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2lrpattis.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2edkxzqor.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2ytcjrcky.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2iysqgmqn.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2jnupsxql.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2gmmnosyk.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2fvqdesax.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2orugcmso.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2xefcoqzo.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2mgsrwsiu.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2lzidmkpu.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2zdxmbupt.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2qaokrfei.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2utxnvaor.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2kqyforjw.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2ktyqrvbv.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2cbvdclnn.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2pomupenx.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2ggnkjrjq.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2onahfuug.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2zoheybax.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2zghfgghp.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ujwheyxu.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2ogmewggx.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2qbsggdnv.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2cmrwkpug.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2tladrwsq.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2wpbgprdf.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2piodspih.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2fcemkddj.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2exxuzgud.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2pkxdzpnl.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2cqacxtch.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2ztjxhbav.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2ljjkbzmr.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2rmdiapew.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2mypcaiaj.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2eecdqabg.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2pzcgejgr.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2paiztmmo.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2lvzdgpcc.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2frwwgbqw.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2ffrrfyqc.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2aqgiujnb.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2udceiebp.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2qqgudmdl.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2jzfcwfdo.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2jkzezmlu.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2fihtzkao.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2svavwuhf.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2wofvjxog.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2yuporlyx.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2xklkkjrs.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2biiwgxwy.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2tbnawucz.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2gjgenurq.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2kmqwxlnx.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2xipovqjd.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2vdscmvqa.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2vhccqofs.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2dprwjsqv.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2tfutatyw.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2dzexrsqo.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2yeutfbyi.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2nrhjzxmm.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2vttsupql.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2kmffesab.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2ceqqycup.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2jvgykrlr.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2cwlqeayx.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2alikbczk.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2hufjbilt.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2fmiqlzqm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wipywwim.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2hdgpkrvv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2utvcmqhr.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2vwoejpuf.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2vdzoelmp.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2heckddta.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2nzyhtfof.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2lgtewcss.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2qywbtzgq.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2swrijtey.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2ynuxftbb.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2kqfkaaum.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2ivsvwsud.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2otkvuifk.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2wzzbabus.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2qawfpyww.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2aycmfzjz.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2dhdshyod.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2oczpovgz.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2sglvtpqb.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2rmauliwp.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2magbrbpn.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2qlfjbwyl.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2ikgdvyce.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2inbqyhtd.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2xwyliwoh.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2fimzalbk.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2vmjwqllp.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2ajtjjsfg.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2bavdggsl.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2kqdoggof.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2djeznose.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2doirpzns.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2dskkmjla.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2jhtzskun.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2fikslynt.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2rpsvelmj.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2olvlubqf.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ilbzrnun.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2cbqhuqqk.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2xwtgctkh.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2gwmsrnrc.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2yfvelluw.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2yijsjtix.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2ypqcnupu.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2gyhixogl.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2tredrvdr.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2dgceegkf.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2dtkrmjss.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2khpahsyn.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2ixlasvpf.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2xirtfeji.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2fbttlcnn.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2ovyrniej.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2eetbmohm.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2cuoszlil.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2zyaooygv.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2pufacpsd.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2nuesfzvz.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2omphbreo.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2yifjowuk.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2xhaftvrt.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2gfbgkuau.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2foppufgd.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2albadgop.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2wgmwusby.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2brwlislt.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2yczjwazs.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2vvkrfvaw.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2xwtfsphm.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2fojzckrv.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2mdbkmkma.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2llryhmcp.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2piqbfnee.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2ouaoksvr.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2jomylpln.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2olfuprzl.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2vgwwwlgx.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2mnpdxxek.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2qdryhtzb.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2pxdgvbso.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2icullvwv.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2pkvtjytr.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2jfejhsdz.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2qwpjijbt.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2rdsxvjwd.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2aadakdgj.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2ztrxdtet.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2jozxfwjx.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2xnnabosj.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2jkoybldx.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2cbkivhbh.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2ypvsisrs.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2lenlkzkb.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2jebfjiyg.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2zdyoqzfg.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2sgbaczyp.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2cxmquloq.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2putckoqq.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2eewmujwf.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2jlqsrheh.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2bkznawzn.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2wfpvgzte.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2rruhnlbb.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2jqcxubct.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2lgitvhwx.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2niiewoss.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2bcllwyyt.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2fqecgatg.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2eoiiljzg.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2agyefdrk.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2hgryzrbu.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2lhsabyds.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2dcyxszsu.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2oyuumyac.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ueyqokwo.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2zfmgydhp.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2rhalsrre.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2bavsijik.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2ejkatcos.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2gvjyryyo.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2auepavgo.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2wxisgivb.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2zkknbfbb.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2okdthrfv.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2ldoaobdb.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2klfhfpob.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2tduejrzl.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2kopqjjka.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2drxfvkeu.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2swgmldxj.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2eyubbyou.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2apwrcffj.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2acpfesgs.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2tfakceae.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2pjzuntcg.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2perrihnz.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2tcgeivzy.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2nqmvfput.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2zzvvobaw.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2mrrqhjzx.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2ylwbkepm.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2rkqymvlw.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2drjkdosh.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2kgsyuvme.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2trfmogyf.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2blafeosg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ebgsrufi.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2mhdroejd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qkmlrwkv.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2qwvfnitm.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2mpgnbcro.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2smuobrpc.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2ybajushh.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2daltyytt.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2ybpzrraq.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2mtkqaklt.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2njodfidq.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2vkhofioi.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2mdarbkxh.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2fwbjxbgw.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2xhjrehos.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2jzdkoook.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2gpldfqpr.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2taivdfur.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2obwxsnei.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2rofkrdkl.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2cpqazmmj.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2tuwtones.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2yirnnioj.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2uxptrosy.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2qjjtxiqn.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2nrbahvfn.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2hqykjmzc.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2mkukdwle.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2uybswjzf.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2uawsprcf.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2fcshemxr.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2ppyyqjje.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ipzbpuxr.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2kakqqumz.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2bxmvlant.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2csmoljep.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2mspzsspy.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2grvjfyyq.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2grywewfj.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2slmtsjgw.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2vhheuzeq.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2uxuoxjjp.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2kicdxxli.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2bdzjfinj.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2lhfknify.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2mxttamzs.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2rssgianu.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2hpvzkdvu.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2xnsphnnt.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2qjvkdsqy.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2jkpfefsi.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2woijwdgg.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2lzkwpyzx.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2xirazwqc.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2miagibcd.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2dtrjkbke.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2nwullske.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2ryvahhxx.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2dgtywmus.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2eylcnbyh.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2flulqvid.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2ttdyrapa.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2tcrymiuo.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2pqxdbbde.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2koaagldh.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2pkbzfimu.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2jrfvyjts.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2scquxlhx.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2eelpicoq.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2tguzmiet.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2ymalqlws.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2zsfcbakm.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2hnqqvefd.html


<!-- 参考信息 -->