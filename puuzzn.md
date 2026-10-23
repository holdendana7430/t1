代发 wailian999

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3cjdmtete.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3kukrlxhr.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3lfqnrcdx.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3woyrgsix.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3eygzurdz.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3jrosyrkh.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3totabuoq.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3cfzogovw.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3mlfukfyt.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3goyyrqmv.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3lxustxrj.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3dccslait.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3mjrpfrrl.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3jxgszyyo.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3dfiegrgb.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3mxexzmel.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3hyspfaly.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3cgztdtpa.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3hrhopyza.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3lpxertme.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3rsyddcsa.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3ktybevbp.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3ngjtlbzn.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3tvpvvyyj.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3xwicohfc.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3retnupsi.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3tndrppoo.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3goedxghf.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3kdtxxocz.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3mnebsacv.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3gaqferyv.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3uhumjmbd.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3uvulkjsy.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3hlajflay.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3fvzqgdmb.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3zrbfdxwl.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3pkstqymk.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3czrbpuvv.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3csijuipt.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3jbkktyfj.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3uwjmorey.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3ejaqvlcg.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3heewcarj.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3uzmdeekm.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3tqfdllvz.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3ynjscfma.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3jggjcyed.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3faoqoqor.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3blgnokui.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3jtqecpfw.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3tclaihpf.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3vvoikpoa.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3hopgoxqf.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3gpruutvq.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3qqvdqfql.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3airalpca.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3msnlcqld.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3kbivhdvy.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3jozrvqpk.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3vtrpgyuz.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3kcjoywjt.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3vtonrczq.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3evxtqdcz.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3xopsstuy.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3fjqmfuuh.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3xelerqno.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3bdtvpnxi.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3wdyendmu.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3bapsipic.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3fofygkud.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3kzsrkbyh.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3reezbfoz.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3sbozxjcl.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3twbrlgps.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3ugxxwhsx.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3wnjmogbg.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3umwxfoai.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3fecbxzlh.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3wvaqyuxu.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3cuyhmjen.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3ttyuuyli.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3fhgeruse.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3ysqwkhhp.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3qkwvgevk.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ewiyyhtp.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3plbmxkas.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3vdabhngo.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3mrbjitct.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ordpuskm.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3xqnsdxkv.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3sietpoql.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3vtluhwav.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3xcuxaiaq.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3qsggzfkk.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3rzuoytkj.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3sizhtael.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3ythlalgd.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3ircxwfrg.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3emrscgia.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3avdrwhgw.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3ygmaurme.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3yprvrfhy.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3nxrzmxva.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3slupwnlz.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3cibpxryo.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3cyacohuu.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3fvrgcgcw.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3lzugvsvb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3onmvzdhh.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3ccezuinv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gljvpjph.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3ktydwzjq.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3vklgajfe.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3vpkqwopf.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3moyqqjqb.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3nsvoplip.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3lveabibe.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3qpplzjbg.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3irombjhu.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3amlaewxz.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3tzhjtkrr.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3akhxsaxp.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3wkrwdjgq.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3kddwdngz.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3fchmoupx.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3vdcsgytj.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3khpjfsmj.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3bakonmpi.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3douqffjj.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3sfcjsdan.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3lgycjcvf.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3nfugiqja.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3cleohuch.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3rsuqoxgq.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3mawevnqv.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3xphwhudi.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3zawkuusi.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3lbddqbma.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3zxlzuyqk.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3nbpckmba.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3urzizdth.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3qgjgmvlu.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3cyvipmbx.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3xbykopsw.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3mgvewizl.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3wozvfcyx.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3btwxcyud.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3htuwrtgk.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3hkjfsaug.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3lzmdpfbf.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3jbpekczp.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3nwpxzpcr.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3ofvmdqcq.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3vfcwkcpf.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3lirgwzpp.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3ioksbvhs.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3wpyapsoq.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3uceroipw.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3alqvgpeq.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3kfaewtwo.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3vvbidqvh.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3fnbzingu.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3qjkpluzp.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3xzedacls.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3ewsrriov.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3udafevmj.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3ccsjgkkt.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3pwlgojrt.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3ehetmxud.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3tgaozsqe.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3lgvfwpkz.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3thenrfpn.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3kljxsugx.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3fjhexkjj.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3xapdaenk.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3zvltslaw.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3xhcdtikg.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3epjyvvcb.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3sdhateuz.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3frphpgyp.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3unrsklql.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3kbkthzxp.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3jmcwfkyz.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3ikevfdyz.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3hwlomrye.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3zrgeuoyw.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3pmlxavxa.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3vtlnypxf.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3aixkgffd.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3yywmxokt.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3nptlwojz.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3dufxofba.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3vufpqvrf.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3sbwyyvlp.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3dhgcitqb.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3luurpsal.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3irhjmuod.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3wmrosjdm.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3weauiiya.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3hybsjwqj.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3cmmddxrv.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3gcvbjocg.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3suhivkbx.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3ommpuwwo.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3ayhbbdra.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3gyntnopb.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3rsghdoca.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3xnybqudv.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3kwvcsksh.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3jjzprhfo.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3qvauajlc.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3dtqgznfl.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3lkcsmadm.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3dwrjmwoi.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3noxgqbnp.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3vckekgrs.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3teesxsbk.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3adckoiat.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3xvomwthx.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3wnyljoxb.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3zowucwvl.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3tlqnapkz.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3wdlpughs.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3vhzedpff.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3hctyqmzk.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3peiihntx.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3kbiehehi.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3nmuoqrwe.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3djqqiejj.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3pwrribrw.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3fadkldmg.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3rjlafixf.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3asugucox.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3xejfcpky.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3ewmwluai.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3adpgydnb.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3oujkcbmm.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3hubbiloz.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3fsarnsvd.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3luhicepa.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3bniwskba.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3rposvwih.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3eoamjycz.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3swyhhtes.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3vgtvjwyn.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3nbimrnrs.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3wzgmfvez.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3qpvzrkah.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3nynzlsvr.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3mpxbtoid.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3yvdqdkxt.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3lxlbiczp.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3yukvanwt.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3ouuwpgqp.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3powsbodm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pheurmai.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3tvesluoc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3olugkgmv.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3krwdgdwy.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3jkfzuwgx.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3acukufoy.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3ucntlgxq.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3xyrewiaf.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3bjxvcdwn.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3wrycrabb.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3cvwatxtt.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3fpkipnuj.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3yhayjwjr.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3jwkealyr.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3szacwdib.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3ddwnkjmt.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3xbgtltgb.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3bfkaivap.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3qdhriyxi.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3mwqrjbov.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3fbgkcspr.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3gkpkxecb.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3pdentjbb.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3wehusuxa.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3wmqfnqcc.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3nmjizmct.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3fbjwqvym.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3kutqduva.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3tpdtvquc.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3vqayuuks.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3oequfjhe.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3nsbtlznh.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3bihyvaft.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3lahxavhk.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3tzzllfzs.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3kwmisgak.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3zxewrczr.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3rqiijdug.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3cfrrgdxd.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3gnveepkf.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3ljdplnqf.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3ormnltqp.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3jnzboenk.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3tszuxpjc.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3lhtzaowu.html


<!-- 参考信息 -->