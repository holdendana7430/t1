代发 wailian999

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3gvjunbpv.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3noahgbbi.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3rtnjeqra.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3lkhehdnz.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3ngntonpc.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3escakzcl.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3aiqhjsii.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3vxlnypvc.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3gybhjbtz.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3ohrredap.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3wqwkpgwf.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3qrrvmyis.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3rlbqnwtn.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3nbeynrpk.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3urupfidd.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3xlrvsmaz.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3lxonxnjv.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3ekytmksb.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3etpmvdih.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3ocrgykqd.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3vuvoddee.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3qquczlcm.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3mbajhhnd.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3xwekumvv.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3orzxvtev.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3ynxaphvs.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3xsziqyhq.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3ukkhgpuk.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3ulolzkzr.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3xlululou.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3ehsjfmdl.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3llwnlowk.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3rwcggihj.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3yqtmxxyx.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3deubrpfo.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3ztwbnfue.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3abugoscn.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3wxtwqeae.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3ljwjwauo.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3xegtfsfv.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3cobnskrp.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3fbuwuaxe.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3jwvajrjk.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3osabocnb.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3uerrzryw.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3chshmcdm.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3xwkagzgg.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3fkgypavd.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3jopdxnui.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3xarorcar.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3ychmxerk.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3ywakwfgk.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3pbmtnyin.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3dtquihgn.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3cxoumdme.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3lvmvezye.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3lbeoyssz.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3lxjrxwge.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3qscvokux.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3bdoqnnpr.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3hgfrrwbh.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3dlkawvbx.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3cfgvapkj.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3prokprpt.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3jxpitwpt.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3yihkvlbx.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3nmralatv.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3juosrnfs.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3zenpdavu.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3eaajgopr.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3fkepzkhu.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3tdvovldz.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3dqkwofme.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3usswzaad.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3nbfyieoy.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3cvckffgu.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3ynmtayxk.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3vhqpbnfd.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3zzgvbjgq.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3eiasvcxt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lifojlzx.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3dejamclf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jzfspnpg.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3flaucipi.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3bzptxftt.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3bwoqdqed.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3cuoayurc.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3hlqptbfx.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3issqnrqs.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3lpyqjsyl.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3rsyimphl.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3smwqqcpr.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3mvxfbrfr.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3kredmokf.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3cgyonedi.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3blsufhcc.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3kcptdjmx.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3unfcjybq.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3mjtwthco.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3lzvecbqx.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3wujtphwm.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3huxaizyh.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3bkymctkq.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3erxzdijj.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3cimweair.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3hsukcces.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3vpqhxzfx.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3coqmdtpa.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3jsjucqgw.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3vpinmuji.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3gduxuuux.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3uotcsmvf.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3fzccicwc.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ukvltlhw.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3gsgzaobs.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3dgcwwdzj.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3glouikcr.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3hnoueeyz.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3yhcdgmzp.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3dnwoqokn.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3wcydzmgo.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3xdwjwgcf.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3avzeksra.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3xyhzzbbc.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3ywjzqoll.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3gfywvkdj.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3aogbpnir.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3sfkzuyqz.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3euehcuck.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3yftwycvk.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3tqqmixzr.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3ztkmbfhs.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3ujayvbby.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3zlunjgee.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3rfnhyclf.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3hppjmvpf.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3dtuqmthn.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3tzcyhzze.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3nogdyyvc.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3buwecnci.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3vnirbugf.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3bvlzuyii.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3ptclkmky.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3qotomkyq.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3eniwdbhx.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3napwradq.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3mmniznhm.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3grqjrirm.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3eywsjdqo.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3zobbvlsa.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3ajmdfshb.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3dgubibwb.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3oipkctxo.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3nfcflfaa.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3ibbmqaim.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3boeqszly.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3nkimjdxf.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3mnvhcoix.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3ylfpehgv.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3gvpzzeut.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3bxdquspd.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3qjyqkslf.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3mgrwhqdv.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3xotcviki.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3fnxvnrpx.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3mhmxcblx.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3xharbudg.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3gxnxblxa.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3pbpsgbhw.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3miowvyrc.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3zikjwpxj.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3kylqdhrf.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3kgyxnzyw.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3unvqmmoz.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3rdkzwnvj.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3ioqvouer.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3mvzjtvym.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3bcksdeao.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3wexllmgc.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3glfhtbam.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3xzytrvth.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3qbhcsvzl.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3mhlaiwdt.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3fptblchy.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3iigsynbm.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3fhzromug.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3wgjczjvr.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3mgfvychf.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3dfszsmbu.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3emlcihpo.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3twajyfwd.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3fzxqqznn.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3dvisskek.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3jvovfhrz.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3xyxobxwv.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3yptzwvqx.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3skbipspa.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3qvjsvwpr.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3tzcplqdn.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3gubxagib.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3lnzfuvcb.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3hwonryfv.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3jkpvcjau.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3wzmlfgwr.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3jvckicyq.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3lnumtffu.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3qvyapzxp.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3asgzfuyv.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3ncbgoojb.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3lpepzihz.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3nbuudhuo.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3oienzoxy.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3rwjvwrzz.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hwrnhfka.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3sqotxqpl.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3nmcbitgp.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3pmsisvao.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3vbsomlre.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3qnocrolf.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3clwhiguc.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3tlmwyqzj.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3plseobar.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3piwbgujq.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3pmjjmjoj.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3tnkbvsih.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3rzghppsq.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jimrywka.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hplfvveg.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3ghhjwahx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lbnqzsry.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3upwelbmm.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3fkidmilf.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3cpnzvawv.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3projqxlt.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3yqjjtzkz.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3pernuiku.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3tbdzawyi.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3uctczevh.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3jgdcetyt.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3jxczpvnv.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3vvxltoxt.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3bxljxatd.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3yttnhxrg.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3idilihuw.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3fbsrpjew.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3bayilfxp.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3yuynagus.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3fopntsqg.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3mifscchz.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3behswpnm.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3mspxiick.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3hjugoerk.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3eeepwzgi.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3opnkyqxs.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3ejecaxvc.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3acsxxwyi.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3wejafdfe.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3ulnfskgr.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3cvekgvuy.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ziddibyw.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3xjihskcw.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3ekgisrtc.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3dokvhtwe.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3bhjzmdbq.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3sjiseecv.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3kqbsdddb.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3gzbfnwdd.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3mtvjbxau.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3vbxuhcuv.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3rqmxxzed.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3juekqlta.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3zujuedgi.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3qnqhrdml.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3bsdveckt.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3vmicxwty.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3djtzjkog.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3hlfwrrzq.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3fakwlijx.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3acofbivb.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3cyizqeql.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3lxncgfvo.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3kqbyvevs.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3qteliyxj.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3mnatagpe.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3nezvzray.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3zlbdadcm.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3fibsfywv.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3bcewpokw.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3rrpfowyw.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3ekymydmz.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3tblbbnom.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3bmrfjkdy.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3jyxtcogr.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3crqakcxf.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3kdjjgonl.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3ymnskslj.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3cqlhxdkd.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3hirmesxx.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3enhoqvin.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3kmxssohy.html


<!-- 参考信息 -->