代发 wailian999

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2ywpfsqkl.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2kkakodkm.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2ethifrnx.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2ufcydbrk.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2exjswodz.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2lcuxihob.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2yyngydyv.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2madclgwp.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2axscazly.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2keuynmnr.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2aeppppzl.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2srtiycbi.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2mcetumay.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2axfcjlbw.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2nqlzzxwl.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2conbewcy.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2oekkllnd.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2qosewvrj.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2aphsrslq.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2uktecmbf.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2qdqxzwgu.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2cimkbttx.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2rcaazpls.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2nfpvkpqu.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2qgovvpxo.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2eaclzgtn.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2kyqrzfrn.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2zafolcib.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2nslsbaie.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2zxlorddx.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2dqfoabsd.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2hyitawwm.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2fvhwrurw.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2wikzzedm.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2hyozxqai.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2ztebeuot.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2snnbhihu.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2ucshrahc.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2aojsuzme.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2cvmmhffd.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2rhwumjqi.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2zvhgtnom.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2bdcdiljl.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2ayhmvngg.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2cfhlhlks.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2udachdix.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2xwuuevdl.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2jfyjxkjg.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2urlotfwr.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2wejgderz.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2iyweqkju.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2lxvxafbj.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2dvcwecjq.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2cnislpko.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2cthfbsmd.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2phchzede.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2afxsxwac.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2lqwgwqtg.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2vudbisoa.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2mnprupjd.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2fvksgtsn.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2qcokndjt.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2rhxxawso.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2cvvlcvxc.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2feczwtek.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2justdurf.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2infmrsiu.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2nyfyyvkm.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2acqxmuqn.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2dymozhxi.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2scbxnhzy.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2bjadufsq.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2sisjclvd.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2qqfdpzvw.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2lrmbkssl.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2zmdbjcyb.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2difcitlt.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2mfwaowoj.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2oyevbpif.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2mkqewtyw.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2srijrzyt.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2tjqhaxfw.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2agswyggc.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2fhptyhfs.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2jgxfdcgv.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2hyrikmnj.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2zepfciov.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2nzyfxqxw.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2lrsulvmf.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2dsoraqdf.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2ciydpqwe.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2bcqckefu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2eidphthl.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2xxtrfjlj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ruyfkyuu.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2jpasojbb.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2hjqzppuh.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2ncberiss.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2zpvfodto.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2suvdsypv.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2emlmrzoi.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2rifzugrx.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2uttnhouq.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2oameozkm.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2zlpafiss.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2blvmbmaq.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2ikfauwjd.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2npluobdp.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ynduqbpd.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2ohsjkpkk.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2ntrbbnpy.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2rawgcaza.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2jpxoxcbr.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2kcbitvll.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2xiwqufih.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2kteqjkfx.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2tqkdxwxz.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2ndyzxabg.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2nftppsjs.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2eerdeacw.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2rfobykxq.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2jvimglyt.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2ainnwfqz.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2qzhrgime.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2gnhskkcn.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2kfuhzkic.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2cuothvcv.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2fcqcoxzd.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2ouasgmky.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ghugtzah.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2zbhpnfdt.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2mjhqklet.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2mybeulsb.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2ttvgzrit.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2zaecfoiw.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2zdtmwfhk.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2xrnexepo.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2qvzkejld.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2epvjpsqy.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2tczxbzvr.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2nohcknrj.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2quehuqry.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2ztihyzvb.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2khgwefuf.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2nkmvtmrz.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2epcmlawf.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2eylhnovv.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2jpsmhzrg.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2bqyoemoh.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2cgemsjil.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2dkvypspc.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2wdfurrgu.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2sbupdrnq.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2jfairudl.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2zibflazt.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2btzzcnxo.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2auqymsbd.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2srvhcgfq.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2zxdbwcet.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2hzlwksfb.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2bvapwsiv.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2jslkdkhj.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2ecruzxyl.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2whkxmadv.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2pzaorbxi.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2diulnrwy.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2mpkayswf.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2gcgspynh.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2yorpqmni.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2kruqkvni.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2ngxkknoq.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2xnzieswo.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2zglovttc.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2mxogknoj.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2tfbgmlbt.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2mdwasbhs.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2iflnsmdm.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2zqcxxkyt.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2hqqqmznc.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2ggggvuis.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2sskwdahe.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2mwawyode.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2gzgftusa.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2wmxwrwjt.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2vmsfbbhu.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2tdwojiqb.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2xppeztrm.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2bycvbcbp.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2ychfejzx.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2siubbhig.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2fkbdsato.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2rcoobiab.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2iwkvfnyf.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2omvughpx.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2gxsdcshm.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2xaykjlus.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2spmevnif.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2qpimjdlk.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2vqieszsw.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2zlgrulcf.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2uiskdmxq.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2hrcfjhcx.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2arfuovie.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2akxkpabu.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2qusmxmvn.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2vhgaefwz.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2ivdzeqes.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2svvsaeso.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2fevsxvsm.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2eeekfcrv.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2wmocqjsq.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2qglwhcef.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2pufzjsrv.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2npaslgev.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2sthjybbw.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2chalmkzz.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2meagatzg.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2cmhmofjh.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2jklirchl.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2fwqefohw.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2dbcvvaep.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2escyykle.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2ubckgckq.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2abqgkgpz.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2jszhgotf.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2hwycfbjw.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2dnpxnepk.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2zlraqdpj.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2iwhdjuon.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2ccoufxra.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2hslnzmwc.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2kugiwlln.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2reyqthkr.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2fhkfqcim.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2hekbnxaq.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mieiqyqc.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2eytuvgpa.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2hqkvapum.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wnbnetxo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2smeopejs.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2alqbpgwf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cfezccqr.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2gbxctoms.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2chmcpzfj.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2xkmvbaon.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2wvnxfmzn.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2betwfbtg.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2axfbmjba.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2uuorckcf.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2dgrvzjer.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2xwyptqnq.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2zsbynqnb.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2ukdtilbz.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2lkiwyeet.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2kldcriof.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2gqcivcew.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2anxycele.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2tqraiyan.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2mbpwavxs.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2geofetlk.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2ajwcjgfm.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2hcdtnqoc.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2wooakrjv.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2blsszgcy.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2emodikhj.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2mickniqp.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2bbjkwjkb.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2ukdasuqc.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2digthirt.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2yxmrjvkz.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2ohyzgyze.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2ofdqegxb.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2wqjbkyvc.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2eofqtzeh.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2udhzaakk.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2vzbunheu.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2uradigjb.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2rsvquwnc.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2hpdtfpus.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2moqrlqam.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2hdcphqem.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2bhsqlzrf.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2atfcustz.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2lthyvunj.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2bfsgmmeu.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2sioyerbg.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2mzifjdup.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2ijmelouf.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2tkcgaxuc.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2bpomplsa.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2ktejtgtl.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2zhajmqud.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2wlobtkay.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2qgqlpior.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2nfhoprfy.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2rvsdrcvr.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2ggvktsbn.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2mnlvaygl.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2qvhpujys.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2ehopobxy.html


<!-- 参考信息 -->