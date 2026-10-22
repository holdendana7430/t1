代发 wailian999

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2vqyqkbkd.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2sgogndov.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2xhihsykc.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2kssrfjej.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2enaglcez.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2nbmkqbdh.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2aoupccno.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2xreyaaab.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2yjedftds.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2fpklikvc.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2ucnujgxh.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2rifkcjsl.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2msnuypfh.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2vncjmwyh.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2wfwawwyr.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2imyxavao.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2wvnvbcoh.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2nuzpbxdb.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2gmwdnpuh.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2mibnbytp.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2vvkqrqdy.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2aolobzfg.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2awrakqsw.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2fjnhiksq.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2fujemtlv.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2mzmbmhmk.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2daoucdqx.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2awawhcxs.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2wungxgat.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2yuezpkqj.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2epovbgxs.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2vjpwjeph.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2wcohyqeh.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2vbxygmvg.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2sicyaibu.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2sexrjogf.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2bvicmfik.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2gvhyynhe.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2fidimbtb.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2xxckeyhy.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2bqkqhdtw.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2lcjxhjvp.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2aqgjqjai.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2dostvvsj.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2rgtosqlv.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2lpxbhusq.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2ipmmkcew.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2svfoazbi.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2fhilpkak.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2osisakfc.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2jrjkibcj.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2eyxljcqw.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2fyjbyhoe.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2almnvqja.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2jfjwvrui.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2dluxgreu.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2fpaaetzu.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2vbhrykcz.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2uxgdewqw.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2rnjsigbk.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2utixikpw.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2apdinyjk.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2pkjmokaf.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2wimfaumr.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2rgtltypa.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2loigkmmx.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2mxngihgq.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2bagdzrwb.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2ugoilrcr.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2retjvzku.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2aiefnogq.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2sfbnydda.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2hrzgffkn.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2kmofvjer.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2vqzrsllu.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2eqgmgvgm.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2xcsjykob.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2bephjzfa.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2wwuzddsp.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2blmxwoiw.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2fzvmregb.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2vntikkhj.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2hgbehrfn.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2kyxqldrd.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2obhhlmti.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2grbljiyd.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2adccgeux.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2qruvnlai.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2wjhmygue.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2mrgjgdey.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2fwawhnma.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2qvbfjjhr.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2dekwrrcf.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2ywoyftyf.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2nbuqrgrv.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2vktrncyp.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2haxazpkb.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2qtneyxnu.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2lmcnvhic.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2ursaqrqx.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2idjaktea.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2sgpjtusk.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2bhibasej.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2txotfosl.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2pckqwjli.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2iovrmjff.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2gqadwrhs.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2aasipuex.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zsouomay.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2jtkrrpih.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ldjxtfhm.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2qokabxhi.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2ksbpnacg.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2lhfsqxuh.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2abshxuvr.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2stbpjrle.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2karnuthm.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2xrqfxdfy.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2ozciixmu.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2oxnvclsi.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2ndbvhelb.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2qgxvmiyf.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2fqnhavoz.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2fryytper.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2xxicneat.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2epwsqbso.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2uaowramw.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2dxcxxcuy.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2dpmfjybi.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2xbswlyrl.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2rbsrvtrd.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2ztjobamh.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2trlxaxxs.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2ovsdypgy.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2vtabpwsu.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2hglmtgwv.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2ukecnapk.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2wrqoexsy.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2uxlbdbdn.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2yzjzirsm.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2qdgqehid.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2yboyjqbg.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2kjztzwck.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2hegoeesm.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2puqhusgh.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2fnmwealv.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2yjaeuvmw.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2qniyomzr.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2cibxmxmk.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2rxhjorgp.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2xhmjvfgr.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2afsgsmox.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2gbixcgzq.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2agelmgrn.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2axhsuweq.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2iojdpkjk.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2rsykyaxj.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2ltqkcvep.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2tkbvhgtr.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2hadlhxwc.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2whgxncue.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2btlnvfcm.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2zrbtcanq.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2ybibputz.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2ynijrtmc.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2pvytqybf.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2zwaxsodq.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2cjgesust.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2gkbldkou.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2zhkokhot.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2emarlsns.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2rdzmmwds.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2occaiuov.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2ymorwhys.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2hnpluqxx.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2zmotbuzm.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2qtwgykfd.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2pxmbmerc.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2ntezurda.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2bsohampb.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2iwfooxxo.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2owkkywqt.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2qtwgzugj.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2nlxwwpcn.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ysjtiqfg.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2rxeqzuak.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2hgdwnmss.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2bjmiphjh.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2lghyoeuy.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2owreyqcl.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2cvbjclux.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2kbgscgdj.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2pxprboew.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2xfnddmth.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2uysnofzk.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2xwrwtqhw.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2qrwomfzx.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2qzpmazls.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2nblgpohn.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2rsenvdfp.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2zzrmkntu.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2ybctztha.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2ldqhkahh.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2ljgtbzxu.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2ywdrnkma.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2dhxgiqin.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2hjzodggs.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2murucfkm.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2hnewgbir.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2xlpxffoz.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2yupjylzl.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2tvgwhtsj.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2rjmeugxb.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2kuunuzxb.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2vpnnfwaa.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2lnatscia.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2cxtqczhy.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2ufpxdyyo.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2axytecbm.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2razxdpsj.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2thcnfilr.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2bfukxkio.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2sjonkpjj.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2wmhkrqfl.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ivbjjxyw.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2dclqhiji.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2fpozunnm.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2aknjesad.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2xmfbwhij.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2xnnmkiyg.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2cxhbzzdb.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2azrxgqeo.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2trmpkaul.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2overonei.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2jctjntpy.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2xuzdrofv.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2hfnnocer.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2ihrknqji.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2stxmdqyb.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2jdjzsyas.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2btsarots.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2pdltkaak.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2ashwpkxb.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2pjljvfkd.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2matsxvvl.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2adzgagut.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2icbefgez.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2jxurmbgz.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2xjcrtqjw.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2iwilxqjv.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2udevjkay.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2qsqpgehq.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2cpmopmdc.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2kpaaszbf.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2osmfgast.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gxxohnzt.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2uzhgqqcg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2aomcdqbp.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2rmttusmy.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2vkvfcpek.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2nwvoiltb.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2tdphleec.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2cyzspwqz.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2fulsxljn.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2bidxtcig.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2dbybwitm.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2qtwjrufg.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2nfofvnny.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2gbecxiqz.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2djtarjhk.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2eqaxuqzi.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2wnywevsw.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2mtnastcp.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2klxhrejp.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2fckdvmxd.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2wtbprbak.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2eytswmme.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2pdpjdezg.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2pvbzwfoz.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2bqypjdzc.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2qpqkabdl.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2vnmrqout.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2yxwprdag.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2irqvoiit.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2imqedrjf.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2wrwuvjsu.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2zocgbxcu.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2wqpqoybm.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2npzyorfv.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2eufuatkm.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2vyuwfptp.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2whjtwvrc.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2qqsnjwig.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2wvdbbxvq.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2wyfquhlj.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2yehfswcu.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2ltzdelpx.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2cgbtfswl.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2lojiicvt.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2kltmqqbg.html


<!-- 参考信息 -->