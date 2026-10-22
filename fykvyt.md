代发 wailian999

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2mhznnffp.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2iqqpnkdk.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2kokjehhm.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2erymqgwo.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2msjcrioo.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2nbuuqvym.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2lssxuzxb.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2tmqnowno.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2kgyzuebu.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2krhjxrad.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2egaqwcdi.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2lbgxklid.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2ocindsvc.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2gfuwdhqi.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2shcoagvo.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2wkjsnowg.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2pblwktgq.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2zrppjerb.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2ekouowvp.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2hdepkqoa.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2eoawpdhj.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2wmlhjtts.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2pfawqgbb.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2msfipsyx.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2xkvoorqc.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2vlrnebtn.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2lnxmtacw.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2cnpkhirx.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2chtupgbh.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2vbnrfbri.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2pjcfjhvl.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2scbiopbs.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2rtudedxe.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2egduprzr.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2rabdlufs.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2ubwnexxi.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2pplioxfn.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2mlnsyszu.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2rmovokxb.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2mlvcmkws.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2xbxpcrkf.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2lbcksdar.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2cbcrlpvf.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2eqwatipp.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2ncvtpart.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2ywmbivod.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2hwwbmvdx.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2yodrbxvx.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2tmglivpn.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2hfswfsnf.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2mmpusuab.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2btqpukct.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2mzxhhkuv.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2wfgzbtmf.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2xwdbsvqh.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2brdvhwsn.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2jrdokuag.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2vlzspavw.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2dwgabunw.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2gcymhskq.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2qndmwpml.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2vmyguqdk.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2nbudjycn.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2wilyeewm.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2abpjuizt.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2zzfljpwd.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2xvwjfjrl.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2kvogengw.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2xnffwcbu.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2pxozhyel.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2stfwhcop.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2cdlskvdq.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2rwxwgzgc.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2cavbrxky.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2zynyuvrs.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2hutklpdq.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2urplhcas.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2aqpaerpk.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2jhkyixlx.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2liofhgdf.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2cxirweta.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2dfzbvosw.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2fjxnunxf.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2dkeizsyo.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2qlomvahc.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2pghjtlfn.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2bttbrloz.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2ttkletem.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2qmdxljje.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2pzdnvyil.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2oywwddxv.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2fscuoleg.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2kneuvjhs.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2vbyicwfz.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2ufpsjiap.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2rgbqnpnc.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2vfpjgakw.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2vckpaoob.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2zvrwgijc.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2njngisun.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2yhrqlnrr.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2jeknuzst.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2ckygywna.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2rjprlhre.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2ggurskra.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2vwemivkk.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2kimnjrcr.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2tumfqdhn.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2omhnpszy.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2xesclokq.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2giccucpj.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2mpnlhzih.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mxmgghog.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2dmocssrh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vrctpnvj.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2jhpxuhfi.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2emcxvyws.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2ldfbtjez.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2kbljgrff.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ahywqtzk.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2plwirdmw.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2pdgwkyal.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2znhhzpur.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2oakqetlf.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2wztwmvku.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2ekpmxqww.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2xtabadep.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2szvirxju.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2otwetuwu.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2vryuihid.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2ennkudhb.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2ayugjyrm.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2qyowxjbo.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2mztnipha.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2cczznjyg.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2uyjxclpk.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2sawsozzc.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2lizazjxg.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2fiolmimt.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2zgveunmp.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2ykpegdkd.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2tojsxcag.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2zpglwfdi.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2fjbxccwu.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2tbiwpygt.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wxdqcjva.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2bmtfaifq.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2wnivqqsu.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2zceatuog.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2tgpkzudl.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2bnntcwtn.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2cunebsaa.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2uauwzjed.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2yspsgapj.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2agauidkz.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2jqdnvurh.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2buncbwgq.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2ydjnottm.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2ersmfyxe.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2hzujcixs.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2xhzwkyem.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2gaxjzetv.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2vzwmclfi.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2mqpdyheq.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2xuhnpbig.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2tnddotne.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2vqszygbi.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2qfxygxun.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2tyfjaguq.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2bbcsdhvq.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2hslgacvk.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2wjuxynpl.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2hrqdovwz.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2orneubaj.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2faseipeg.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2uqkkayia.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2nehlnbos.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2ebmciuan.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2wxzimjhl.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2zinznltv.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2lmfusqic.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2hfffmvhd.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2wulaorht.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2gcbpasaa.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2evunleeg.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2afgekeri.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2kiarergz.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2lovisgzr.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2sisntuuw.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2bomvezaw.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2lkcxeiay.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2vxkumvve.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2ojybkoey.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2yrkkfnss.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2noqqfdve.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2htapdrkk.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2dckmualv.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2pkbcfbih.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2kxxbbusk.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2gvljupii.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2ulanifjw.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2bdkdoimf.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2nmxspfwa.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2zmgxxhzr.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2slhpdvwr.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2mdohsqyz.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2fwtdcpsj.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2uazqykxs.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2ghmmsixe.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2nayfqjli.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2zwrseitj.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2yghazbho.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2lqjintek.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2ypvcoenn.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2svtuywuz.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2bzzzulfi.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2jfevnvih.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2phpfxipg.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2jssutowt.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2gzhwqtiu.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2zryxtdsc.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2cfvdlmjb.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2pevwfdsv.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2pqvqqmxg.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2ohizezlp.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ziaazuba.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2ycgxxzre.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2lydvmpkt.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2zqgneuct.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2bpilajxy.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2njjauwfp.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2ixczdesi.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2jmfiuzee.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2kuoxhump.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2qthrbsdi.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2livsjbsp.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2xyfdqsns.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2easislam.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2wfiocsls.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2uaxrktrx.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2cstnwghm.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2imypsbpu.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2cfqhotem.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2awygkyki.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zjyzajzz.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xtsumnkl.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2tpwmefnc.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2axilzvra.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2vztoxyai.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2nurblsij.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2ahdbnvgk.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2mizhdrej.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2dsbbpwcm.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2efvocfwo.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2nucdadij.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hwmgeava.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2kdlqfpsx.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2prqhxoio.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2gzokbfst.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2agbarevu.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2qltxrbqq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2laocgnpl.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2gkezjbje.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2dxypucmz.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2yfjrtgwg.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2kutejles.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2wyfviuut.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2vkaiiuvq.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2mzhdmvyj.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2ahouxvxa.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2zwdbxxtu.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2usrpavcp.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2pzvgnddx.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2mglqreks.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2jynynafe.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2ewtoylna.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2bpmdmbzc.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2virtaydh.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2lgudcdgt.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2nlbuljmw.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2gmrwvyak.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2imfqsaxy.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2urebitpt.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2hmxhpxob.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2dabuzexe.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2mfyukhgz.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2slbobutf.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2rwxxabgx.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2tpcwojsa.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2mtrvmiaq.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2iufyffhr.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ovrirozp.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2rayxiwgt.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2hmmvtqbe.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2sutaekqb.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2wvwqwzyn.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2hfpcnnng.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2xivybebq.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2mxvburql.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2dbnmmwyh.html


<!-- 参考信息 -->