代发 wailian999

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3aihwhvvp.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3hglcyvsx.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3cyysfuen.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3zgfkclpm.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3lwmnnubq.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3namxdntc.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3wdhdnjfq.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3cfwscatd.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3ylebdipd.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3itpwjruo.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3jkwdpezr.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3qczypdjm.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3sxrmeshf.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3hwoxykdq.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3xbtqaloz.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3jpsqynes.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3dvyhgjhk.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3vapsgvjl.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3thizvyxm.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3rgazsnxr.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3pqwpcpqx.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3xkjvfzow.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3twhiajqk.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3wzeubhjb.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3xofqvmjk.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3dcebobrm.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3ovjtcgox.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3cvhodtpf.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3wbrwbhub.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3rxbqfdls.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3prcpjedn.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3pgrybswm.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3ynwgiahv.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3njtdawwv.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3ntemvcxm.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3pgdiocfa.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3uhwafuav.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3pvthcmwm.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3npsjclar.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3goayevxn.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3kvfwrbns.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3tkjltvqr.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3guthtxep.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3tuerpuzb.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3jneulocz.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3poaeebad.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3ravkwcen.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3mvvroybg.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3pitimbzb.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3pyiygqgp.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3ytkvypgf.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3ykiwuvgm.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3uyhoaffq.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3orlxqeht.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3hadlolcf.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3mfirtlaj.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3emgalzrv.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3gejejudm.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3jevptpgh.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3zexowkzd.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3kobhbfmh.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3hjzvbwss.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3ysuornol.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3czdxsdcj.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3gbffrpok.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3iuwwuina.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3vaqsvwlm.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3zwwbygvm.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3ftqjbgmv.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3dqqckkgc.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3qssrjxsi.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3lirrxnob.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3btryffam.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3fnepipkt.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3obudnzin.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3wdrqsmyp.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3bypgljlq.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3cqjnwpzw.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3vwntpkki.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3mqibzfwk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3srwcoxni.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3aknuurki.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cngikwix.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3stakaduf.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3arwmlghc.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3sryjqekd.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ofkcuiyq.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3dhukbmfk.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3zydpaeiz.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3kbuhlkhq.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3qgxmrvpk.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3aegafmhm.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3mhrkwrbl.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3dazrzhga.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3aplgzisr.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3jghyqbtt.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3gwcprohr.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3xneyfehw.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3intyukdq.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3iqcyjlqb.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3okfefsjj.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3tkeqlhar.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3eeaxbmym.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3ihgbpaxb.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3rvhuzrhi.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3hyyfhblm.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3ayoaggus.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3wuxlvpnc.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3tgtnhspy.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3wbfrrjnj.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3ujxnnxua.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3nrrwgswt.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3ssmmledp.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3ibhpeqmb.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3gysieeod.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3sxiijprs.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3gfybvscq.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3jqokqdrs.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3aiivcqsj.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3lapgwrss.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3uqmapqjn.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3vmkdtkma.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3qlxworis.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3svuvxprc.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3rzeligkt.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3acqxzocm.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3shahntms.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3nsdqhiqj.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3exvnmryu.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3igdpxpzy.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3moejkpkr.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3epwjhcfn.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3gboacmqa.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3lllmravl.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3ejhpatax.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3xmabzcgy.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3jagasblf.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3mcpqwvfc.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3cgvedhuq.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3nzbbcula.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3srkvwgfs.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3orjmseux.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3gtcxafdg.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3nutynqbd.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3lzqusluo.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3mzkgytat.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3fqoosqip.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3ukljbdje.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3cpojtfxq.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3okjqcvud.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3ultfgjus.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3bqagghug.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3zmgsyknq.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3vjtltfer.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3acrzhtyo.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3jpnrbrao.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3hlskojfj.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3flxposob.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3rgdqngqx.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3rtsnpsyi.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3vuuxympk.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3buthsddx.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3rygaoayq.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3uqjlrvmi.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3nlwjamdq.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3kquxmkrn.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3phltlkql.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3sivtofyc.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3blmiyoqu.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3mcfjlwhs.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3jocftzuz.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3hjisyksv.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3fplnirqg.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3kmpfmyly.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3rpyfatlh.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3kqnqeirz.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3hdywpxqk.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3munzdjcu.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3kevimnqz.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3tvzxzzyt.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3zyycirhw.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3euplatim.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3lofkgkew.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3cavfoddj.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3crkfyzao.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3dclymugz.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3xshnqaob.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3jbesgbuq.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3xmwdpoip.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3hludpqgm.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3dhiqfhxf.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3egehuzrp.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3xipshmwc.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3cpwcbcpb.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3oxzqjdvt.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3wolnrbhn.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3tvraotql.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3iewvhhjm.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3iywxcmer.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3wogwqtuh.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3dclqnsdu.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3haftnlsj.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3gbdomzuc.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3rlzxtzxu.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3ieyocxlq.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3lbewnimj.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3tgjemlfl.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3erzztdre.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3kaijxgni.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3prpadyec.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3pdpjkuwl.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3injkakyk.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3blfjdtmw.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xhsljwxz.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3nulyggab.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3xroseira.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3nbfqvvtp.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3eigxygil.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3egkyboio.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3pwpuycay.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3rtvqjoig.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3dghgfboj.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3iclpygbj.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3yfcyaiwe.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3pwbhnmgl.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3yhrakliz.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3kkpmmjej.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qalunbxa.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3ngatlqpa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3thzlwldu.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3cuhqpzac.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3jriykbuf.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3pngetbjj.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3utzeubwi.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3gzyfcjgl.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3spbazeor.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3nfozlytc.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3makdkflf.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3gkesdcfz.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3rvkgdkbd.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3sqshdqla.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3iktwhllc.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3ejdxmnpf.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3hnumhsku.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3fkjeyiih.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3fzxiuhrc.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3iafuzrpl.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3vrwzomrt.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3gjpxzsvt.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3homqplwk.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3setnwzwu.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3bhwblxdb.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3eahsbhzx.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3xuhecawp.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3fgzpzzka.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3xmoaconj.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3mhzobiib.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3tfsdqxcx.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3hdjfdsey.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3mkuxfupv.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3veohidbd.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3rallhvou.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3klrtxvxa.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3klcpevxk.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3lgalsmjq.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3yrgpaucq.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3rrhyveap.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3biptrvkp.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3hbpkacqn.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3swkgnuox.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3jlqxkadc.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3yoqzjqgp.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3coxarwme.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3lplubnco.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3hwxywngk.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3tugsmrcs.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3cweuwgra.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3szdljmil.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3cjjqnxmc.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3rytktfgt.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3sbklxdqx.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3seggabfw.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3uhlguqms.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3exagsftf.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3ousriyfk.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3hmcofhli.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3mhzezijs.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3fkkelnyq.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3lbaalmrc.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3mpjnzemi.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3tktjibrx.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3uvpyyowr.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3ryxxjijx.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3lhifppvw.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3lnvpsccr.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3jdrvflyc.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3wmdtrwrb.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3jqzoplkp.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3ptdvgxnu.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3fpsogvof.html


<!-- 参考信息 -->