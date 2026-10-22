代发 wailian999

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2gwqaycsn.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2ovokwxda.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2sukdcvhm.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2szyodlfa.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2pzfcuoht.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2qfzviqvz.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2lcbwveen.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2rmshuvng.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2ebheklvw.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2wrbuwmhm.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2sjmszigp.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2rcahifis.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2vivuxwmb.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2vjwuaoqi.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2gqjdoayx.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2tdfomrya.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2igikhelv.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2pidkklxo.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2qwgfovqa.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2ygypjhzp.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2dmmqjnzq.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2kxojxamm.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2ardthlqo.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2yhnkmjvg.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2ulztvqhg.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2ohrnbxid.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2xyndyixp.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2usfmlrke.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2lxgvyuxh.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2ajrcywgb.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2kfqgifvh.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2oqytiupb.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2mejewnfu.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2yieplpcn.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2yyhkhbec.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2qssnydfh.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2lqfmsacz.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2nyujlgoo.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2nqwtppkw.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2ljyxcbbt.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2oaxxaynt.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2kxaisimf.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2qkdwdvpm.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2cgwtqsjp.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2daqsvucm.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2biahqqjr.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2xetimqod.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2wyqgugvv.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2ipgrgwcd.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2ezdzcucj.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2ufagimww.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2fjqtsyeh.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2rkemigvt.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2jvcagjmq.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2ekeubuye.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2frlksesz.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2gyqalgqc.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2gcwhzwta.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2boawrera.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2xwdxxhav.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2hondpyzu.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2bfrmcfib.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2wfntxbet.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ynxjspmp.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2kpqcsgat.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2ufplushc.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2upcknmvr.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2xemkuoft.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2sxgaxyoc.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2parcnawk.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2zhbjkjlw.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2ejopjcjp.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2dvrxquwx.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2pwcjjpkq.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2brpuwtdy.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2ybqjcgdx.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2mtghrblr.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2sqxniqpn.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2jwvomgdo.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2udvsmkhb.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2cwnrdnbl.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2oxlweoyg.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2ntyidehn.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2hjlsubee.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2zxorxsam.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2gbnjxulc.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2ffwnospu.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2czrthtzj.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2qwmmfjtl.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2gjtxriip.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2rfehliip.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2dpxqmdda.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2fgwzqyrp.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2hdpwqxby.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2srdlyupx.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2dbczurtm.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2srdwlfnf.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2rvpszxhn.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2opfzokyy.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2fwnqwwub.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2npaxosui.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2fahcrynq.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2agvwdnkb.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2dbvlbzvm.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2umjhdjvc.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2khwffzdq.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2evrkyxmh.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2rkgskfvw.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2wyyczhdy.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2nmylvdkp.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2otxvbrvc.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2otupgpyw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qijszbrb.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2mwzmsigt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mrzfjjkc.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2whezftpz.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2sfqukdlo.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2jepkeudx.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2izvrjujv.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2yogtulbr.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2qvzxelsh.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2btvdhckc.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2tfsndyut.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2pxdzdkmv.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2tuncjctn.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2wadpiilu.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2agnanryo.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2cxsksxji.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2ocinvpfa.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2jkntsued.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2jqwuqulm.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2guavnptj.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2gulvqbrg.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2imsdwlyp.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2bokunkhi.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2iptramyl.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2xpzadjil.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2xwnljwqc.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2llxiaamk.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2gquikkqe.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2crrexjms.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2aiuvxwif.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2xkandrno.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2dfkwljgv.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2sqbklspy.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2qeyasgym.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2mcjveeoh.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2qxjtloay.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2lsasjgfl.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2xjmnjuoz.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2ouuyooje.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2boyybshl.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2dotocqtx.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2vsxinwdd.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2iizbabkp.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2xjajhzkl.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2bwxuxjuc.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2drfkgwmt.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2cernnwcz.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2txmizbtn.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2jcqiyhet.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2rjtwewgc.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2dxikmpvu.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2ppoyvgtd.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2dubbxrjy.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2fryoivrn.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2jtdvhjzf.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2ybnsckzj.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2qjfefppy.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2edkohszh.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2dbszzuoc.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2qasfdktp.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2zhsphyfr.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2ggxsnngg.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2uiroqowh.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2naohtbxv.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2bclkgunn.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2qxrtguvt.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2lehdycrt.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2diswjgkb.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2xgqtmgfb.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2izombpsn.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2vsgojjvq.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2hsiulaou.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2xuglbjfn.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2qkhcbvmb.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2vozzysda.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2ksqczbmb.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2dgdzcrml.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2vrffrpja.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2irriwlwz.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2zhoqtcsc.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2fcgihzfq.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2xftfdkyl.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2bjsafglf.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2iqacjctt.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2uxgnhchz.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2fmuzgwcd.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2otbaiahu.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2wmcnlqaf.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2hnqacdnw.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2tckrxqoj.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2dntfafqx.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2axpsbrmb.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2fslrypqk.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2ugfqrkli.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2rbqhstay.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2xxmskhun.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2eojihxpf.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2aiyckvmx.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2sbwsbyfp.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2ixghjffu.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2ckkbhiln.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2vcxuhacj.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2nmgdtjqt.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2kbekqihx.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2vamghbug.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2dwsbndlf.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2kzsxofde.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2arqbqskd.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2beqaqksb.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2dnmqwzra.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2eugntzzo.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2pgctbtux.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2mcxwwnsz.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2akkvznzi.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2tsshtzce.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2dbqxyvbh.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2bqruedwn.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2givyedpb.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2dsnlllut.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2ibrujdqs.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2mufjgvvm.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2lmwgshbz.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2ywzpjsei.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2wmqimmov.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2mefufcjp.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2flolbhcq.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2gfaikhew.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2xokuifxl.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2pbangrxf.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2ejyzwnde.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2zklrnsvf.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2ygyvmigp.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2vbklzzqu.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2jnusfnrb.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2ksojohzp.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2frvajbar.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2jlxzjevq.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2nbyhdzux.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2ficgccuo.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2naxhaxqv.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2arzhbjkq.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2tvxntwud.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2hovtvwxh.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2qgabpele.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2dtgytzny.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2ygviuaho.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vctljber.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bjdwziia.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2pvykeqay.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2akmhuvrg.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2jsmvfiyk.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2hbyxwkrb.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2ugjyoejg.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2lxcbpawq.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2dnjvjewl.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2dzpklbkf.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2kydnonbj.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2vimmxlmh.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2cxkljpkt.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2vayuogve.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2tqcaaqon.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2otdzssji.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2ibvkbdhi.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2xjxtuwns.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2pmbrzafr.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2jpojbrrf.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2hgxdnoja.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2sskvnocb.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2gtduuvjn.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2kkhvhsbf.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2hqqyszqv.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2qnqnyjwq.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2abcdtjdt.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2fcmhlang.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2qqvmuuvq.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2wgzdfbrc.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2tvtfdtxo.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2uczljywe.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2zogbwzil.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2uqqchvav.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2vcxaatay.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2hmlxidau.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2qweyotww.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2flbuvzcd.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2qteemygj.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2coxiqueb.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2ingheppt.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2fwtgicdl.html


<!-- 参考信息 -->