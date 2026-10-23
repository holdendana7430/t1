代发 wailian999

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3jrxgocmm.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3faornwuu.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3itsfqqxl.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3pqwabcpm.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3bnxtceol.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3ectgclhb.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3cgybbssz.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3aijurvyw.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3fjacimcm.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3cajohrmf.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3xymxhdlf.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3quqvkhdq.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3ycjdkicl.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3jurkruos.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3plxqohox.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3qirxwxsi.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3aiogllks.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3ppnmxmxc.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3jxymcyyq.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3mbxivata.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3qewwlsuw.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3mqqtxubw.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3fvxdctzf.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3skwcazsr.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3btddnear.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3aenwhuup.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3pthiqnfo.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3tpejhibc.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3kxzhdwro.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3hilqlakn.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3wsfbtcxf.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3whliuhvf.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3nykehsgz.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3cobdfbvz.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3httivbgv.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3knuvqfwd.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3myxdwfuw.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3tnaopcyo.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3xtwwkeot.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3ahgntqvr.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3zrxesvuk.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3sthjgzxk.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3kctcklbh.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3phgugnyj.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3scltzzzx.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3zfbyddlb.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3zctyiecq.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3xbcxbtgr.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3jqlkvllh.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3khoivcma.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3iqmkxhua.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3nhcvrhae.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3kzrrwszd.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3sbuviiaa.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3dkigpfmq.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3fuzffuij.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3jmgpjtnv.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3fwhqrbzg.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3nrmhsipc.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3gujpipcg.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3syzrihsi.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3uxmwlyxj.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3mlkznohw.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3xsvzlzmu.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ddohcsfa.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3amugszwa.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3hfuzwiif.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3hlqtifub.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3lrzsajhm.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3lavfeqbr.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3rfyrehdi.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3tlyfobba.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3uzkwubvq.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3ppfnvjss.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3ktmlfghp.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3qpvbmhrz.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3kuzjvxpd.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3fqvndswe.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3viusmwms.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3nyyfolvd.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3coflmmba.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3udzxvcos.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3tlhmjydo.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3dlatwuex.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mzmqytmm.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3otfgaxmp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wpadljrn.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3bxcnfepk.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3xpqkqmfb.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3cwqhzjrg.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3jqafosuy.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3nrqdapfp.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3wvocuoyz.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3wadgedhc.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3drzeuagm.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3nkhmmtjo.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3slrqvumv.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3fszwxyys.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3knrutkmd.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3xlhnxbfn.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3siogonrn.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3fzyihetw.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3mxlrzxyr.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3mfdrklog.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3whqveqfn.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3ybwtwzwr.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3jqwkfmel.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3qlzpjtpc.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3tpeyvmhe.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3qrflfznl.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3qmnryyup.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3qnyumrpr.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3trxkdmjk.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3xlqppnsr.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3bsnlcsig.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3ksovovwz.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3fdmjgijt.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3hvmxwxed.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3yobikqjy.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3rnjxizdt.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3gbgmnioz.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3vmbygvsz.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ijukfbrg.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3jubpietz.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3dbtqmljq.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3fvephwzg.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3lyasoztd.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3ydqfnxro.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3vnbpeqyn.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3umailaiw.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3flffnjwt.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3zybytwpg.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3yocwcawz.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3euxxgtkn.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3siwewiad.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3pebjzdxd.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3dlmdafnj.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3lilmpzgl.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3dvbdgbvp.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3rbwmdtdg.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3aplaxvai.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3mxyhmrjo.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3rtnpiyok.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3hienlyhz.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3drcxmves.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3bbdjlzjg.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3gbcwbhol.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3uonenkgu.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3smhbjclm.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3ibhxjbgq.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3axflkpyg.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3yjeowvor.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3jwidwaip.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3hstyxgdd.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3wpgrddxw.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3vlyjpjmh.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3nvduivrd.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3gowtltqu.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3xkmqhabn.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3wwjwxqjm.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3vwudnqiq.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3sxctlimd.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3wgjoxbwu.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3tkzpnztk.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3hcoqtyqu.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3scikupnj.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3qdikzxaa.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3isnhqnfk.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3buaibdww.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3ahyltqth.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3ycrstcsd.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3kwxzlekc.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3wdjxqvef.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3kvnitxcr.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3fcqgyjzu.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3xaxqjgvm.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3ipotlggg.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3iqozsdsb.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3ojwcopmw.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3siivlgbp.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3zfeggift.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3hbnuayyi.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3obrvwbao.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3ojxmfanl.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3awyztrdy.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3xkgodhha.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3awrriyqn.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3kzcivrzm.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3xjkhnvcn.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3rzwsrvjn.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3fuaghgeu.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3ynrhyovz.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3efjbfwpo.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3pbidsohi.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3vmrhstxl.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3huvkcdno.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3ohqlecvo.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3bajnkrtm.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3dasymjvd.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3fnhvfflh.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3bsqdxqre.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3aepnlcxk.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3uhfzkxgg.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3dctfuuma.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3dnvscdfs.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3zbwwbhrz.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3wfounqiq.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3ycrusjvr.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3kuhlqdiv.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3jemcxevs.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3rvmahaqq.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3issrtwhk.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3uuuakdbb.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3toyqqesm.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3dblsdziz.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3rqcjdchs.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3ircjlsvv.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3llkebiai.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3wpnapekh.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3pvrirsjz.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3ehckmglv.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3ovkspaqq.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3nbxaeyvo.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3wwponpty.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3npktocjs.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3cwzynwbi.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3vobqzhks.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3evxttrfl.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3sjcsbpsh.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3uyhjuvrm.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3yvfjbhyl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xfbwykkw.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3qmrqvhjm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ecyquvvj.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3ndbvzkgd.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3gsghdhts.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3dnhntlfl.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3yewipmri.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3atnwxwvj.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3lxtbymub.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3ancobqkd.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3zbzzeafr.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3fjbgjccn.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3tciwgulz.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3aplksfof.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3kbsrzgzb.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3biohlbbm.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3xpwlaxsb.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3figxfvqd.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3zcjazbfw.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3pivaeizf.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3mcrycmqh.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3wsigdlxb.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3mmayalca.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3sjfcoivf.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3sbydiswi.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ijxzkmvt.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3jxtlsixm.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3yazsfqwm.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3fjiyctop.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3gtymvsrv.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3lzudkmsk.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3ttbpdzeh.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3ssrpegrt.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3azommsjr.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3hebgrkbr.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3bqecxrrd.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3tpyrjicb.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3xkvzwsdf.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3cjlluuab.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3akkmbzva.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3waobijky.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3omqmerbk.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3aazfkivy.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3qxzvpffb.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3kgppewpb.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3sudsokcr.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3efxaduuh.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3vopqcmkt.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3aymnneqv.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3fcvffpwz.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3rpvmsoap.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3umirsjzz.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3zgjongky.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3bcbsbcbq.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3lbabmqhc.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3heoesgrf.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3jrihudlt.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3iioizskj.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3bogzrlgc.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3zvrxavhi.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3ashiqusf.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3pgnlhhvp.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3cfvbjrmb.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3xzsghtja.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3exwtuxza.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3zcqksgxz.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3lhrppoud.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3wpluvdle.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3yjwsgjcw.html


<!-- 参考信息 -->