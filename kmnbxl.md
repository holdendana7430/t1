代发 wailian999

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3pxzykccq.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3jtayokyq.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3dbzeqjrr.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3tzpmdjcd.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3qypmyofb.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3wnkajujm.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3udrxeqsd.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3evpzijhn.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3iotlrsyv.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3lrbmmgzu.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3qssnytrj.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3flhpjetz.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3hfnmhpyn.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3uleledtt.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3farwrrun.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3teeeglgn.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3ugyuwprt.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3cdlnhwou.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3zqgtmyxb.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3nykbdkgi.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3jsrmxkkt.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3chrkruov.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3sxqmhdpo.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3sxqjazug.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3buwqqdgg.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3hdbsqepw.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3dglduked.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3zeigthwi.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3zkxwzpbs.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3bxpbulzh.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3vfqhovpd.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3hsszijeq.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3yqeogsjx.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3mjmppcxs.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3llldmxhr.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3cjhwshhs.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3ryhbyiyn.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3oqwksddo.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3ttzstgpq.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3qdnrmxqm.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3fllepqpk.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3qhroqzfe.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3wxzlymzq.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3eudijjwp.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3lktmspdb.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3noirukop.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3iygclwqm.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3gmhmbuaq.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3ktunsvqx.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3agjnkxqh.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3oahjlzrl.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3xezpibqt.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3ofepveev.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3ueevofvk.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3ikokfncf.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3dwwceaid.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3vsejcuol.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3gnuinfhh.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3nzlwtprh.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3tdvpgagb.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3hxlbjach.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3cwsgeypj.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3nqsoximj.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3yzujsfag.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3vvqfuhkq.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3dqqnykjf.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3rtkabcnv.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3yjmdelxe.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3ykxfgopn.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3mfuvkrca.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3gqawxrln.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3cbtcwsnl.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3tspxtdbg.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3awdrkter.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3omzqkxsm.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3llgjnora.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3efnfpkee.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3gvzfhmrk.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3hzjgpocz.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3wcjrdmeb.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3abfmpyfj.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3cbjgbmfu.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3otvyqivy.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3vipimykf.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3rwxrsziy.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3tkqgmavo.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3xgbnwzkw.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3ujprbmel.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3cvrdxmjd.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3zbhylhyh.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3cisoxyvm.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ulqzwmfe.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3aktzfovy.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3efmabjnf.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3xlbbclzc.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3qssilvew.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3dlnakhtu.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3uniooydh.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3pmexwgro.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3zbmsfylc.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3axqmomqe.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3gvabtixl.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3dklantwa.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3cjroegxw.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3dixckbgv.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3qpkvtsei.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3johvtzmh.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3snmdsrqx.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3rimgxxxv.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3ryvxsgpw.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3lfzjmzol.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3noojfbhp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3khktxcna.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3gqhypugd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jeyfrhdj.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3sxupyhrv.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3vjjahmys.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ojtovtkn.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3apkjgzgd.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3txsbytjy.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3fvljvpzh.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3zewkssaw.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3gpwrsuut.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3kfyvvwhz.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3paytphlf.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3uckdhqjf.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3vjyxsurj.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3lbzloscu.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3ctwfvnql.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3ytbqadtb.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3dfkgxffa.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3wxoaocse.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3iyptmmuz.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3fyfhjkzb.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3rjgauonj.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3kbtvabrv.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3dyuvpirw.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3eqmjdaia.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3aurpgyqp.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3opwmjoed.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3hoagngnp.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3ewxyproa.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3qwyiyraz.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3spfprgrd.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3zlwafhwg.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3filatvfo.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3ttelrhki.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3ieguoznp.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3dgowafha.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3qcartefk.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3aflgijac.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3elvbzzsp.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3zlrqfuyh.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3zqckosvp.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3vbbxjpkg.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3mpcnuniy.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3wrjsbokc.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3icwjenzp.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3tzrsuvtb.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3inlkrlby.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3vgwstruh.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3igbxwbob.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3cvtpyuma.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3ailhpvgc.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3lrllfztv.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3ysrbuyxs.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3tpdjcupe.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3llvxrwrv.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3mqeblbjs.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3bdoijrfg.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3uhfnkira.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3ybkxvbsc.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3setuiidt.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3qybwsxnn.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3pgijeban.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3bzpvbtht.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3rmdpjzqv.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3dcznkqse.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3ojzuljfx.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3sydaakzy.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3qfdgqmvb.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3korfmofa.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3nzisbuis.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3dgalesmw.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3onrbgbba.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3jglydvxv.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3hdsrmiod.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3retpipgi.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3wvztqoxq.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3tqmfplqq.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3viazjhwd.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3kkloifmt.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3ppwgnsxq.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3ruvusuna.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3hqoxgjex.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3fkxxhkfj.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3essvmfka.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3mphnfbtr.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3rwxsuucd.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3fywxzmsb.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3okurcids.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3annqegse.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3cyggnkiz.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3dopnieqh.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3zbklodjj.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3xjcbmjbc.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3obsjjttl.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3iummbisp.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3ccgbjhiv.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3yyrrsbts.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3ctegflpm.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3nfopljof.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3qdcyfvqi.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3iramdfjm.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3yqkxglpn.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3xfhbtrqi.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3pyaikfam.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3tsamveyq.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3jzuxnvdl.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3jakuspfl.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3fvctpdar.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3bosqjapz.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3dbbpdwpw.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3hwbxgqvk.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3ihwhatkn.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3sncapjmh.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3egzsaqrb.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3rlwuuctb.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3ffijwtvx.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3dsbchqzd.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3xifxnyux.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3pydvabzw.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3cqtkgddx.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3laouslmu.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3oijvjmgh.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3klaqwvzg.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3smqnyqfo.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3mohryqtq.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3xvljtrhq.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3iidrpjtt.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3hpgcqhwu.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3jqvbagby.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3ptaswfhs.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3xwpebitx.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lgvhmrpo.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3gnzazaoq.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3bmeekvht.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3fsyqtsjp.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3mskgpqtx.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3jkwdjqet.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3ytlzurcq.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3wdcooibb.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3dqdfiyfe.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3zxxmxlvx.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3jidxcsgo.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rudwxfcl.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3arizdszb.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3nmxwuzwk.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3uhhkbvet.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xkmxszyx.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3vvrhdozr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zmnfdefj.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3zopechej.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3ykbwiqto.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3xikjmgld.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3ijijhnni.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3ahowsvyh.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3xvlkgfpi.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3trndmvod.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3hpdmnoty.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3vghprncx.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3uqxpjaxt.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3hpuocahw.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3rkpvdyyo.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3ezjxjkwd.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3mtpxeako.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3tmiboxhu.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3onfswacc.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3xbamzlro.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3jhslkumc.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3gtxheqgm.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3cnwyrufw.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3azookxwj.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3lkejboxc.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3kzppaoxn.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3pnlpheyx.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3wmecstaq.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3vuhicbqs.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3tcsyitlu.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3dbdlbroq.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3lrkiuaoy.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3qojebzuy.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3svfzqdvu.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3ictuqhbx.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3fwwfiwdh.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3uetjkisi.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3jtrfzgap.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3oqiklbpr.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3knrtdyvr.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3dafcdmsj.html


<!-- 参考信息 -->