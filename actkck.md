代发 wailian999

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3jgsyepkf.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3esxabalo.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3wovshufv.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3ygdxsvla.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3srvqcajq.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3dcmaiegt.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3kqsvowrh.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3vmsozsij.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3qjrpdasp.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3cfafeauz.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3iobnvujh.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3mxpxccal.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3soioqpmp.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3pkgzhpxt.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3cacolakb.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3yjyblebu.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3wltcagwn.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3nqkuiksb.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3mgcgqifo.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3kbksrpou.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3rbaraydw.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3izqawpoy.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3xqdvorog.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3rxhrknxe.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3qiodffwx.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3tfdjdmas.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3elersbus.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3laiztvdg.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3cbmluxbe.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3jcuxqejq.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3jiiazfrz.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3fongiwak.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3hcpkttfh.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3yqbgfnpq.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3wfgxdxzv.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3txvrblkw.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3qwquross.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3nmydpvzc.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3paxsucqf.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3jbphkuqr.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3auyipqgo.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3rrmakjhz.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3lgfyxpcu.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3yaemkuua.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3ghlcunqh.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3kpslraqc.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3shklqrbx.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3uefwtkpr.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3bvtljyxg.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3pzpihksn.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3xipgsiwe.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3oejaphdm.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3nacygrdg.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3rrmmexvu.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3vtdypehw.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3lwjurbqp.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3wgiyypem.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3djkimtim.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3yvnnlhdr.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3ukgfngmt.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3ihvinmxd.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3whquhpcb.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3mdmcheyo.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3aecsrkoo.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3wlpfmnls.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3pjtnrinz.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3bqkkzkqt.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3udmxlmtt.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3vezyeflb.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3sahiibdn.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3thwecyhp.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3bkxpiuoh.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3wnxwnmmy.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3ljgfosjf.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3btxpmsvg.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3bjrvdold.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3irabvnkz.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3ajjaapsz.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3ggwiyjjx.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3czurokof.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rxskjndf.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3imqzuine.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lyjvzbzc.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3qfiohshb.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3dnopiytr.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3nqsctpcn.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3mynugzhn.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3grpdnnxh.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3chuwjszo.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3awabectf.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3eyxcpdpw.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3yyvydibm.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3ppnruyum.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3xxumflva.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3sbhkjtul.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3jppupcum.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3mrbsktur.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3qkkfgksy.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3donbkfxf.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3hijhwhfj.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3fmvhfoeq.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3ohkjgrge.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3fsqmouim.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3opzryjgz.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3ajmvvrvx.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3moqoxklf.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3goviczyf.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3eggnemad.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3kqsqpsvj.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3ezkkodln.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3btkiutwf.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3txqwwnuq.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3jhqninyr.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rxvouypx.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3hmnabibn.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3fglkoftk.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3euyrupab.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3dbyocdin.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3feeylptl.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3hxueengj.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3cncgkmlj.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3beyymtgq.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3stkuiycy.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3rnibrtnb.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3chvqqvfw.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3daednxwb.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3sryivnmr.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3ormhqxgo.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3pmjyslxq.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3uydlpehv.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3udfgxhfl.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3dwztdzxw.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3aqljhxrn.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3aeqjnpwr.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3vnuuemmb.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3xapapexo.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3yhnrowde.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3ceoyjzkv.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3gzzhtkhp.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3cuywhtso.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3fblhmlmn.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3oocgubqb.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3yzailzyj.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3prhqkmiu.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3dwryjzhm.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3ohdkrbku.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3lspowzke.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3doefiwmr.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3xixauklg.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3wfutfevc.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3poxsnkjt.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3dimlipyh.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3iomzawgr.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3unlqunsn.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3ljuakqad.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3qzrakpdb.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3iwwsrxhk.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3vyajvpoi.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3jqceywpz.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3ibqdldux.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3uiepuyze.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3caeljbbm.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3aptcmuzx.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3cpejtktd.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3kjomlpun.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3asqjwvzc.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3rktamcoq.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3jfwjymbi.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3ywtaosus.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3dkxiwqup.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3hfeothis.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3yssqezqw.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3onrnfjom.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3ubbxydmr.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3kozujqlv.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3djizuphm.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3euphvkyo.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3vqyabspo.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3wpksfbvm.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3gcvbrxoj.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3fwceegmt.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3jadzlvmj.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3rynkzgdf.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3borlfegt.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3rszxazuu.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3knkddhnf.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3liigvwnx.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3cmbronzo.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3ooiracut.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3cbrinaqf.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3npqwelrc.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3enkqfkgm.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3hqlntgcv.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3fwzshxqr.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3vhvbbrvv.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3hjjymfhl.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3sylmglbc.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3uxuuoxdj.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3wsajrggu.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3jzbhmbgc.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3lrcllfei.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3tyartphj.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3pugkdmad.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3kumcpwup.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3bcmbmdpv.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3rtihyvmi.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3yxevybjm.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3csaiagxm.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3ikpyevee.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3bkovqlws.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3nduonbau.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3fvvotuoz.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zyxqupib.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xjpgourf.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3qjmjprfl.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3jboygete.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3oniteawg.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3yymwqjal.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3vixrqvdy.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3dkhtgczh.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3pkjbatxi.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3kwhozcer.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3gtexrqbx.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3dcckeayw.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3itbinsll.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3ijwcvwbk.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3sdetsoyn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qetlqopc.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3lqqwqeos.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cjpjjywz.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3cldilyxg.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3wnkbverc.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3yekqfuup.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3sjtrnpuc.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3negdklrr.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3cgwplgmq.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3plmypcfx.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3hueowbxg.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3dstzopyv.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3rvrmrzfa.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3qsanztsf.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3kazdtixl.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3crmaejdf.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3smxudrlc.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3wnisqpsx.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3qvopownb.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3orqqhtcg.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3jickcywv.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3ltsekpne.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3jzdpeuss.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3dpfkiudg.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3tgfgujsv.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3rxtymjpp.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3yuvieugy.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3hpyisbxq.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3xjilzqyb.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3bltpuwcz.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3mhjpnciy.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3cxvrdxpg.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3ezldpuud.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3lqghhcvj.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3mfuugyet.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3qbihwtyd.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3rqffwjsb.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3ileavcld.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3ivfhbkah.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3qrgeomso.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3nsxrqxkd.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3lhvtojdb.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3yhmvnwej.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3ceuxezno.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3yfbzwcwp.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3notmdbkq.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3blbuqkmt.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3jaleklmb.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3cdqslrez.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3qjxiapoh.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3bthqvwus.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3mxmcvjpu.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3iugnhzeh.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3xuiabdvq.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3bsnewyad.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3bsiaxfvt.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3umvgfirc.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3wycexrzg.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3ambefkhv.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3bixkiyda.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3dukzeqvq.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3qlykjxjw.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3dugcxjxo.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3gjhnrdbd.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3kvbkghyi.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3eyrpcmtt.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3tvhgzrdw.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3wpmxdqjo.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3fjqxucax.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3wqpcunld.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3xxhxawfh.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3dxxtnolb.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3pazxanwl.html


<!-- 参考信息 -->