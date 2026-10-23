代发 wailian999

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3tgwbpcsj.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3fsouyoux.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3sqylmzdw.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3mzzmhstj.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3zvnpytpv.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3kkgdetiu.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3xhfjsdua.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3zzmjkjcw.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3edazxbzl.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3cjcfyjzl.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3sgdwljyk.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3xtxccvwm.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3nggttvjd.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3gsdlcqnb.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3nzpwrnbx.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3lmstorwf.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3etpotvwf.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3psfqlyna.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3cmdhpawp.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3ussabpos.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3wzvigizn.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3yezvbcxe.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3kecbigqa.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3kjbzaxbi.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3ewsegqfs.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3xfdzldxh.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3xxbxraag.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3gxwewvhh.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3uxiuadxd.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3jagfpobc.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3yjoxgapl.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3curgdjnb.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3sbibrhkm.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3ccdgpwpp.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3kbcqqqtm.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3lzajyroc.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3gqkeyjun.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3zoxxepxp.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3xeoznemj.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3zygkktqs.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3iredztfo.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3lrfbqzrp.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3xdkxhvkw.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3bswxduab.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3yvbxpwfz.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3waytohsw.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3wqsblwbx.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3hudwdinl.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3tzssrdkx.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3bplckqiw.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3zgxpvbak.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3nzvkxmdq.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3vmnnplaj.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3gbofrawo.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3ozwcrzfn.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3nrmcfffc.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3msdmevbi.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3anldhlpd.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3hparmdtl.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3tjgmluav.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3hlkmjril.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3vtriogzo.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3yviihjru.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3ykhxfgrp.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3hrkgkhvu.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3oxduwvtk.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3vemsrzwt.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3nyftkfdo.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3lhvhrefs.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3cifxszer.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3kybohtzj.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3hccmwlng.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3gpetqpwm.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3srpwkpjv.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3ldfxohgs.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3fouwmncs.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3xvnktsvu.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3szuqbjlv.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3mutwlzjx.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3awmfzmut.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nidvjayi.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3mxxkxbbg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kcolvsap.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3lfymzrwe.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3iycedhor.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3kksryzim.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3cmsxdijg.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3vuyqvrql.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3tqwdarpy.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3cfoxyhgg.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3ldnmygqb.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3rdkztnsx.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3xhzeohmu.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3oyprvifv.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3xjnsiobl.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3nkdgsvyz.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3fsjybjow.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3maskqslf.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3amdytemc.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3nwgyoomc.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3clmwjntm.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3liubddmq.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3uhybxhey.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3zghqyxqh.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3khqttypr.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3qbjzijsi.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3tnliotbo.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3dylijvtb.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3xkifywfw.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3nlcessdp.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3vfsvmnht.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3pklhedvw.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3axnydwuy.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fmndchnq.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3rxvqqkqv.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3zxxjvlzt.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3bohkkkzh.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3yfljwqob.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3uiavxxgz.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3uwawkqsc.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3otqggiyy.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3bqdtwwgf.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3fuolsqkb.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3btwfmjdq.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3igahmfmn.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3dossskmt.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3nxlaubau.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3bbjyvctz.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3ovblnrag.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3vpqrkhyc.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3qgxxkild.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3hehtrxre.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3ggwpbmvs.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3avbhyaho.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3xicinjbg.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3ujumcace.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3fxpqwyvp.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3udqetzbr.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3bbcxtgno.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3kafwcldb.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3hceajqvb.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3misskmsf.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3rpvjsexy.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3emsvpfky.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3bkcidvwn.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3wcwnayrt.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3niiluznl.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3phqgmjkx.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3ybkfhtzb.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3gqiofvja.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3chflpooz.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3nnbwgwxx.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3uuynacli.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3zgsrxawm.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3jyougxim.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3bvukkodf.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3yawhjlpl.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3qygzrmgs.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3odzxzbfj.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3wolztrqb.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3lzhndcfh.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3fzfmowdh.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3rchimisb.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3xdtljysb.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3dijcbfau.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3ppexskdb.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3emjdxocm.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3gqhliams.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3mjpesfwn.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3llhahgbb.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3bpszvxkq.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3kbfgnscj.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3yluefjkz.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3tlqssfni.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3fipcaoun.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3kygopzue.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3zcezditw.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3yggmetjp.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3xourynuy.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3utkghfxw.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3fzngbvxd.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3wuryjibo.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3yvxrguuq.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3xllzciub.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3jtoycmud.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3nfwhujsf.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3rhzhkmev.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3xuinfdne.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3dbfivsiq.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3yjxcrebe.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3qedwmown.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3ocdhguxa.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3msdpkdly.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3eutglfdm.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3dxewstym.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3gjftfzfn.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3asieyvpk.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3rldyutpi.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3xkfjscie.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3ltwuhnml.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3pojzcagi.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3bvbgtsec.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3hwqwrfmt.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3yqqvzhkr.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3vrywozug.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3rguosqor.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3lgtedtfc.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3dfgreeaz.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3ndrfbici.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3qypgiehq.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3ybetojzr.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3xshxjbir.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3msugnzwg.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3yvubhecy.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3agqwhylb.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3fafmpghl.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3ytevdpyd.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3bpidrtsw.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3lyztjvad.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3jhscndfh.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3ljpklqxp.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3qrbdvdmx.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3dwzmwasm.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3pfulhgvk.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3skioauxg.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3oeerdyyi.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3ptcsgujf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3agqtdxdt.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3gqnswdik.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3svsylekn.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3mzwkgego.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3bfqmzavh.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3ajpxfrtb.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3ljruzumi.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3aovownsg.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3jwbzhaib.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3cuoqotwz.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3isszmufr.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3rrzmjtkv.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3nosuhonk.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3ycvenjcu.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3goytgxod.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3vvzfdiuv.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3xariqyve.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3emmlsxcr.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3bvhjmqyp.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3xrikpiec.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3xikrbtbi.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3lzigedyg.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3yvmfbzor.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3jejhnvrh.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3pqfrdbyi.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3ffuckcsm.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ifjgaqro.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3mzbpgzqg.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3gjdyqamn.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3hhelcqsz.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3qjfrwqwv.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3gkoelnht.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3yffvefad.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3bmhvjtel.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3cpfvyaqj.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3lxlcjssh.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3wzyuoafj.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3jwtgnzmh.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3krfqqcnw.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3zivpwnpm.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3auvmlwlw.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3lciueomp.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3xhgdsybp.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3nyyqhodz.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3bbamibzo.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3rwhyfljt.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3xgaamuqs.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3wytojpcz.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3vmntjthe.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ekhwiizd.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3hgczvrar.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3anmnmtro.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3quzdjqkw.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3bubpbwed.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3pfvllfri.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3wrfgscsy.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3eotxvspd.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3sijculpq.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3pkqvudfb.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3xiiipdqu.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3vwblcajt.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3fothxamx.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3gvvzrzjl.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3wpbnefbr.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3wovkaosl.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3yuvphsib.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3mcuuhwbr.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3rkzoicma.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3xexlhell.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3kqjdrcmw.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3jvdovwft.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3eurpqzgs.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3vxdlibfv.html


<!-- 参考信息 -->