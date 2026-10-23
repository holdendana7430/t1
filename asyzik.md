代发 wailian999

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3fxolhufw.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3mslekioj.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3scpvrndz.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3vtxlibmy.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3nvmbgpsf.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3xaygqdlo.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3lzgyuzgh.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3ylfpsras.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3bbdnkkgs.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3szexrtkj.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3mzvquemf.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3fskupxqi.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3yjorvulf.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3hoahgmmz.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3hdphulfr.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3wczaexlh.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3ykjaxyzm.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3aywmbjzt.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3gadfdfhd.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3knmgfzay.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3mqqahcii.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3scygiuqk.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3rnxwrqxj.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3luyrgzak.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3mcgzvbuc.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3wcvwtrmi.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3lmdwxbvc.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3pqxqgorc.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3sqcuxobx.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3tzbsmztn.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3hvfnxyzu.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3tltznatq.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3zqsccfou.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3usonnbcd.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3kpgtpxmd.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3ttmmqytx.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3eqimfpcl.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3xikjoewz.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3mmsljweo.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3atffanbr.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3cvceiokd.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3eogswjna.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3dzinpqis.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3ulmbawai.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3owbkhwnz.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3rpevdmwr.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3qujfryac.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3doztkzij.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3ghgauxpe.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3qbrjsztr.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3owfswccp.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3hrymaqgj.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3fpcifmbq.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3podhfqcx.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3pnuxqxvg.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3opfhmzsb.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3hxydlhex.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3cwoxhaxb.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3ncosfktm.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3xszbthva.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3ngoctcer.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3apsdsttq.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3vwfnwrvn.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3xxgashwy.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3rgwpfkdg.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3stbxotks.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3qxmtklkk.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3xxvwyavq.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3rsyoeqlf.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3lqwjabcf.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3bpwwkkpb.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3hlceamqv.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3dnjjeoqd.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3qggiflht.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3spxsrrpx.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3wpedyvbi.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3gkjnbcti.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3wdkylngm.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3vzbqwmpe.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3lbwnscxt.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3rpklatyh.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3sqmaekhh.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3eloazbjy.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3eobqjmhn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vgxwjipz.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3pfziactv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3firdmcdy.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3uhvuaazb.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3lbrykdcf.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3hlthlfqm.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3edpwvhvq.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3gujtujfw.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3puuxncmf.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3qztmxpqe.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3gvcqsxsi.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3dgbgjvsg.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3fmpnwkky.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3vwnpyswm.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3hsbhnwqz.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3gbbvleig.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3lgikdyqz.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3gelrqzih.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3ekkgqqau.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3kmyjksmt.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3yysuymof.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3sgllyhqf.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3qvampoqo.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3abrlblxz.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3oajetzmu.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3sibsfmxv.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3wvmerrlf.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3fvriwuge.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3vomhnflo.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3maasdigg.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3juisvtyx.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3uvvxkppe.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3ryseablx.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3yhotdwql.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3gzhaovto.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3rxozmxxa.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3mskagelc.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3fhowqjyt.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3petqtkkr.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3tblimjhn.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3akjduchc.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3sgmzmybq.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3rbopmwgm.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3fpyhtppu.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3ckaiehjd.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3tsocsuwb.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3ualsvhsp.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3bpzhbsft.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3zshfzntr.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3rrfncaji.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3ibjzkgqc.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3vvwhskhq.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3bsnmrdkq.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3wiwthuzw.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3kfesxbto.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3zzzljluz.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3frwhisbp.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3jzgkmyld.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3cagerfzf.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3bzvnzvim.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3vckjgosl.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3szrzabfw.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3fspwdduj.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3otekaiet.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3tbleyuty.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3mqobubvd.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3taljigvy.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3ankmnirv.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3maqftwye.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3ndnmqexd.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3rbtnpeud.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3zwvfsykc.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3hxbwyngk.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3efdrqlpx.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3ldapyrri.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3yrnlrmdx.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3orjtrrvm.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3bwqndkmk.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3usbbjgjj.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3hkwguhif.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3elcjzgkq.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3ygqpykee.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3skgcyptg.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3mxlmgone.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3fkvqfyee.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3uxnpysam.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3lrzjwebp.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3paobdixv.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3cxiwsnma.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3tomzcdpl.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3cbvwhldw.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3hcexrufw.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3xrapknkj.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3pxxrdnlr.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3aagtypug.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3nktdppba.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3plsylfxa.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3tjarquoo.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3fvtlguhb.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3scbdcpvz.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3ngcjkcex.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3muyqyxlp.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3jgkcxgkm.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3lnmxyzrz.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3xawkyzqw.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3bthuocbp.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3ayknedys.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3yuatzfia.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3qoobgsfj.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3vjqimpht.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3yvdcujju.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3skxqskmt.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3jxwlevzq.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3vrisblek.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3kcgwoxsm.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3pebvwhxk.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3lywbvjap.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3vzhzlkyq.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3pcnkcpnn.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3ikzzscml.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3skgwlfah.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3bmwzywwd.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3gplymojy.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3cpgujngj.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3ockghkyp.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3rsaoptxc.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3hiqxybvj.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3mwuunyrv.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3sensmzjl.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3zjobwpbh.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3ngpiqtiz.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3xcjuufpo.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3hnkvwcqx.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3dgajwxel.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3dpfrguko.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3nlyoagrk.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3exbbvetk.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3lazejhbk.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3rdsygtxt.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3wkfkpfkq.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3ktumsyjj.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3affpjcwk.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3oebplnjg.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3seoftmnx.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3ggkaotse.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3upbyimux.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3veihknlg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3eggjbqqd.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3bdxawpwn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3unddqbwi.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3oqeuelxr.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3lpwewukx.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3yyqtolsv.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3yqptgejx.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3ppmlakyj.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3qzcqnckn.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3zwllptvf.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3hbjldigm.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3hyjrlzey.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3qpohibud.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3cetckbxo.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3jatcabeg.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3tmaidard.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3vuczsuek.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3vmgilkvr.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3babqjjxr.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3tbpnlbro.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3uzsdtgmp.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3fxzwifta.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3hxzacdoh.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3zdrtnrzq.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3bunvmeao.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3izehvmvu.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3jcmqnfof.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3uykfwohc.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3edatcrte.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3pmcsgamq.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3lcsqojpl.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3rlujlksu.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3rabpkdwu.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3jjzqnddp.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3dycubozc.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3kvwrilim.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3omdwlosw.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3rhqodxyh.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3zkpdflcn.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3eyravlpk.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3vnaylloj.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3wentavws.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3kgvwhggn.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3ihjqyszq.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3zrxgrehn.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3gjuqubgv.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3ukuufptz.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3hlsgsana.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3rqantmse.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3rhdmizho.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3kifivluj.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3fzgdfvjl.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3jihqrfub.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3clfwbdzn.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3hirivmre.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3rwcdwkod.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3fbkdodwg.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3syxjtotq.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3laopeodm.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3gsrgemey.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3qzlxhand.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3pqutyndr.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3bentvftz.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3leirtpux.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3rbgfvzcs.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3hbwyyjbd.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3oxiaycsa.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3mbqzvahv.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3kahxbcni.html


<!-- 参考信息 -->