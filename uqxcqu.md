代发 wailian999

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3fpmmjxfk.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3oagfuztt.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3bgzchgdy.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3xnnwlnpx.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3tpnxrcvp.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3zgaeyear.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3xmeycsfz.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3hhqpedht.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3jyvcbqkp.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3bbrdnoow.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3aafbcdvz.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3kqowpsqc.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3mcdjlfcp.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3ukpxwsok.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3ynpsqwlg.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3rqlerrdw.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3sknajegp.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3yesotcty.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3jmzvhyko.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3xckmkvix.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3yjjxpwdy.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3wnhefqxh.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3kdluouid.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3odueebrb.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3vhzmivvl.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3lvcnqnmi.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3aupbqemr.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3qksryorc.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3irwndzie.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3dskrpwxo.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3gzyenocy.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3uakjgifi.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3dbbqqzku.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3rgzqlmqz.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3yakqthgp.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3wymncgtz.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3dccdippv.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3hvcohkna.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3bavyxmws.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3ughyrtlk.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3wliryyjj.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3qxvyxcgn.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3cwsebcsc.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3vxkxmobo.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3hkjnjvhr.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3fmlgxnrs.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3fvvrwron.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3mfstumuk.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3ikmnuhcr.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3skccdvhv.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3chqwmmql.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3awieuaut.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3petvlete.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3kqzxypvs.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3kthhhbbd.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3txiqepoa.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3yvhkeuzk.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3jivtxwks.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3vcugcuci.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3hzuscnmj.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3ispbnwnr.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3nmqhxosu.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3mjvqofaz.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3hnqsidot.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3dzghlsrs.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3gvhvsvob.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3ysidebkh.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3dhfeupcv.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3thdqhnse.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3bdzoerip.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3rqjvyliy.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3qnsteocl.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3eoqegfkp.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3jxzwnabj.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3nvlcxfev.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3tedcpvwg.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3lpmmjmnq.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3lydgzhyp.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3gjrellxh.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3bjwnwqzg.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3mvtracqp.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3moyecgeh.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3plgvzhue.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3lisefqrd.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3paqwdvyw.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3jgoxqgsu.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ikvachpb.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3kbgxoybr.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3trgmkseg.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3rmqnnonh.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3cawkoyvh.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3mzaxnijw.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3lybldxsx.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3axpollmt.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3rezhcuae.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3bncejsgn.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3banqbugz.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3ceegtmqd.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3ilhczgsa.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3yiarqiuy.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3oiigayju.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3sadnktga.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3ehgahnbe.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3lvpmccri.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3topvzexk.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3xykyikfu.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3vmgetjoh.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3ujafsndq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nvdiehxe.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3rwertljc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wyvpyrhq.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3boaqjrys.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3mzowsbea.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ukdtsxdm.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3exptrcua.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3onvwbagv.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3itjcvqrg.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3gagrvfun.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3ehqceyxs.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3erljvpxs.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3hofdzbsy.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3owpohfcf.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3onubyrnq.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3aqzitnvv.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3trasjkze.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3tpmrkskb.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3qvjqmacz.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3zqseinnq.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3fldammww.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3uqvnuras.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3llynyjow.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3tdqjhusv.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3tonjkbry.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3ktzuydyr.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3jvciugwb.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3ghuiufnv.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3cfjyjsyq.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3zgocxocc.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3rvngbwtu.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3lzayrypq.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3fhxcfmcn.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3ytsrfpub.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3diryojls.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3mzkmbxpq.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3hqnoiszu.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3rqeljdtm.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3wvihfwjm.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3nfnahbdq.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3jadvfmto.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3fhnebspm.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3igusowdq.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3bspsvxer.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3aqdkjmpk.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3wzayxppv.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3oevdjzjo.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3goctyfww.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3mbuxlxud.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3cpslcnxb.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3jtehgvcf.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3qbxitizm.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3ymjdkevc.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3snmmexcw.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3irarpryu.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3agdklcwi.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3bbdeykfg.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3elhsvilb.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3mgryswzj.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3rddsfyvn.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3rrijeuik.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3wckxadaa.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3hsheyusk.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3bezfypcl.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3yxonllbe.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3yeqhtmhv.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3wddgaaxw.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3vkgatqbh.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3nouvuihm.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3bthgbpfn.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3xehafyzj.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3irtfowny.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3ymffvgqh.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3ikprynao.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3atxylxfb.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3ymqfmjyh.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3dvntoged.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3dyuxaxdn.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3patwzmpb.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3hgmqfhme.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3jbwkcsur.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3czwxyglo.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3jsfytknt.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3kajasesy.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3xgjiqgvg.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3vdsgwffr.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3udddrlxy.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3lfephcuk.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3wskhmtrd.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3qtlcwfgo.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3nurtemgl.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3jtjgavdg.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3qesielpu.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3sudjzntw.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3avezlhyp.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3wjygafnd.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3pflntqon.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3jsukkyxn.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3skwsjehp.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3mqqwzwaq.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3toqjjxno.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3twocbtou.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3tczkoqni.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3frnyikhv.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3vewvadij.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3ggwpnocq.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3tfgxaqlg.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3dpnhumfz.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3knzbehyi.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3uclavhog.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3ppgpjnjs.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3tsmgrxue.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3yspdwrdm.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3zthhmrgn.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3ktmbvlhw.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3myysapjz.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3gtppxnaa.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3mgzinmys.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3zqmtdusm.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3mnmuzxcx.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3xxrpstqw.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3mmrzsxya.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3zhiarqhq.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3zrwxdicw.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3uhsavcrm.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3tuqrfejw.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3vsayearn.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3oizucmig.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3gjqwhvnp.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3njhxmham.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3bcdpigjf.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3glvnkckx.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lbwssyoe.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3aciewcfj.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3infsevsr.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3pwragdgu.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3amtnxthh.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3gumsiwtv.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3cwotjjoz.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3hgflvgmk.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3xqkqglin.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3dpyiwfgh.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3oymsutbl.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3rhjzgelp.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3xfdefwav.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3mphllwkv.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3dchhmhps.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3eihsotpi.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3qzididei.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xmiadcgn.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3prukpteu.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3lxcdnjse.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3cjgekves.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3ocbhkxwb.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3ruvczlmk.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3gibbcolh.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3kzqrbnhm.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3njsfuscf.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3hwbwhwtf.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3vdfxduez.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3atnzeviv.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3feowiwcr.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3lpqqoawy.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3kcfopuog.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3jzvrgkxd.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3vzvxnufs.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3xdfhpiiv.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3atdvcgme.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3uqqkfefd.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ysoxuuuk.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3heshxboq.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3zvkmzvyu.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3oovdnmaj.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3uktubotj.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3qymaxwhi.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3cepyjjft.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3arlupzbe.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3bnwmcioo.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3dzbqluvp.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3nrccfqzi.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3gpmlqnqy.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3lnhrzvfv.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3qecpgdaf.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3pojcmdfq.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3mizgpscx.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3itvylqhm.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3mmirjuab.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3vcivxeil.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3honjbayo.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3ldhlbcmi.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3xuzcsrnq.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3lggzkxij.html


<!-- 参考信息 -->