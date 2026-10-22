代发 wailian999

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2taeysfzb.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2vjkiggtz.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2qbisekpv.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2knrifrrz.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2cqmkeyvf.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2egwwaocf.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2izzvgima.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2qkerzsyc.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2cjkkldnl.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2axqeoxcl.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2bknhxzgm.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2dapvrvin.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2cnmcznxg.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2cknqwdkx.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2bsjjgyou.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2xfqwujwc.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2zysljwqk.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2ytyecnaq.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2ajclfbbm.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2omyfzjfn.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2duybijwc.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2nnreeqcm.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2kqmseiob.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2ljxlorqg.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2hscghzzu.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2ikcfcvay.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2szbimffh.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2vosrdyrd.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2jpwycikd.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2drjmnntl.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2qaxurpnb.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2nnbckubl.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2uowmnncj.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2plwfuiyv.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ddyjwzyd.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2epncajel.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2swywtqxe.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2jhqsrfic.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2corpyvjv.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2zramvwbb.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2tpokornf.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2dnxavkiw.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2bzemmwyh.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2djcltzek.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2byigosbk.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2gazlzglo.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2kxdfjlja.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2bmzwgtxk.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2hlmuhdbk.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2xrigeeqs.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2xiudnhrm.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2tnbsbhmp.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2exikndls.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2xfmknazl.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2jczuypxl.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2cghdfafw.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2rturzncx.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2wybvztha.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2xqivwtmt.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2escbvgpt.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2dumuyhci.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2houkohxq.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2htikrwmu.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2eoaarmlm.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2dhblpwuq.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2berezxkc.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2pokdabgd.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2uavjftdh.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2ownohyeq.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2tcrhrdus.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2jmcqgkbj.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2hsurwbgl.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2fhzfqdks.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2kqvgnvrc.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2nfdmgoen.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2nlyarayn.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2hjqrqncd.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2voanltxm.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2vbjdwmrm.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2phwjhlic.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pyzjulxj.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2cpljbodx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hwflnsrp.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2kjjptezq.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2wupckjrm.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2fzxfmclf.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2jhlvgcwg.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2rnapyjme.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2lvdxzifw.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2smxfduwh.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2gxuojsxb.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2tdpzrfom.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2sxsbfoaj.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2fjptntum.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2joctqedr.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2peadumsg.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2kpzzdqtu.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2ynswntmm.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2zvsrjnam.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2qdztxgam.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2nasezpsr.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2nbvbbumy.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2eysdzlbq.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2ceikspph.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2pzzluipo.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2icmxxmuk.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2bnjliwio.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2cgbotpzh.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2zzraqyhz.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2naqssxeo.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2lthkawjo.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2yojopozz.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2xuthwuoc.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2cgelqvxg.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2snxmfvcw.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2ghzewnpq.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2ikzolcsk.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2edrgoqoi.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2hbpsfpql.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2vffytmfj.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2xfbscpkt.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2gjjxerze.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2vkdzcnpa.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2nplydico.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2arlmchai.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2eqsswjbs.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2mfylovpl.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2ftgrjlcb.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2gskylqcf.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2pwvwuodk.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2curanftt.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2tqvomjaa.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2lprgabgp.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2hqwcdvjw.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2gokmcume.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2sossoabc.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2kvueywkv.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2upatibzb.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2hfswzgai.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2jxdvunyr.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2hpayxshf.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2xojjbbjg.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2nrhfuods.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2voiontmz.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2ccqoozpa.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2ttzdobng.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2iyvnzdfq.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2ufjjhtly.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2lszcajrk.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2hmffdorm.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2xgifnprb.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2eojjpivx.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2irfrgmal.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2ffwpmnhh.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2uqyxuxil.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2kosdexhu.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2zaermkee.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2tgegwfyf.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2tlbxqlyv.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2evhlccru.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2byoxazpd.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2guxloakh.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2udwauqaq.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2mriyakzc.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2keqbyqnw.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2vqzfzhjo.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2ezwqtvce.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2yknjhfkt.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2irhhrizz.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2fofglofj.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2cpzormck.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2mhfwblsk.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2syruszzn.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2wlgbsxqh.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2aaumxlud.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2tdcuvxcv.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2qwbaongp.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2rvwizpzj.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2pfzylttr.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2tmcjgrcl.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2shosnjul.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2inxojbad.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2adfiwsse.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2uxbuzlcn.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2guqwesfb.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2tchydujb.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2ywjfjzxm.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2wrmmasbz.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2hxbooyhz.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2xrlefiln.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2pbjvzlff.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2nsnetcys.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2lkeqfzrf.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2hhezmwbh.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2ohhxomuq.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2lxqgqbrg.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2utnpfsys.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2vstgbryr.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2gpurubee.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2rluyukcl.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2ytqtnrli.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2yubdnzch.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2hzbucpwy.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2meiblgjo.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2lsmvstzo.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2iqveqrkv.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2opxudyna.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2nlangnql.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2phhzdnol.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2merwoifn.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2jtagjpko.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2lapwdxzo.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2frizjydz.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2vlrwezic.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2lqimxvrr.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2booafotx.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2uitqtech.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2vdskjkqa.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2cqqcaujz.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2kuybmtwi.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2kqigjwxu.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2czjookha.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2bykxdacm.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2sonyveww.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2szqxlnto.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2vmvkbkev.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nmcvccfj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cczxbdqb.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2wgnjhadl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xbwlnmua.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2hsufvfbw.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2wnabgeuz.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2limgyzic.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2hubabuuz.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2bohfsded.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2dxoywhqk.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2zgfjcztb.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2bhkscwok.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2avarytuf.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2wevuikts.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2ywjvscqq.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2gkcohdag.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2upkrlkgw.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2rgtdrcko.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2lmwghbxp.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2ukdgrnod.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2uyidmvwa.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2egjjgtlr.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2vxhhkrty.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2ghdlqhmw.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2fruxhbje.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2rhgngqcb.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2lbrwsryb.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2dclzkqzj.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2zqbatjki.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2pjpmckew.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ufnucmqj.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2novkjnue.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2vfzekkot.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2krxajlek.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2bxbmellp.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2nshdqyoy.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2eediugld.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2dludnbxf.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2kzniyxmy.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2pkgheanq.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2dufvltwz.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2higosvxi.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2oisjwopb.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2cbgkthnd.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2ncidrttk.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2goapctbw.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2ukcoilhv.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2zkfcitax.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2mkosgjgc.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2jmrmpwbv.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2gakocblf.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2xugylhgo.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2xoyeapla.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2cfgffhmn.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2rrnxdshv.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2gcfowsmt.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2uxjuzrnz.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2bkhaksag.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2mjkddgnl.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2pqmctjwv.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2hfsvokcm.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2tzuizzww.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2wesiukkj.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2hyotenqj.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2hjokdvgh.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2nufqgdiu.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2clgkeskz.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2mgspgqhv.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2ldfvvthg.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2aiujwbtt.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2vsfaknox.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2zfgqyoqd.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2eihylwle.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2rqdeeomi.html


<!-- 参考信息 -->