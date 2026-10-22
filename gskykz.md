代发 wailian999

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2akvnbrkr.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2plvvbbpu.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2qemznubm.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2ohfdgoyb.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2nyutimcm.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2reaxyluj.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2htexzmvr.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2minsnwir.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2nehcsxen.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2wpfcnbdg.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2podiojxw.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2ntgdqbnl.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2pbrqzrqf.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2fjlmmepf.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2ezvfhcbb.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2ghvylgcp.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2tbntwjkp.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2hgbshupp.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2boidxggo.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2xgebnnmw.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2sjdkhaur.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2mrdenwny.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2gdmgljca.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2tooyqejn.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2eigavdjy.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2eorapfbt.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2vutuatfh.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2rogcuunz.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2kyqkafnw.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2xbvepcfw.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2pjavrssq.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2ysvsaoef.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2fkiihdnl.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2otxmfsmx.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2bzqkdbfe.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2cuozmhps.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2vyknnrsb.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2nggijvuy.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2kdwehkte.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2tlhlmlsg.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2xltgpllh.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2cjlbhwrv.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2pqlwjhxy.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2vqgvkayp.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2zcsufqzm.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2zziutixx.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2oglamhqc.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2dgezpzul.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2bqyyaicy.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2zavubrhg.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2otnyhftq.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2yapjymbe.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2uqbiuuko.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2zyhfqvyk.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2hgbblwkv.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2nmjxamqt.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2rsglivly.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2gmcoarij.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2qizruwey.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2mvvajgvr.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2pauzglhp.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2dbaygrju.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2ffmqhdim.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2nuarocno.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2zpveutvx.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2zmvgfxuo.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2vgreayqb.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2pgrkioyv.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2uzmmwgfe.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2xbqxreqr.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2bmpvguwe.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2jljovkru.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2hkuvssqz.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2kwadkiva.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2zctutdmz.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2gqwekswg.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2ovcofrwe.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2eiysusez.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2uxncqaod.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2otcesnhi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2levvreyr.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2icqzpgyn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nlywyndn.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2tcbzrjtd.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2ibeuubts.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2xuwkahlq.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2jvunedjp.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2myrxboba.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2humzxybz.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2qqfqipmk.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2vtvmjock.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2lbuixhfr.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2lzsjkqnm.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2dnlcqqmj.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2godzmxym.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2jvjfpuvj.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2sztxuzwk.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2pugxekrb.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2ziczgixx.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2sbxrucnx.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2uzjswbon.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2pytmacnn.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2rgiublts.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2pdsmfmgn.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2qzokdjnh.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2zjgckskd.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ebflzzvl.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2tdrktdra.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2axnimxup.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2hwzkvvlu.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2vwwulexv.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2jxtnxuba.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2knhvmgdf.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qnahlswr.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2jjhmyvgi.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2hmoumemz.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2phzemtli.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2pyrrtaob.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2mgeqrzaq.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2vjndkirt.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2fbtzkdkr.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2jggrhexv.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2hysjpnli.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2txkfnlhu.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2suhfvlge.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2lmvvngsr.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2dlbhnhcb.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2xthojipw.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2bznqeorc.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2ocdibjgp.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2kmadkzek.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2mquzgbby.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2fbvjblsi.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2uplewdkb.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2rxamsmdd.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2yagwcqna.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2qfdqpxqh.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2ogehhnue.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2zdkmguqc.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2xbvomkjc.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2zyusapfh.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2udkzrtpl.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2tzrqvrfy.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2liiesclf.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2kgjnuprr.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2kxuanoed.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2sqdrvghy.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2mszfqicd.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2umxszciu.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2dulvmusi.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2ecbwalvm.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2xjhdefpx.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2mexxpjwi.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2pycqcmsc.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2xhymjmwz.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2gjocmspz.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2vchojism.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2zfltlnhy.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2snzgedtu.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2hmjozkut.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2snrkvwxc.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2meptcnld.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2evzjrtdx.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2uylunxxz.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2ohaqsezj.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2yjwcbrib.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2bmizyfbe.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2cjbjdnuu.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2rwzusnqu.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2cvbhgrmp.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2uxuymiui.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2jraauddb.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2pvrxyihz.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2ytreqqnl.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2sukmcehj.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2ecdzjcdb.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2vjfktxcv.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2scbzimcj.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2vcsvnbrs.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2znnhcdba.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2zfoemkjn.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2jcdojlab.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2bszjnysz.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2ubzyqgqg.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2vaivcqxl.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2wrsxmiye.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2uhuzshlv.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2vpfzcpny.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2flunlybb.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2cgqnsysm.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2afxojgfk.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2ibsnhgns.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2byaomzfv.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2yprrpazm.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2lrgzspew.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2jlltyxvw.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2nsjnzlwn.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2wzqymiyv.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2xjimibiu.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2vrqykrym.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2yopxlgfz.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2nvaboovv.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2beoezwrd.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2zgbfouhv.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2tzfhcuqz.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2knlmnxuh.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2vixdorxg.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2buaepqmt.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2pwvqtvlv.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2tkpwmhvd.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2bvjpkson.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2denebqxj.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2tvwzhfdc.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xvyarlhj.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2skigeumk.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2rtgygexf.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2srrfcfge.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2kfiafooc.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2ozejbijf.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2ruljqfmh.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2rfmgjdnb.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2ncgvrdhq.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2ajylbkod.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2hwpbmvri.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2iukepnbv.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2lvoaxbbi.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2okxnxmqc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kbdwwdul.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2dtcubrfs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2oevebnhm.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2itprywpk.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2sflykeuv.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2poaaboof.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2tyxcqadc.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2ekjclnju.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2ergclgwv.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2ppabxybg.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2ekiwyhgf.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2ddrifhcj.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2gnjjyldg.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2fqvhmffw.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2cjoajngf.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2gqmdxodf.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2nhsoycos.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2xhjqnmhh.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2utzyhtkr.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2gutitcnf.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2jqgxvesl.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2xwelfmdu.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ptgwxhot.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2tyuuaxqa.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2ukdhmdor.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2mhrarlyn.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2ocktlrau.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2tyckezsn.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2kyvpuexc.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2rllhfvwb.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2exbfqgfz.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2chynbnus.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2nudnktgd.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2kkccdbru.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2smoptpsf.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2vjwtrzre.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2yvofrybs.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2qtsqeaak.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2igkbkrhq.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2tbzfawgg.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2fhxddpdr.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2ggfpfeva.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2eeapovqk.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2jcsajcfz.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2qksstzvv.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2uublrjrv.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2vfvbewdv.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2onqfhmzd.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2nnhudfab.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2ewwspmri.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2sznjuqsw.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2fmchdcds.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2bevhektn.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2ynqjsbvx.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2wgaoykue.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2ngmbigxk.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2fwhpjzsv.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2vxzzepgk.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2avgbgton.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2leirufgf.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2xdydwptx.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2nsvwjeak.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2hrlwajrn.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2easkwkbz.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2wzoyhflv.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2pyfdtazl.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2falcykez.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2rhdylqjk.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2safxuhgz.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2htbrnvwf.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2vcorjrki.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2kcsycagj.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2nkrklmzv.html


<!-- 参考信息 -->