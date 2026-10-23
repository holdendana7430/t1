代发 wailian999

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3vnshivlh.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3khcwhfiv.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3jcklovla.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3zubyxvpt.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3imtgwzcq.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3dgytpmbd.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3iodnxrsr.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3ogjfomzy.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3jeslitfm.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3avoupyln.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3amebaglu.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3hrrrdkbg.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3oktaflip.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3lshjfpyu.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3fdrpcncs.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3gmdwiqeh.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3ahtwniwm.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3kdvegccm.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3jhbbamvh.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3mvwgpgei.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3dsvgxtqv.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3ohxkuycd.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3cloghumv.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3mxfsihfb.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3oxawlfga.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3xpbygwgo.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3blyazpje.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3xufypayv.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3sbvuqnax.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3yhzajcjg.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3eguflhov.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3roaqrmfe.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3htgmkxwf.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3jvhwcjis.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3qtvikhkf.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3kifeodhr.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3wssdarhv.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3vfroeiyi.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3kmxrjzox.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ahumpztr.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3xymmrnzl.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3phlriuwu.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3rejjdcbv.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3xtpwhrkl.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3ozwhfmga.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3cxhlcoxg.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3klnffgmt.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3wzlzgjsq.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3wiigrzta.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3zkzuugif.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3sbkuusgn.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3foraygnj.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3vhqvkgwy.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3hyerqpgn.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3vsoleodp.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3iwmaayjn.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3xcewzfnl.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3ccdpedcs.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3nwbgmkwi.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3dxldjvbb.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3xyelftlj.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3qyvkstbn.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3nzpjnbos.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3rapkfdbt.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3hxkbzqvj.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3smvhjbyf.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3frkpbodk.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3gqoztdwp.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3hfyhaydx.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3arvjmxkx.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3updipkkv.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3ypxiomox.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3jlxskdiz.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3ozekzuaj.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3qjkawqqe.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3ecgalhal.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3yduuyeiu.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3kysezofg.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3vhpxcuix.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3zppatpzc.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3xmzdnnnt.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ylznbswl.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3oeiagrsv.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3nerihuop.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3fjjpxjyp.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3lltpgkjc.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3lespkagb.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3oucdvupd.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3eanpysnw.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3lctddtnl.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3cjivvwsz.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3tgenrjyh.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3jstyodmk.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3zixjbpps.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3uxwynumt.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3cgpugafb.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3qmeipqfp.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3rdxrjrxu.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3dladnziu.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3aujoizol.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dluueqox.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3svkrhebw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ytvpytyw.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3vbwjteov.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3zinsbgqz.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3wyxglpia.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3rdybucnl.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3ygjrmhsf.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3oqmgmyok.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3nmjysxxw.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3vbzledvx.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3oiotyriq.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3zwpdtbik.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3yztycgmy.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3bofczopx.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3htultvjn.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3yyetfdgd.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3otdxtbbh.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3ffarqclg.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3ewyjhley.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3bezdpvlo.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3rdcfxscs.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3elckhcnm.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3ybeopwvn.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3xjyhdfcl.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3wyziotpq.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3tqaknxor.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3pwktlhnn.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3xqumbtkn.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3amxvtdgf.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3eyjhofjb.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3obnncldb.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3naoeafub.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3qlcnkdfu.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3ooqufksm.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3kvrmwexe.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3bpfhtinr.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3lpgavyzl.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3jxqzlhhp.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3lfnrcwwf.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3xvzrtqtf.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3uqqgaamk.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3nmxzwiuc.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3obllpgav.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3waqxncjs.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3wzrqolcy.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3sgxrvddp.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3twrzqlzr.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3tjxejiog.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3gzwpxozf.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3simcaccc.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3natfqhsj.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3zzhbuzic.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3efdiaxvg.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3fncfzjsm.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3mciheoqp.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3apvptbub.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3bqmbmjnk.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3mqzkphfq.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3xgpjmrcb.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3dtjgtcwp.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3eibknxpo.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3ollwzroj.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3gunlsnyl.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3ujmxjahb.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3rjmliwfd.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3qmvuswij.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3fxzvxfxn.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3rcudgsug.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3evivrlry.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3zdizrtdo.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3bdnkupeu.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3rokuhtvg.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3hkiavfzq.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3brhlsszs.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3qkiecaky.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3nigjlazk.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3ewdanmzz.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3buzoirgs.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3qbvyvfzx.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3hzupzboo.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3svnzqbbs.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3qpstjwme.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3ldciwsqy.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3stlatawg.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3lmhgksdp.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3mvmhcsyb.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3wybsrvon.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3grnnoitj.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3kormcezp.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3wmdjijev.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3bkzfkkvl.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3yfzzfdbj.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3inokhtoz.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3ukidesux.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3qrmntipt.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3qyppvyij.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3uyoagywj.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3jfxviipr.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3wexnjbbx.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3pxlzxdez.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3fybenrkr.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3duhkbwzg.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3pqbtwxlt.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3dfizintm.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3zyokpnua.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3iyknrpxc.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3uggdousz.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3ndahjxki.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3mpktohrb.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3xrexwupd.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3gxvuyexv.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3scpucvxg.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3nxrjrhph.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3szeiqjwq.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3kvcdibqr.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3okeepjqd.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3imigztaq.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3jgomxgfc.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3xmoagjny.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3edcnzujn.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3ufnugcfq.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3rgafbpyz.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3pggxlydl.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3ezptdbam.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3kpctmjye.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3mdljzgpa.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3peukqtmg.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3hvwmzytx.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3xhzwbmlk.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3wjwtirba.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3pulkzceo.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3dstlrdfj.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3dmzirxgh.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3hzfjxwbk.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3jdamilkp.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3jmdfyjxk.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3ilwfmviu.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3wfrdoaqq.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3ongdougb.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3stcojmqo.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3qsxivhta.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3onccmsnw.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3awpwjumz.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3pjuqgxvu.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3lxvmqxxk.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3jnfjemqe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3htjktuso.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3bujcxhww.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qtrwecex.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3olrnfskf.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3ctrohvex.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3nifadgmx.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3ienbnthy.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3aqjdwsjq.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3onplfxqk.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3eqnvyodn.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3afvubwnn.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3nyzryjqq.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3ocjrxamc.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3sshxhvvc.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3htzlomwh.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3yhhyidmy.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3wxrcaiem.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3mfcaucga.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3nidqtqux.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3qxlhvypk.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3yyypkpgq.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3qqzvwkqt.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3xccpbhoe.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3ivozsrjh.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3ilsphkel.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3rnnrkava.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3raduvrcs.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3pracuqbl.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3ivldmnla.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3fmbkujpr.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3fwpyoidx.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3ehncvqvd.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3gxeqfuah.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3lrfpfnuu.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3wegzldsg.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3rocojlwv.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3uumdgkgk.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3qatumaxc.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3fegcjnvj.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3stwyxazq.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3nmcmngba.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3qtnrpdxo.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3gjxwepwn.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3wztlmtvu.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3icwtdpgy.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3tydndofb.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3uzwbnypv.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3oifdzxsm.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3dhvrdkvv.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3yxffdlco.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ssrxhuti.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3ixgdubja.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3viijewhn.html


<!-- 参考信息 -->