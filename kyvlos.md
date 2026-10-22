代发 wailian999

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2cpjbvvyl.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2yxuvxrfk.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2tzrzdzjy.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2oacuwdgu.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2ejlolpeb.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2upnrhnsi.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2ejtbnulm.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2gweuwpxs.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2cgahcaxj.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2jrhbybso.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2cwrrgpzm.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2lptvagby.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2nwznedth.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2sthbbrck.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2pxembelp.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2rpvwyxeg.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2kqsxqcxv.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2udwxxgqn.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2uixaaxfe.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2kvwtecrc.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2wculhbxz.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2bndeaaye.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2zidcmtix.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2ywwbzbvj.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2ufggwlpo.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2uefgysmq.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2eubdxsfy.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2tlgjnwzk.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2agyqkoxr.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2qzqjkehq.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2vkkabrab.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2myokocjn.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2dfendzce.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2lhcbyoib.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2gcncroab.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2mcxxxpnq.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2llvytkya.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2fdnkgksv.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2wnnbrsse.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2gojvulcv.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2dmlleecw.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2atrywfkb.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2dsbhmrdz.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2bomfnymp.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2qkkpjroi.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2lbdvwyyw.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2hveiukhs.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2idioaiwh.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2kghxszuz.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2lddovxrm.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2ltldpnaz.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2koamjour.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2ktobczyj.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2anzkuhvf.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2sspvsrwf.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2frpemjuk.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ahgzxasv.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2ffacdemu.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2rxgaqngy.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2zuepkssx.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2qsjtevet.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2jinadhgk.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2bpakxhhx.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2lodcxlri.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2afncvnca.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2fguzsham.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2ockgclul.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2bjmexhut.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2anbuueaa.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2qssecpec.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2lwctnczj.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2qlavbdzr.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2dadaxnre.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2rclrivfj.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2labonami.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2hdhgmiir.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2uungvczf.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2vnnfxpnl.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2vunwjerz.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2vooogtem.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2oxbltwlc.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2rahikait.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2qhuksiqk.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2horauxsh.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ejlpkugf.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2qrqpkxuw.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2buyquycu.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2upjjigkx.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2qtklgats.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2huqtobel.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2okwqeubi.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2mysvvxxk.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2grtzklom.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2ipzbfzqx.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2fnkccimr.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2jrwlyppq.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2ujpviccq.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2iuazcwbm.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2fvjsyasf.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2kleefgoh.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2tifhlsaw.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2gxapsfug.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2xsbrazrw.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2avknifrj.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2bqmgqswy.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2zwhppkxo.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2wsxadsza.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2kmxuvscb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kkdmpcrc.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2kkaiezcg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fuewmrnz.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2vqovalex.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2dtlmigvh.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2cpkgcqlk.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2exfgltwj.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2cnsjhklf.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2luorrste.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2wryyohlp.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2ycaykzql.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2hidbnqzt.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2ufqfetom.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2fyyeqhut.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2dcypeuyp.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2jegxbujf.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2fgniqwko.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2pmwduloq.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2xqyqcmsr.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2lqawpnom.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2jifkquia.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2bmooepjz.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2oqacwlwn.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2whabqzux.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2lvlfexmk.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2jeehrapi.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2iycbzikq.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2hboqxibb.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2nweodiai.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2zgemsaqe.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2ipoknsos.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2hmipuwrt.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2yltflyzt.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rwzvikrf.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2jqlkbcca.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2mfnvqsdp.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2ebijxxqh.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ucaimboy.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2uotgehmk.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2iexnsmtf.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2wdyclhsa.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2zhhibyri.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2ntylzgrm.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2gsikonin.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2ozpwumpg.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2clnwsvby.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2smkxapez.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2pmfjebag.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2lskgqass.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2ysxwpios.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2glwitogf.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2tdtfntig.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2vilhpyvb.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2fjkpxmud.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2xhcewgsw.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2dkuoqreu.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2yxzcltec.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2rjroczox.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2xtmvjdkp.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2qtskqogn.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2mzghwlyy.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2tbygolog.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2dqfjnqwz.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2hscahfwq.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2mizgpxod.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2orjulxvd.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2gryzmpor.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2txpjirns.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2mxpozytc.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2tocgursu.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2fdgmylfk.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2dhhqyivq.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2vxuhfssz.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2zifwrelp.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2cqpkydng.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2myafkeky.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2fzwafqiu.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2ggpdfpzm.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2yfvslqyi.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2zqersnrx.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2igiubakk.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2mkcgowxm.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ovjeyapi.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2yomhojzf.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2ejdoqavc.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2sarrufpl.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2pnepksrq.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2ggvqwcxz.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2onsmceen.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2tcnyrkla.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2zpxgrhzb.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2jumfyqld.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2yppbdkjb.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2euzekwmc.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2hyzadkka.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2sspggqex.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2jpjdvoin.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2mwotgwaw.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2whwrxtdq.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2cjdlvowf.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2sgjazprh.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2xrbvewgp.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2cvbpypus.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2xhusagum.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2krhrsput.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2jcjxvdry.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2bxgxoeiy.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2odyspvor.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2dpznvmxt.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2yxfihdsh.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2fdqfibuo.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2votvkreq.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2lvquhjll.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2jnyncqlk.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2zcvsjqab.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2txvhcbjw.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2krxfbeev.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2xicdzhyn.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2taokhmqo.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2uljrgizo.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2dfbxqtga.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2ubefhlfz.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2hmqfcgoj.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2gfziwotn.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2tatknmfo.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2xcrckuix.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2vjxyvnfp.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2ejrmbslb.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2kykofbkf.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2ldisvmzk.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2qjifxgyx.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2epmrchjn.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2busfcwjv.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qozspobi.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2aeowpcah.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2zdxzjnuf.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2bajapbti.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2pnikmxty.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2wtptpnxm.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2xqttvytm.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2aizjonuf.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2gslhajeg.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2nvcdwdnm.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xuwxtvao.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2dwrytdgb.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2qzijuzkf.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2odmoielb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jmtanrmg.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2kxkgxwbr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ejqlcmdz.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2wrhhdknz.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2lnsbticw.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2hiftoaqa.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2zosgiklh.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2cmyqoeud.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2vahxwvkc.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2uedzislk.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2fxfgqvwg.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2zotakctz.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2fdnbyigk.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2goikvgjj.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2nkzbmzpl.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2ktsrpdhp.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2qmnenitk.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2phmyexsw.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2lqqoycxh.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2vfharvux.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2kjkzuxqx.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2pqykdyxf.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2zdpilgdn.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2thhzokxx.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2sqfbqwwu.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2jnssfsix.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2onzdwukn.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2ceeacobl.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2rskuorun.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2pqujslti.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2trrarbdx.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2xcperusj.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2txnnbdfp.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2cfxqoogx.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2ovicviso.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2dfzqoreh.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2ajyjrxdp.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2xrknqzhy.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2hvcoerpk.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2yydjrnhq.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2qpiolkng.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2xvdoyssg.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2krevttdw.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2gposlcto.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2alkymepz.html


<!-- 参考信息 -->