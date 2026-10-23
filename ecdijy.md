代发 wailian999

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3aoqxkpuu.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3fnuzmifk.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3zuuhkvui.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3bzhpuosa.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3reuzamtj.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3enwcpntn.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3udhgcnjj.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3tgwfdmkn.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3vokegage.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3gsfvjevr.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3ysfqdakq.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3mpeqkfiw.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3yppkjeny.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3viyobict.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3mikaalgk.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3fjevqswm.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3sojhhqyx.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3uqgfzphm.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3yzwhzszs.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3kdllqtll.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3ghlizmxs.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3lmlwwopd.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3zpjtuhrs.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3eapsyfmg.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3ujmnozcz.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3vxfmctgc.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3aspfouxc.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3rfxvxzgt.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3afgvmhmj.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3yktzkqfj.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3hgwernav.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3degeutjh.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3brayorbm.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3xrvpbowg.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3kstdfwtv.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3qetuidtq.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3gctuwtgb.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3disxbpda.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3ryjnyidk.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3kjtzisce.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3ymbtgtzw.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3bezyrrlj.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3ixeldnmt.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3gcfocbju.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3iqcokmbb.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3khzhllbz.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3zapbeqjj.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3ltxzxvlm.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3qqyevdcb.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3yvhexkks.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3kxmyyqgv.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3rjszgltn.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3kebyqrdg.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3klziejmt.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3ogspukgd.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3fkuczsib.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3jgddrhwi.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3iqrvlvdm.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3cofruzvp.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3zmnzhadm.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3lqpzivdq.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3tyxeherq.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3kencqfcf.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3ysxvgpjl.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3shaneyyl.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3lqefrntz.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3ytdxavek.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3mghavvkf.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3ajcrldkl.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3rnnxaotz.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3mrogtyos.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3hgwuawwn.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3zayingkw.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3wtfdkjao.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3bvdjyxry.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3tmsaaxne.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3fzvqfrlm.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3bhibwcnh.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3rvqfkobc.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3rngpcttq.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3tchwqghk.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3dicykdql.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3jfppvlaa.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3wuebwnwy.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3zcwstcpi.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3qldzcpta.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3zyyxsgng.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3sviffrkf.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3zfjgcvrx.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3elzrnwzr.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3yubuwpjv.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3bfykvxcb.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3obtvjklx.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3mqaptxmk.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3gpwccese.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3vkhsnnhb.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3qqyrmjmy.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3ulqjfoki.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3khrepvpx.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3ixdlphdg.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3dkujdyoy.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3fdnohqfj.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3yobynbuw.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3aawskxmj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cebxznmf.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3iomcrbgg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zxyefqpc.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3dsteympw.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3kiyxgosd.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3iobpahqu.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3dltcwyvx.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ymiyqtpy.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3ixwrbufp.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3aogaeccx.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3dqozgxct.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3glrvpydb.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3aocfbgfh.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3hibiqgfn.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ujdzepwm.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3kcgmvmmb.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3odfmivin.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3jsueqrdo.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3aqagghlf.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3usazwefn.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3cwsrxyjd.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3mxjjnhgc.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3dcdodpjt.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3hoslejnw.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3vdmiewia.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3mfpydzku.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3lmkimogu.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3kldsevwt.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3gobstglc.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3bszbreah.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3uoxijlvy.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3lpzhrpft.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3eyarfkns.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3yshebhyx.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3hmkuiyft.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3bxdhfbbd.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3nrrknfoz.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3xczazmin.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3deiatbly.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3bgreexul.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3gpjxbtmo.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3huxgxubc.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3prqcichi.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3qtgrhkwt.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3ofjdhlnr.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3kxwikowc.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3oezazlee.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3mfmwvegu.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3jgrrhkyf.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3rnaterux.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3ythjzayg.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3lpiciwub.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3uyytyyrd.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3ydjnozff.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3qhgepquz.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3tjwkgnil.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3tfzrefwb.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3scftbrpc.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3aynveany.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3agpmtneh.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3pmvvkkks.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3gdkhjdwt.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3tzmsizex.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3iwqxyhtg.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3agrgkaaj.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3actroaza.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3ejoohufh.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3mszlcjfc.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3pqfbubft.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3caovdmlg.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3lsmqddwj.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3lksmginw.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3tmuomktl.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3qgrxgsjj.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3stokzpju.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3uiapcilp.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3vhrcwlyt.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3tmbxinzj.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3kfdzvjue.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3jtudtbto.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3ioyprbpr.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3qtiiddlr.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3lwmycugt.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3riwgzbkw.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3gtihoglb.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3kfrlbvwp.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3zahfwowf.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3hgjbzodi.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3bqyhkmnu.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3unnmbejp.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3yjzsgonw.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3pohixxbd.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3iredjgpq.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3ohehcwkk.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3lhxnjnlb.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3npksmzvj.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3buvovrjz.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3tsibuqie.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3qnvhjviv.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3rfnmvotl.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3fjtenyzt.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3jqhfrchq.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3hxnqwnpb.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3wsndwxhi.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3rdfglufl.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3yoqxxtoj.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3bkqopvmx.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3qjvrhcim.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3qkkhjjrh.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3ajhxipsx.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3kbrzttah.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3edqahrvz.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3dkglsbjj.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3plsusiyz.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3nqhamidg.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3qwqfrwav.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3goucywaa.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3psqanyqx.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3tfezfxti.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3beapxoda.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3nnvkoibb.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3fzeqiqei.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3nermpbwt.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3vorsikwf.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3hnvjtssx.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3cmondrik.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3krparqub.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3rejkknps.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3saxqvusq.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3mdrlbvbm.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3dchsxlvn.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3wrsusxks.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3zzqdjkze.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3ergstfet.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3kxulzuly.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3axuoxetb.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3lrygivbq.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3tqgapgiz.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3bosrktpk.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3puqtmgyu.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3uvbtmmab.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3ngtmtlqg.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3fqvqyddq.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3oiqwkbsf.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3adikctwc.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3bluoslsc.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3ecsymsdt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vremmycv.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3aekuzgrf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wbxhfsvs.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3lpjhtqlb.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3kwtspdia.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3nykdtovs.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3bkhmgjfx.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3siqggmja.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3tbtqwvls.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3gvrpyotz.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3jezcrnmp.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3dbpjfsxf.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3rwclcmqc.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3hvsiuwwq.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3mhkvcnmx.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3whbcebxk.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3fawounug.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3eamzronf.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3txjojtwh.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3rffnkguh.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3wngfuvfk.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3stfqkaql.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3oeleqsqr.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3pxkeljfd.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3coqfpsve.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ojwhdooa.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3guwusrqg.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3xlvxfpef.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3digqhdvd.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3yykiuruy.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3pzwdbpqk.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3qtsuwwhj.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ujvxorqj.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3rgewjmyg.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3rebanihm.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3pfckfpzd.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3mztftyqr.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3zqtbpexe.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3hvftqyqg.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3ukturqss.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3mfzlqprg.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3wazlvwvo.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3biizzjwv.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3gercszxz.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3gjaigqwa.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3hfukyqex.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3gouilziu.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3blxapjgr.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3kzjglcit.html


<!-- 参考信息 -->