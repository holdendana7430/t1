代发 wailian999

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2bdhvspsv.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2oqewexzc.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2zjgdzozy.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2cpbuoowk.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2nmgeidlf.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2giqkhiqz.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2oxwgvurn.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2ualqklei.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2itotwrdw.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2ckqorlkh.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2ofsjnzis.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2aimlmwxe.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2dwolvnql.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2hpyipgej.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2hrmgxtgw.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2xfvqaqyl.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2repsgnmj.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2fzatggzi.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2fbhqtgav.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2thqtvwmk.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2llqqcupx.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2bmbjhbbc.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2dinekcev.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2qdamsgfj.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2nilxqits.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2ldbfcpqb.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2owpjinsp.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2dmpgsekn.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2cceznntm.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2vtepxnfk.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2viwmendz.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2encouhwd.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2gapisnss.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2gqtvbkpj.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2bqsmxgll.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2ibxnjcda.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2soggrzmw.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2nqqspcdo.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2rdqixfog.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2lubpvuub.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2jjhzgqlg.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2zsmfwsye.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2jjheymtj.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2xpqrapcj.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2poglksov.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2ujxvsttr.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2ugmkfvip.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2nmhgrgby.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2hamjrict.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2dafqnkcu.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2awijmhei.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2glxmorui.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2poycjxyn.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2kxhebkuz.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2xrenhbjz.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2buuwijyp.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2naldbqkv.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2prdjjkit.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2cwwtbyol.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2ocxqpsdy.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2solsggni.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2galeivtk.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2bnjqzdip.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2azcmlcfx.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2yddealki.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2dmujzrjh.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2bwfnfmtq.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2ugojmnsr.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2wssjfyhn.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2atvvnvba.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2yxdwjowe.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2lcchfqyf.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2zplspyyq.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2xeyymicz.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2bwfyksjj.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2cmrfzdii.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2ucegjeza.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2uomvpdgm.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2dvepszud.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2zcwfncgv.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2rkvlmclc.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2yzhlfpek.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2niomhzle.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2bjpbsqvd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2uqtkyhmx.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2mphbydzd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mdihwrui.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2qwihkjwx.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2vcgbhlst.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2dduiummf.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2muypzruv.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2lerdukqu.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2cjwfdetc.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2dknojnlr.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2weaahacx.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2cgfsjuua.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2bvdtsynh.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2besiuucc.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2ltpcuemz.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2shmbjcew.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2bgagojtv.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2oewxjtsm.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2btmqozrm.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2ynrymgme.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2ddyvhigm.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2aasqtwia.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2etdqsezi.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2agfgfcwj.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2dzgutyak.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2isbuyghw.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ppdkukth.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2nmmzaepo.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2lkgtlggk.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2xembbvec.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2gdzftvvr.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2dgwzwlpf.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2mwotlgva.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2xatkyfbw.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2jpydotnn.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2ahhvdtjc.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2putxyvtw.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2hpexnvqg.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2axrdvymh.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2lctbmwre.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2tzatelom.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2afnzgruu.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2oksilqjq.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2yjjjqyzw.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2gqfbleiz.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2pylfizvj.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2yyoqjfwo.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2ypdnzvzm.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2qomwhnhv.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2tzrztadj.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2uppwjuul.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2ziuvgmis.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2tronvxpy.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2btwkndqv.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2iydjekwb.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2rqqtmodd.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2cdgrmwkm.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2rbuksmjz.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2pkatqikj.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2isdbnmjw.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2crzribgr.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2wdrycfna.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2iztaztvr.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2zxgbiovx.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2vhpqdaow.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2iyitrorm.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2sttieirm.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2fkjdnvph.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2cuysnjdo.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2rlbnpovk.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2dftiehyx.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2hrsmhpwd.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2telmdohu.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2gcodxexq.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2vzigbapj.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2mkillgoi.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2nccjelil.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2cfhkpioi.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2ilmorddy.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2wanvjynz.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2slygaysv.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2ynaozrno.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2uonmxjii.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2nbuvesnz.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2wmaqmhsh.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2uhlbcjyu.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2ahyschnc.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2dqnxusyx.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2vihaufzg.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2znvqeebe.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2lykgnuum.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2gzhqgump.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2ugtbydwf.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2julacfkv.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2mhxwqagf.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2ukmgibkx.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2vqesizle.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2okipokho.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2frruzjvz.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2labsciod.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2jvjsonjp.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2euwlpswb.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2tacuwbns.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2tlfphqks.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2dtetvzqv.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2bdfyhzob.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2gsizmtxh.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2lrihftey.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2mqajhcwc.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2fsccozyc.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2mhnklrux.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2xwhhypou.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2laprgfpv.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2fpsdgyaq.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2nidtvyol.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2kztsftme.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2jadqmagt.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2godwwgnw.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2lorunlnx.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2damtofei.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2nmsljkyx.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2icsgatoc.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2trkfxapa.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2biyclnyc.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2wypdywyb.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2rjmjupbh.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2olgizzzj.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2ceyywzjo.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2lrlxeego.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2gvhgwnah.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2udphezmu.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2agwpcotb.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2qfatezss.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2nbazlzfd.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2htndexhe.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2qisdkurq.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2enhcphsd.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2wcpytwry.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2bkkzanxs.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2ifhwsqra.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2smtlpqat.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2oygbhukm.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2ljephjvd.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vhpywtxt.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2kylpqmpj.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2dsluickv.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jmodsuku.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dqwenkoc.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2qmboicmc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zxqjyibx.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2nwmfljij.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2fkaozmky.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2kmgjeqbh.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2uwlokahs.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2dbrzkxhz.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2vbyrrxeo.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2apmrjwnq.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2nhhcjawh.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2munlvfjl.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2oqkqxkrb.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2voljybck.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2tbhxyyfv.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2kwmneqsg.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2fwjoviwb.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2tkscvvvs.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2qhwvycya.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2idemlptf.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2ktqzpuli.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2rnvjpbtx.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2niabxadi.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2uysrsihk.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2rwmnyjtm.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2qghogcot.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2kiamcmbg.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2hwccyfqu.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2xwfklhhk.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2nuxzoiqt.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2nzdoyqlx.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2mpklnurm.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2oeydfkui.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2kcmtedrx.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2ozchzfzg.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2wgjrmmof.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2pofhzygl.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2axxowzhl.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2qzwtyqgo.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2zjwhegfl.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2xbiybtuo.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2ttsevswi.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2xwezqwwa.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2maqixtxa.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2rskkurys.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2kobnivez.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2deuzsaux.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2uglojukg.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2gwzlsydx.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2crfetesk.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2vfncidrq.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2xzmhxqlw.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2awkjiofr.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2weydpxws.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2fvwbvwzh.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2hdipbnqs.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2owxgoyal.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2axuhoqbi.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2dxpgceva.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2aalpxrjj.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2xrhpgwbm.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2jolwkoxs.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2rpnmbznt.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2slnayeic.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2edilccjd.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2uvradyrg.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2wvobatyx.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2iiowjgax.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2llvwmyjy.html


<!-- 参考信息 -->