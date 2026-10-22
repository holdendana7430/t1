代发 wailian999

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2pdrqtvpc.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2acrjpplz.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2uksylxaz.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2vpvrhuma.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2xcrfgbsc.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2dqppqjtg.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2vxnlhcvb.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2awgkpjaj.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2ohypdabv.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2netrmmqw.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2pcvjjdeq.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2ddfhcdnu.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2upsdkyra.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2dxjhgkkn.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2bhamswbn.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2spxthqhg.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2luehcxzw.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2ylcdjfxx.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2bgxzboxo.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2bzbebopl.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2pauognml.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2ggrccqst.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2qcrmnxvy.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2tvakozdh.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2hfsijuah.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2mljpjjpq.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2kulxbqru.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2sgekigen.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2ebilucxw.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2gnfkulyj.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2nsavgjpo.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2fsjxaewj.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2qcqbojms.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2cjjfhlsq.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2tdmtmckh.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2dpocjhjy.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2mwpjdkgq.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2vgsxhprm.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2pyvvxkzr.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2kpbvkfzd.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2zmnzcyeo.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2sglpvtvp.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2djrsubwu.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2bpebikvx.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2cnzuxsao.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2cbcyfyez.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2oxcmhozg.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2ijikwymm.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2vfzttqrk.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2cxhgaohk.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2flcrhmsf.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2ckcwnhag.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2lzlnobiz.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2bcjicjtq.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2hcwcllku.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2jzhijykp.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2xzzcbhwc.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2brhoqhpe.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2cpyulslw.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2oruqnvgn.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2hlkmtdbr.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2lbwzunea.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2mqjvpdwq.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2yfwpeuny.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2yfbypgql.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2nphjiamg.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2crrycytq.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2vsqrxvwt.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2nvhzeljr.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2cxamxudn.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2drzxozio.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2gbvwwgzq.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2tgqdpvdi.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2jvukfvto.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2fussjjgk.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2ugpgzocz.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2yrpdklwi.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2gwttpwxa.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2mrnccdbw.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2qcgumajw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2iozjzsze.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2fjsneili.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ijyxjcqb.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2twavwwlq.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2ptknhdgh.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2drycjmnc.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2juolantk.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2hmwhofsx.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2cbjkktvp.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2twsabklv.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2bzmwxcwu.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2vygzrmya.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2fzlzctrv.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2pvecmaxe.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2qdknugve.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2fonejvsz.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2xptvsnbr.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2ippjiryo.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2ylivpnmf.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2sqlcrule.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2ijthqkui.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2zwclfimf.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2olijcbwr.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2aemdyuzy.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2iqvwldav.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2utrmmzzt.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2febydrhn.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2pxyohcss.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2ebgafqah.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2qmunlnbo.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2pdpeznxz.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2rnmtppiu.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2wafgrukb.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2jjkytcqs.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2bizvcayw.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2omafcvmf.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2lagvqeks.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2rnkquvau.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2axnxhbdd.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2nzjcxujs.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2cuiflzgo.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2bjeqxsxj.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2qreohwmd.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2jhpyxgnl.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2xexaomjy.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2yrghwwod.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2wgidogah.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2ucscntri.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2qaxhklvj.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2jsyiutzd.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2niqxqqky.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2yzximgje.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2vqcjipfu.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2lqhqwfuu.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2pgbyomos.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2srbhmvrq.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2vsqtzuyc.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2omnxckbb.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2chwqmviw.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2sityeole.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2wxgacotj.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2iwylqylz.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2brkpgfia.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2trizvxdg.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2nqnurpms.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2cwikydcn.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2raxosxiu.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2bpnzbcvv.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2luyjnqkh.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2lvdnrxcm.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2dqxmmyee.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2ktslswvs.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2foikfzdq.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2eakdkicr.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2qxpntukx.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2iiberrbr.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2xefltcct.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2xdrkozig.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2nefbifab.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2bgozkbrl.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2wblfmztu.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2bfuvbgzk.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2uyahqcyu.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2nokvvzrd.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2zasltybv.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2ekjjttgi.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2xhhoubpd.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2ehlcvmzf.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2ehcjfsvn.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2muhexpcq.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2gtawwenj.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2eribvyhk.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2zugvrhge.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2cnfetkqy.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2vxllusmn.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2hfkbwdht.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2fgtilint.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2tnovdnri.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2rczqlrrw.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2rltsqart.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2euozuoda.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2nypqdtvr.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2pxieverh.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2zgoyataw.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2vpzczgjb.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2plhvueaw.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2mzatquoi.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2zdalddye.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2qmwfhiow.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2zcazkhfs.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2geotgvmg.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2dbxktdgc.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2fotcejsf.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2bvazjyyu.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2kpamgifx.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2bfavjsrv.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2yrtuosyk.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2hnzwzzgg.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2kmfzycig.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2kngseiza.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2yrqdeays.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2mphhcbpb.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2qtjvqevw.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2fhqgwspt.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2hcqzeiid.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2nwqwjbgl.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2otweiwwi.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2ybmtyprf.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2zrpvbymz.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2cqqereur.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2bljwvddo.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2wjwqhaet.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mgfkkhjp.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2yjxmtllr.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2cdtmsvlp.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2utrqcoft.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2eaofkdwe.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2nyeqpusl.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2ripseybv.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2xfcvjjph.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2tunwyqjg.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2rkoupztg.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2njxxrusf.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2ikgeuemo.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2xnxnefdg.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2erofauly.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2sxpaujrb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ztcdmvng.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2crvhgfbe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ywuemhai.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2fmqcdmhf.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2jrwmlyiu.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2rppfflyh.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2nwlwckzr.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2dvunsqok.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2kyecpxak.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2akdkjgui.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2slbscbal.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2rssmaars.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2mheexrpn.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2yzyxwkdw.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2pzxqitxi.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2kwonfflv.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2dndevztu.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2welvpifc.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2udyosfin.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2wxmsegvt.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2tbylhfmh.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2zyakeyrc.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2lhehseuq.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2altniqft.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2ahdpbrpz.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2sffcgqlz.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2dmrkwkrj.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2khxamosw.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2fgqzhatw.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2sopoyqxg.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2ithmprtw.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2blnmhqfu.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2xqpfchou.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2ozbbbtrj.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2savgzcsm.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2vynvwiyq.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2spygscyf.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2nuhebksj.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2saatqldk.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2lrlgvywo.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2aihjvfzy.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2bgcdgwls.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2wxwlfhbd.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2snrmlsxu.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2jjzdvvho.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2xgpslvoc.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2ettbfdap.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2vtgcwucr.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2ptpbicfc.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2dgbhbxps.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2cbnozalb.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2txreweyj.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2smrexiep.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2eqipvqdn.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2wwovussu.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2ioonoknu.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2mrwrxpma.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2dczdulav.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2pvmgfrar.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2stkimjfu.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2vyoixmpc.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2yjpotydd.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2sjnnlwrb.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2fmxqjrvn.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2rokgvgsw.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2bxavpuak.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2plutyihp.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2iejcnozn.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2oksjbzsv.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2pgpsshzj.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2dtkkllij.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2mjrmajwc.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2muoogkzl.html


<!-- 参考信息 -->