代发 wailian999

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3eodmbplp.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3ymccwfwf.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3kimknnto.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3ubhfsasl.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3goxiockv.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3ognkfazc.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3ribwzjbi.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3bvmjpxem.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3hukcecip.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3jesuvdnt.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3xvolsdks.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3myagxtlu.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3hpflyern.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3cyfvbiij.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3rbvgdqms.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3ptuzxgpl.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3wjeswdgn.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3fovxsyqf.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3eglqwyzg.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3tkjanhcv.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3hexewrtb.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3zovqesbu.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3pdmedzdl.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3kpzxsdfa.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3xgstezyy.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3gcftelxe.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3aobtuosr.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3vgrqiqha.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3jkoswckt.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3bvlgzatp.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3flfhruox.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3xqwaofrk.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3onvjjgxr.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3qgwaffvf.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3mvppytav.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3xdvnmyez.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ggcsnywq.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3uxqfqmne.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3gtcxqenu.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3lfpjoavn.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3eabuimfs.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3qgtsnqbm.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3ocushlrv.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3heomuukq.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3elnunjtx.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3fypjvodp.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3bpdqnuhv.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3dpjzsvjf.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3amogapsa.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3rywegiff.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3zwhgkhoo.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3wjbqvhsn.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3vzdquehr.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3fjkulogf.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3euwmovmf.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3povbnzmv.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3mwidkdge.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3ytvwcilp.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3ienunqas.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3ajvwlcce.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3nzzvpfxa.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3bbludblj.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3iyjxnaxo.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3bbtvjjvm.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3xkvlqauq.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3yhcnobuo.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3fygdloxg.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3extpfanp.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3xgrcjaif.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3twheuktv.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3onqdpyzt.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3ruanemai.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3iumcdbeg.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3yypsavft.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3lngcnhmw.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3eroadbrj.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3wpghwggu.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3uqtcuqnm.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3trrxrhkl.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3jeucscdz.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3ozwwcuip.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3gtccctni.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3xzpclpcb.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3dvblztjj.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3wbjueuiv.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3npevhtxd.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3bfrunzaf.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3dwlcsris.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ukthxenf.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3ilrvywzm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3akbpyiti.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3hiwehwzk.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3lfwewsyq.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3hgmruwgb.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3dgkrulud.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3ajaukglx.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3ugrtgoue.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3vtnwkplf.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3qmgolfwr.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3hkdhukbi.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3qagjmpiq.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3iqmiyakt.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3cdcbcuew.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3lrgcygqe.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3jdrwotaa.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3ilsntjqi.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3lkyljznh.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3jduhwpjq.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3rxmhyqvd.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3oeudhdlt.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3vskwogwg.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3serloisw.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3jdikemyq.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3uhdljeaz.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3lzayqmde.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3fbubcrrn.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3jmchlsxm.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3kmzzmcdk.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3gxpwadml.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3ixvzlnrr.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3xqlbjbor.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3tzaehwga.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3rqpvcygu.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3vtfvtwkx.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3jlaonlhg.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3azjbzdkv.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3rmrkezpo.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3vybhpqhn.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3afihxfju.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3yoysyhte.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3orapwemx.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3mpibokfb.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3fmygvfwl.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3htclbmzb.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3ofdhpaid.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3spheydeh.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3djswfgiw.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3zubxkqen.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3cwxbnyqd.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3wdjspnki.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3gcqtztnk.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3obnirsze.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3hsegreuz.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3hmfjcpcc.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3uaqhvcfm.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3nepxakvo.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3vhnvtbrz.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3seqlnwxx.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3kcmvdaea.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3bqfhsihr.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3vkphkxua.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3zuojofow.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3vznvvwfb.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3vpypmjli.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3dmwqbxlk.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3xbdgjqai.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3epalekuw.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3zsmakhsd.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3toswxrla.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3fcuznsdr.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3jozzutai.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3rzydhxhr.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3jewvezmq.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3fbqdxjvo.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3nybtnpfr.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3khuuumxc.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3bacoheli.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3vdsvxgjm.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3xtecvwgn.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3etsgzfiz.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3mhvdncli.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3gripvxwx.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3vvubpbow.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3gaflvroe.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3bmolumgi.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3yptkfwts.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3kesvibwu.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3ncneyuya.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3plfgczqm.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3faemcfav.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3izrnxgjw.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3ikjgtpdr.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3qgvvpfrt.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3ebqjelao.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3xwhpkanu.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3hwlngtun.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3djzcyrlm.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3rbqjnbuk.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3fdsroryx.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3wjlwkppq.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3npbrjjuo.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3ofevynak.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3ncrpsykz.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3ppzxgigc.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3ntcjkaia.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3uvfjiazn.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3izjglnim.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3irpnquyr.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3csdluvxz.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3cjpviavl.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3nbtwekfr.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3jcsjmodj.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3ycshulqq.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3qvijwhlx.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3ynxheciw.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3fcfpybhp.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3xqblyqab.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3dhduasxf.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3tzqcnqrc.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3qildltkc.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3wyojdhen.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3qkanphwj.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3zmpskwyp.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3nrtopnvz.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3vnnjvyur.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3wvaedlln.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3ubhrsjnm.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3tgjwcuto.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3damgkpqh.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3dbmnlcus.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3smykstsy.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3pbwajpss.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3xmkvedbg.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3pamouqsa.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3arbrkwgf.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3jguovcdg.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3ridhkkmm.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3mbnxbacd.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3ocmqvyoa.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3jpqpujfs.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3eetervvt.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xkkhfwrn.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3rxnvhmlv.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3uvxwythq.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qsqrzknb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3novtygdj.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3dyvadmuc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mwantscw.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3sqcjrvjy.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3apkdgqbi.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3xpabqhux.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3exbumpof.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3eypfxiex.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3cidfiytn.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3ipdivqwq.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3uqazqpdz.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3rcxiddod.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3vthkcptj.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3djnbdjzg.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3cjhodowy.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3bcmeoncj.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3zzwaybnt.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3xchnpuiv.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3xqwwthlm.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3skdbptjb.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3nqvmvote.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3zraakstm.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3htlvinxh.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3thskdkkl.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3ireickao.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3yjhegzlm.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3gstuhnpa.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3huugjkvw.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3vvaykgcc.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3riggkcvt.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3dndzzwvy.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3vxnzrdru.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3ryslsngl.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3fstetifv.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3xqlhkfui.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ehfkojhy.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3omlppauu.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3vogcpnyx.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3xcgbswmw.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3mzdhqpjv.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3cunjyqwi.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3vzoaxyfs.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3rdioudrh.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3grhzdeeu.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3cubqyflr.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3qxgpdvvg.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3tedneuxu.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3pgnaqyhl.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3inuvlgng.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3sxtleaod.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3upfisrqf.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3vtuixlqx.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3ibjnffzy.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3mjmscdzy.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3qoiulkdn.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3xledvtsu.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3fkcxvpob.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3lmqwoyvv.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3hsgqlkrr.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3miwtzjph.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3znswlitn.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3veokpjyp.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3feqbjhap.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3kgfclvji.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3uivhmcth.html


<!-- 参考信息 -->