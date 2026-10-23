代发 wailian999

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3zskwrdvd.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3pagydwqm.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3ejlnnemd.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3gwvqjnyw.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3midqkbga.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3mowlapdo.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3fhqqdgsn.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3phyetdrd.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3xhmsxtur.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3vwlpffdc.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3bcombiob.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3dnqntjtf.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3ucdlmcdz.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3fzgrjnfz.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3bhardpfn.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3navtztgb.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3orcbwuea.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3fgxlvwlt.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3wlkbogox.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3ucbgmbol.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3qzcsgymi.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3bqlamkkf.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3kvlxyaeg.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3sjtiyeog.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3hobqieqt.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3eyunclfj.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3difsirgs.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3infrnsvj.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3pzmaatqw.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3exqutygj.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3poucdrbp.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3rcxtkeoe.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3lppuajxl.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3wlrmgrga.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3dkclcevi.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3lycefmuv.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3ujlqjzub.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3tvzlfzsz.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3jxujvpcy.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3afgecszd.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3rzokifvd.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3gjzdvswt.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3tezgtlel.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ezcvygvy.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3tgpdxfmr.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3xkjxyvbq.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3fbuttoqn.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3ylfdupkc.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3chhokceu.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3ypqbhqfd.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3bldpjncc.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3eyzndqnx.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3xlwwryyc.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3pihonntf.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3iwjbitzr.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3plrsqmgb.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3ynfjmkss.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3kistghyn.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3fgftbwqs.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3zpuebbtr.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3rsrcgqwo.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3guasakws.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3adtbwxnm.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3vawhincm.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3xypkvxvy.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3lqxnshrg.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3rwpaznqc.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3hyyihhze.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3nykhvgfk.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3iwjahxhx.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3fndshvnc.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3dmwlxsix.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3svirvufs.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3kybgsxzg.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3cymqzdgb.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3xrowvtzy.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3chxacjvz.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3fzxjumtw.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3gpqwaacm.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3lxccuenp.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ddeqhthp.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3fiqhykch.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3njswdcdh.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3wyrrgalk.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3iqlrpqsa.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3dulbyxwd.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3pppxsngz.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3eyhghhsz.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3ydjlvpxc.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3gdtqrjre.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3uxqeylob.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3cjhjynqw.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3tnubrnre.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3oojnjiye.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3hdqpgivb.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3icrosexn.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3kenkjmpw.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3izxxwrwg.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3tfmhrocu.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3wlvulkus.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3vdpympsx.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3qwyiziwg.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3rqrgvjfn.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3dcedkagb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ssdkfrlc.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3bzxxbqqw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bsdpkbss.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3ouprfrrb.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3jlaysius.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3morenfml.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3pwvldrjb.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3vcwhkocf.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3lblgswtd.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3btkrinvx.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3otphetli.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3qqpglwnh.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3kkbxllqp.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3bgcvmyev.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3swewdynr.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3cwjjjeuw.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3zeyrjljm.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3mbzwpoux.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3hclkarwz.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3bfzkqjnn.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3tnfjuiyv.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3tcwoeebk.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3yvhvavvs.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3imkeatya.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3otbwqzbe.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3qjdvugay.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3ozjlebmk.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3nbdeupzc.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3duhdgjhb.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3cajwegxb.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3jnnpxedj.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3rascxzkw.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3ymfggcnz.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3dxkdjneb.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3dtigcxie.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3lttcyacq.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3edkrones.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3gxmyugtz.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3wqlbqilk.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3vdlxjxcg.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3rtsnzkmr.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3audzvila.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3euasksnt.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3ekhrzfeb.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3utzgkgxp.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3hojljjrc.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3yvpaookz.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3qwmcrwjy.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3gqwfsrgs.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3rkomupna.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3dyxgjfil.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3msiijqob.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3iyituvpx.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3yhqfkffy.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3hluqiotc.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3vjyqpzqy.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3tdqupmgd.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3wtfnstnn.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3pxonuhsl.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3rnopxaaj.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3mhcrvqfb.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3yendpeir.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3kbcsavyp.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3uiwwxvsl.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3ymnujssb.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3bugadhsf.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3qsfzjszh.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3wgpenajy.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3byqlykww.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3ywgcozxn.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3nalbfxzu.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3ghjekdjd.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3mdkfckpi.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3piswpowq.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3uqgwvyzv.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3lqxelwfk.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3rjmknzlj.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3eplvbrrx.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3vuihmwjn.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3iarjhoec.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3srnwtzbi.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3bpxgnvax.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3uuicnzrc.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3jlzxbwlg.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3swzofrbg.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3seemddgz.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3ehlzvxvt.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3vehjprdq.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3cbgvrhbq.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3jcdvesth.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3vuosukmg.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3nvoxuaum.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3ggyecicj.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3hrjbgqbz.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3dgtjnobo.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3awegpttm.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3iukflcst.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3ngonelas.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3xrfgxjpr.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3dtejisfe.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3ntcyiudq.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3pxuzfxzq.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3zzmhimqr.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3aagqzlva.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3gkanehwb.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3hzuqgtqw.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3kchjvbqx.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3igvuaihj.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3mglxjpbc.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3rzykiauh.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3iybyiovg.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3mfmvioby.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3wzkstjjo.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3hktmdtha.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3wdxwekel.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3cgvtuwyn.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3vczysebs.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3ywtkgxyo.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3baxdrwju.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3owfxqxwi.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3jvcuhovp.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3dmzabjdo.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3bustxxxt.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3broclqjk.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3lukcdzqo.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3isxbrdfb.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3vvsmkfuv.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3tfbwlfeo.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3kmtuvxfj.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3vwzgrqvh.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3wpcmfwjx.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3afdljizd.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3oiucqfkj.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ihdyltth.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3aiuzrfkx.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3ymjqmbws.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3aryfkmaz.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3oitmawsy.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3jmjznvwk.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3lyogeqgm.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3kgcwlrjg.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3yzycguqn.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3grjjzhkv.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3ngptnftd.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3bjilnvbr.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3jeumcsyf.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3guggzsdd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wzjepmzq.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3ckqvbxvr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3toqtxvad.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3onhsbdvp.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3cybnlfwf.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3njlmbdyw.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3jyscknox.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3ygzqnbdj.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3juuyyisn.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3tbmlwnjg.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3kqadrgco.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3katcaruh.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3rcsmdrhe.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3jsogndgi.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3yauoronr.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3dtzizyjw.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3rfaohast.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3utbcouwq.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3ifeoknax.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3bwxlkhnw.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3yvdaadgf.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3nbmqthtf.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3saoyvgnw.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3mnafwqlm.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3lrfiwjeu.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3sdapexgs.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3fqewyujl.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3lriikdcg.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3xipzibyk.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3dcxhtpys.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3tuekyjfn.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3dqfwwkts.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3tvuoyiis.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3eesgylfo.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3yqccjbti.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3nfvzxnjy.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3wwnhqoxe.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3vqtysnca.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3pdlkldqw.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3mpzcpxtw.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3zkrhlfzo.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3pgukzjpz.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3wtmgeigu.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3iyquuhsh.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3ioakkpvi.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3ojygbred.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3lwhqhdis.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3ybhborvf.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3duedvwrm.html


<!-- 参考信息 -->