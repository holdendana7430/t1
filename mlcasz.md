代发 wailian999

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3wslszbqe.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3aekspwzy.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3mozswral.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3lhtdmzes.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3eftzilke.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3aybzmkji.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3erfpgifm.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3xbviiokn.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3nffioqop.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3yckxeift.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3obyniwgq.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3tjpmtxci.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3fnfaxvyr.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3hunzmstj.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3nrekhjhq.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3idnalfvo.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3rvhnertg.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3jcwwfopq.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3plottlna.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3zbngfdfl.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3qmwkjmjk.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3elessgeg.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3kflemcju.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3cmhldyws.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3gydkjmck.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3zzggvfcu.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3mmaedkfr.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3zpkkwqen.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3sdwpepzx.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3xcucuebi.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3yjqothmb.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3aycowcbz.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3agxmlwju.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3ukzjfgtw.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3jgadaous.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3etnkgolh.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3qhzjzike.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3yqjodgfs.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3qeylgvgw.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3vkikkebz.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3acijuocf.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3frgloyvt.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3dmbtvwwl.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3hommotyb.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3dxektmew.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3harlslue.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3iaewnuak.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3cdsuqsug.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3mfxmijsa.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3qmwqywnx.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3lsdzuwkr.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3dzpelcfr.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3mcioynkw.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3cjibfhex.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3qmmriskr.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3gqttjtaj.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3vdpcuahj.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3kjjjdmba.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3sbboiquo.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3jltsvlid.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3uzdktnga.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3opisluwa.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3fslqylyx.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3hqnkcvnw.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3kqjuhfvd.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3jzfwvyiu.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3wpptcftb.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3ywtzlmyu.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3mmshlmjx.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3fyilyjig.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3phmfwxom.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3kgrottcv.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3lnykwxmj.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3rxlegyno.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3roaoqtna.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3uqdtczdk.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3sviktyzw.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3prbytxcz.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3nagrvsdt.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3vkxpiwxg.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3nrukpiqe.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3tjqcozye.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3uhiasfeg.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3nufmybca.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3sbqeguux.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3tzwpgmef.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3ybbnmubx.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3odmtmsuq.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3xsgivzqa.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3obzimqok.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3mepbvxsm.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3urbfclaf.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3cjignfiq.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3qclymdpu.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3sfwykrsz.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3lvpddnor.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3quktfxol.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3rvqasskc.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3aosjljkn.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3ggwlmmqj.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3mviovrrh.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3ummbsans.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3stwbwlmt.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3lrimbyjk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3iwatuziz.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3ugwirnvn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ebprdksr.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3ixofkxcg.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3jbrcyuau.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3kyqurbnm.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3gfveobvy.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3itgybjck.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3yqnpycsp.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3gzseacqk.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3cpjsmagl.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3crrytmhc.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3pxeyjvpl.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3tvdjseca.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3yvpyyvzz.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3usanustx.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3pqnxyfnt.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3hrfacttz.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3dclsdlia.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3ktzkkqyv.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3kizptqsq.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3qdxhhvoe.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3abhxmjom.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3ztgtsvjh.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3eqqptizu.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3twypxjzx.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3xqikmbaa.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3xrzefbrt.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3avczytzl.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3xexsnggj.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3ayvowgcy.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3utafdqhm.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3byorbiap.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3rybvyzhc.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3mtjpcsyp.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3gnmvjxml.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3xmpnybvv.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3hushfbni.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3ovoqupnd.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3lbrvjvqe.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3rcffccep.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3arqdbicq.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3fbycodhv.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3aguyxtih.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3frjcqljo.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3khcoptdf.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3ymptkhxw.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3hklydkkr.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3onqldkoq.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3rtbigoxp.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3bzmgigqz.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3ofogeucr.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3xrtseljx.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3xkdetoln.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3dqanpjpl.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3kjkcjpnu.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3pnrhgjfr.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3sbdwrfoy.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3psgpesic.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3shcyupbj.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3lorzqrfz.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3qshqyqwb.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3opaypbdn.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3nzcgtsks.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3thzmllzz.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3qjiblypk.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3jzamptbl.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3lwsgxliu.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3pepcperm.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3qmnmqgdo.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3wczuetzt.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3wdmugxma.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3wthmppve.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3pvtsuehu.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3hctxmkll.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3naudwkrf.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3nkmkzuvq.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3wrrsxrex.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3mfrncruo.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3yifebgag.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3ethzirlb.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3wpxtvgly.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3phjumoyl.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3flbcqavi.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3bjunuimo.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3mpfegicd.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3ajapkzrb.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3njcdwpgg.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3ledhqhda.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3vnvbbhta.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3dioqjtqk.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3rxjhoffw.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3kfbvbacs.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3mhbjmjqi.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3pcitglvn.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3dokqvhnf.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3zpsadxpi.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3floptjbr.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3isqydbtq.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3aajpkpap.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3syxpfhga.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3phpcvzmj.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3aqtxvgdr.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3hwoutbkj.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3xpxfblbn.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3kxnwthkz.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3obizfdtt.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3bneobhgy.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3toevgfsx.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3sdetosvi.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3zkukotur.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3fvuzxhqt.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3xtkbytgo.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3rfopsyti.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3cftzgazp.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3inpjsick.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3veovdost.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3mfhjmtxq.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3moemoyqb.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3ugdlfaon.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3knqhyyrp.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3eeoyutia.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3fgauybfj.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3hmbsynos.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3zoirpqbl.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3pvzexmcr.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3evglevmx.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3wtbrazwk.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3ragoeusw.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3fvjqpuhq.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3ncmdgscy.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3zsebvymu.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3txljjzun.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3obdambsr.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3oauxzsdf.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3slwfgdbn.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3jivoddmq.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3rlquepxg.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3prgynlly.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3mipzuxoi.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3hkpxpdbv.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3fgopyokr.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3aputddgp.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3mpehrlab.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3hbaopgse.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3dpgwdqhc.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3ugafggkj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3upqbjfui.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3ipfoakzf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3spahvopb.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3osdiiuex.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3qruklwkz.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3cabqmkys.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3fzmvnahr.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3hrxfiauo.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3wnqyljig.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3gmwbfmip.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3iiisfhsz.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3xolmcvmo.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3lnoinzlx.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3olxulcrh.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3rtwbttxm.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3zjxnjjhl.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3ftpdszph.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3wcurtvar.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3qyvmisvy.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3pwftoqxg.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3ablhckku.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3yegsxjev.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3rbuxqhed.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3glurhoxt.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3wotosgbz.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ftsjgotj.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3evhizudz.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3bjpjrbhc.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3pesyqqix.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3etmowsar.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3fcizorec.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3pogrvljx.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3hevmdvyh.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3ubpupbdu.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3vyjklknv.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3bgkmgvbr.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3vofjtalm.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3clefjaff.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3oykauvnj.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3sklsxfge.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3uanzioze.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3esrwzzjo.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3fthyjzie.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3bpgnsiop.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3cgjuxtag.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3txkoknks.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3ferlxewn.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3umithkjx.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3lwvgfziu.html


<!-- 参考信息 -->