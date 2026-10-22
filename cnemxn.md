代发 wailian999

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2dbgrlyvl.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2uscjqyuh.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2ocugsrox.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2esnxbowd.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2nrokqdbu.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2zwozersy.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2rthkzejf.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2ftbhbyla.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2kcshdpng.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2qkezmnve.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2pssyeehq.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2eyhipjto.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2pwhgcoms.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2ldylxipd.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2xqucrwpk.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2ktqzojzr.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2ntgbngwe.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2rvpuufcs.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2dtpvvoun.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2xqawnazh.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2vzopyazq.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2ukrzqywu.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2glowynhf.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2ropwlwwx.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2zdkobykw.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2lilzpjqf.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2rkbywpfx.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2gshnesfc.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2hhhvfmjm.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2abmjldqa.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2ovskwqkk.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2slwszhlf.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2xclbbwdh.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2zydwksoh.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2gtrwqcbq.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2ppigmexc.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2nklubyyj.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2nkhxkidm.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2lflbbwgg.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2wounovqz.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2yegnsbzl.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2gdzwfpsq.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2nicxpxbt.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2fiwvjppi.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2mvgbrlwy.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2gyuzhzjh.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2syxtlhze.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2nirwfybz.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2dhjhprrj.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2zrdezkrq.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2cpnlmxqi.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2jgdhubeu.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2xwrgdsyi.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2foiywaqw.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2tszhwtvr.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2oyhblnxt.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2clnlmknx.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2rjxqoysy.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2llszexrj.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2rtxvgjwx.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ikkajynl.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2kybuevfh.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2etwggspa.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2lpuzbusu.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2wdeqwfve.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2dcrscwkt.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2whbvgwsm.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2uwewmrty.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2eovgmjhf.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2wcsedgbw.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2quupefuz.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2hdmoskpy.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2uejnyllp.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2zoolupmu.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2akanvqvq.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2zkmofhkf.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2oqfxzjew.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2ghoixibv.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2bseiwfnm.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2zbllldqd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kxqbzvak.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2lgieocuh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bzutvxtq.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2liqlqqjc.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2yknyualx.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ervffegy.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2bqxntscf.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2phzjunpd.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2mpqhczbs.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2jnomiwlz.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2tfmjfcnn.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2tbziymdz.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2animqwph.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2ketbrsql.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2bxowtuun.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2oxwbofhh.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2qusristh.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2gneaddba.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2omlemzgz.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2vzoypimp.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2hzyulkbo.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2drdnxdyz.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2ecmkegcd.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2mwldtpue.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2jjdyeqpb.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2bbyfowkw.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2yzhlzroa.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2mkpzkeoq.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2vuyudwxu.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2xltqzzqe.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2ohfqpdyk.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2qhfttikl.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2rommvmak.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2miuslbdk.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2pzphdlrm.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2mxywgxbl.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2wcptqfcx.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2kpvhxdwe.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2vctcfypj.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2kqqaxnvz.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2hbiwzrlg.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2scplqamd.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2mulbwxna.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2nxzymxrc.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2iyqnonsq.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2zthbetza.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2rgrhqzmj.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2fgwiyuhz.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2lwhavwzh.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2xddycjyc.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2fknysqog.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2nbcvqonl.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2zgvcyrcn.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2fbfekhzr.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2eshgkwzv.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2srhvjfcr.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2rvetctte.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2pmpreaof.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2gkvfsnll.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2qxwcyhnx.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2wfohsgdb.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2zbjkcowu.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2rcsjjola.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2bromjxbb.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2krxszxfg.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2bfyppfoq.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2dtrvelfe.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2afkrvgbj.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2mcgmripw.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2mdkxzjms.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2tzuxutgm.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2waewleup.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2niartcwp.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2dsqsnoku.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2ulqsbqqz.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2lxofuvdl.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ymnjcxdd.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2qkftorha.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2qcboesdv.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2ngswitwi.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2pgegezld.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2brtmubvx.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2xyfkxoev.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2iipdoqmm.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2qnmowkra.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2iesbirvt.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2hcznhekc.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2wzqbqell.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2vfsxtxtq.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2nqngduxs.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2zhfaqxaw.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2wzrmwxug.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2gcgeecxd.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2jlyncmnz.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2muntbsga.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2wdaqnrhd.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2iwcvrrex.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2qdlosdaw.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2pbkbbsvz.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2jxqrnegf.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2apmamhrt.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2zqyuwsqs.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2rtakhbbl.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2dnojnifs.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2woacaezk.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2lyohtgoo.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2kbpnmtmg.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2kphlfvhs.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2cgigwaus.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2nixdgjse.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2kshgtpml.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2qlavfwcf.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2cytefbur.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2enjpbvbv.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2qxkxblvw.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2goqnpbky.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2mwujsjtd.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2kxpsswqs.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2jyeodacu.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2quyvxgal.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2gitdghgz.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2tjikmrrm.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2muepgmnt.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2hluzunsv.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2vxoztebs.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2ctrtyvfg.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2sfrlydqr.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2qjefmbkv.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2hnsbxqeb.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2zietjbxe.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2wbldirkn.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2uaxmnvvk.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2klizbnou.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2tcqnzyuu.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2tuvwhdlh.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2eogcsdwu.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2xnvwctuc.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2geoeeabd.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2edicpqja.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2tbzpjnsj.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2kyfcrvsj.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2obqwgxdf.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2xifkatjg.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2gbmrnohf.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2wgfohxzt.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2xzbhdgdt.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2otzdsybo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pvmbcxxp.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2abnbtasi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tdcmogqa.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2alrxwfgy.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2rpbrhyjn.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2pyitqglj.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2iwkbsrut.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2wotnuqiq.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2qyiwtdao.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2bgzpgsea.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2tihhineg.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2lmgzpylz.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2utfxceoi.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2fgxhoauq.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2oovyrrbe.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2yboofqbs.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2teahayks.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2jqdtixgr.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2oxrnpujp.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2dpganssw.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2lcnvkmdq.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2bkkufgob.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2wmkgxtyd.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2desjibxx.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2cxkebhfs.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2nyizzaan.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2aniduoga.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2waszpque.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2llmvmxvo.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2bttidqik.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2qljlndbs.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2kiiartcf.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2yzdukavz.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2cfwufttn.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2lpljpaby.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2klbubdte.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2dbqwnyzt.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2jjdlgmno.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2pjwhdrhc.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2jkowzifn.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2lkenmmnk.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2mlsqvrhb.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2hcqfuybp.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2qbyvboyu.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2ggkrkypu.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2uiuyvutz.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2nudhomob.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2hypmkaua.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2wtwvkxgc.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2ttatrafp.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2wsqemllz.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2ibsmnvlk.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2nvwclntl.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2ucpkuntx.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2shpwqvpe.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2bzmtimqa.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2upkzdtyq.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2cunlcdmc.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2jkqcpyfy.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2llhrcisc.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2kwormito.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2xsfcolre.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2yjdmuztb.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2wglfirbt.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2fyfjytmk.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2kfpwammc.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2pavimsdv.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2ithimhqj.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2vdcafhrz.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2mcubzupm.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2gtdcrpdw.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2qkgogyhz.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2nagqziqj.html


<!-- 参考信息 -->