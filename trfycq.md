代发 wailian999

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3ezsmkipy.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3wgpaxfbh.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3oqzjomvg.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3xhwpthbr.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3rxnkdfmp.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3cfbqhygr.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3qkehpdnk.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3eyipebmg.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3pzjuwfgw.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3ltdqqulq.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3vaucfypz.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3zrheycyy.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3gookipde.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3lntootvh.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3xsjekngc.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3cvarjquj.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3jiokpzua.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3zzmcdqig.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3oimnjclm.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3hgpiekcf.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3bwfvdssj.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3dfuisdwu.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3odcnfflr.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3nkgmhmrz.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3lgxnesfy.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3cscekibz.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3qwshbupk.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3ffaoeego.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3bqblcrcl.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3zfqfrkza.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3crmvpiuq.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3rqrsushi.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3vijgqxse.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3rcswisng.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3iqfzsdrr.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3mfyqqpgs.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3miwjpovy.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3kobcohff.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3uteaxeva.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3kdyemyps.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3sgvmzvul.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3uvsshemf.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3sxfzqvdm.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3axxubclz.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3mzvxprjy.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3tqlkalal.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3nnydsxes.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3avlpcdby.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3ufrcjcnn.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3kpgnwhpr.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3bbrqagfo.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3rvqmlgcy.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3aoukivtp.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3tiyewpzi.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3yujzlrqi.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3zmuellau.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ytmjnxcy.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3vvgmvpsc.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3aifhjgzh.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3krqudxno.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3ifluegza.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3nvqimhxw.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3nhiyuaqs.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3zbahyxfd.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3tsqcmkgs.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3hspazzgb.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3aqyghlfs.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3drpsywbo.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3dtcfgklp.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3tyqslmae.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3bjlkzjok.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3dughrsnc.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3tefnpnyb.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3ckevgrtm.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3fgodlsvb.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3hqsskkek.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3fyxdgjwh.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3ygoqvqrk.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3kwxyzsno.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3hhwzybbg.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3bgaqyevm.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3xdwrthmu.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3mzdnbaup.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3gdqtvkvm.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3bniuovhm.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3qccbdepz.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3zczvppoh.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3uezyhoxv.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3xglrppud.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3xbkptgno.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3slfzgvlz.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3ddviqxsv.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3kchradws.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3rribwubt.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3fthlvsel.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3bboaiyhp.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3ssmbegmo.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3wilwvwxp.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3hjgzmdyv.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3sbyqhkho.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3fagbrfsu.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3xuwxbbxq.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3sokassaw.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3nakohjmw.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3ixrwqdem.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3ohttcoxp.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3mfnmqmcn.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3zhcueqpb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gvqjdorq.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3kxkfgvxp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tidahcsi.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3jjbxtcfj.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3tniscess.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3ccohtoeh.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3yhdrbmaj.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3dnziwqdz.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3okdjkbyg.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3ycaaewdw.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3aduhltja.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3llgbbsts.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3xvyybmwf.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3cbbwotny.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3qlbhshnr.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3esebwlmm.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3ihfpvwvp.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3wwkfnjxh.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3jtbsbfnh.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3icajqwnm.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3twwojjor.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3zblwrots.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3bcnuheep.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3wlamxtrh.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3zvjkylxl.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3cawsgwfm.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3qqbvfusf.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3daucabvv.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3dxmpskun.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3supngyup.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3dtkrzjkk.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3mrlyhqfi.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3npigojry.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hsmnfpfk.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3igawovio.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3ydyftqjm.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3krokphrk.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3qgkrjela.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3vizotgts.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3uayzfvzh.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3gcuquusq.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3xbnmlwsg.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3uujqnmeo.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3znuashgp.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3kcezjlwb.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3gjdiokch.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3apiytmbh.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3ieuexyph.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3otaqkfgz.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3ihhxoinn.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3zecjnqtx.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3onsapqru.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3yedvmfpt.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3tgustfig.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3tksuobey.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3olnpitei.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3lzedragr.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3jxarbhji.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3pwdswulx.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3mqlaritp.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3qvauafcx.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3hgebzhvu.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3iyfdwutj.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3tguwctcn.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3sicimaqr.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3wexfelpf.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3apezyiyl.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3qpyfvych.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3oihdemiz.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3utqnnvzr.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3fsztxjry.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3uphviwwp.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3sfopflfc.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3ezaaqjgw.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3uylpidxq.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3fybcvvcy.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3sypvrudv.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3vamdvyce.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3vbtnmqqc.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3bphepxcp.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3zqknbgwu.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3ysgarddw.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3qpmbwpve.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3zowamsxp.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3hgvwvxtw.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3ytnaofqy.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3brlfnwbn.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3uaineolj.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3snuhtoeu.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3ojtarxxm.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3ftwhjvwv.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3azduelgy.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3ufnlazfn.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3syqeneup.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3ksxorkyo.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3hxkhgcuh.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3wturfthr.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3elgpmcnt.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3iyryavza.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3jmopfdor.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3smlxzntv.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3upthpxbk.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3gfauimgq.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3frxbqqut.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3nambszve.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3vfxjnznf.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3qjfydset.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3mulcqbxx.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3efnoiqkn.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3aooquhrx.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3feljqhph.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3nyvufdfm.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3tcneumtx.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3rlizfsrt.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3hqrlofum.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3xmlfjoaf.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3xfngqrvw.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3onblnfrl.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3ecwcnsnu.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3mnsjyfud.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3auhndnvn.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3prsbdzwt.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3kyjtoeof.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3rxshxegh.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3ytcmcmrz.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3ssovpdkj.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3ecuosthu.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3txbxlxyd.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3oovmhxay.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3kvphlzio.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3gehevfte.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3yuixthvs.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3omwycyhc.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3arrprsxq.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3kxummwgx.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3eqffiunc.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3ypniamwn.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3gbxobdhp.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3lssexhrf.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3wkjsuytk.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3xpvzlfxa.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3bqiqamsr.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3kjxmvnvq.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3acpainks.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3mwzxkere.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3umrcjzvt.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3qznaktxl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3huhxugqg.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3ciglrwth.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3oabbjayf.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3wzjedbde.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3olvhfetj.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3qgmohabo.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3yewuffao.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3vjxqwscc.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3dnubofxi.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3tfqpyodx.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3nhdmbver.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3hoexdotp.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3cbxnlypp.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3tczkljhy.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3uvmvsnhw.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3todqsryv.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3qacuinjk.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3yedlqpbr.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3uoszlevu.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3ingnwymv.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3btqauxag.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3lzkkhldl.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3kurywqjs.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3qkepvpco.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3esuanmsz.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3llvalucj.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3avsrybzy.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3czopyjzx.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3qoeypuai.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3smleiudj.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3dqghnsej.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3ykpnxbrd.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3pnhcwmcx.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3kijzvacy.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3jepdskym.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3qupsygsi.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3twwimkec.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3lceifbwl.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3jtpxuufc.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3xzovfjvo.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3rfcpblvl.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3ikxycjmc.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3iyidrwrd.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3nlgbcpth.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3vvnrzaoq.html


<!-- 参考信息 -->