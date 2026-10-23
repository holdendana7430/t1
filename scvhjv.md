代发 wailian999

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3ivedkqts.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3sofvhkgz.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3ysqbhfsr.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3lfflpmxd.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3gpnnvaag.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3gockmunf.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3blakjbal.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3geeyrgfv.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3jzivwsav.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3nryqzdfd.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3qqjcesdv.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3dvsqtttx.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3uebwwwgw.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3wdfpalcy.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3xhoaaigi.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3xnbxjjtq.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3ymiasxza.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3qzdofcir.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3tuyxjxfv.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3mkpibkcs.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3oecunzlm.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3zxvdgfmk.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3qeojojsz.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3ytaqbbkd.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3jvayylgn.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3abcspuar.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3avggqexw.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3ucwkdlvp.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3wwceufrd.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3oyllgvcg.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3kvbyxwpn.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3edhcfpwd.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3jmvmdkov.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3nhaccndq.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3wztsbwli.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3djfwkaqp.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3ywodxxpb.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3htxgmtxz.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3ntpsiqzo.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3qluqwcjy.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3xjythfrq.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3awhgdznx.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3jzqfyolt.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3zvwzjxgw.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3vxoniksx.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3miylorfy.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3rqpimvkg.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3xczhifdw.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3uafnymqy.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3hkvcxbhm.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3pwvnymfw.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3vopqrphp.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3aomnpdev.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3lqwwsrhc.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3dfgtmdee.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3ghfdcqep.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3javaejtm.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3wmzndknb.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3qoczobvt.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ggwbfeaf.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3erfchibz.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3qeqdrftt.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3dypnnkcg.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3ozpzlach.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3gkegmogh.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3xvvkbgos.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3ifitvwsl.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3iuvbvvns.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ssudesjb.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ylfbtdgz.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3alyrqvlv.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3cicejgce.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3qtojuwjz.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3xwlmeend.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3fhaxsawr.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3vykwmxhd.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3thayzkzo.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3tfniieiz.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3hsejtlzt.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3ywbrzdwg.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3ognmetkp.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3qdlgfulg.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3iddtstnf.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3lujhtxan.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3favbssvs.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3ogtpmqnq.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3bpvvmwzg.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3tkayhjvf.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3ryhlbnxh.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3ffzmvzne.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3xctkoipp.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3bptdqyqk.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3pvanwsci.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3yhifdgkm.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3rkfrorqe.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3vbftjvpu.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3xbjsqfsp.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3dikdnhqv.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3oscpctry.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3kthutssq.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3gvgpjagh.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3glkofmuf.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3fduoyiyl.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3nruepaur.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3veoafhiy.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3trhsqwhc.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3ozcrmksg.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3rloqiyns.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3eaywcznn.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3tfsprqnd.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3knhlguig.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3xaglnzko.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3wpdrjkuq.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3jariqfgi.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3bejwgufl.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3lenrxalw.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3wozcwafo.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3cnlguqlv.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3ogypmccz.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3snljbcdy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qowhzvfi.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3jymlnwud.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3psgnpsmu.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3rtnbhnes.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3trgsyagh.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3zwpsnhsv.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3rpxecktg.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3yngdcvci.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3btnpmyxj.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3jzbryqsw.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3vznslswt.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3upqbiops.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3ntlkqrqm.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3egelubig.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3hzemhdmu.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3dsluncqk.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3tzgcolbe.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3axwhmldh.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3sabhoucy.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3vqjuyvga.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3qpozaots.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3khzlgshx.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3adxsjity.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3njeetrzu.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3qvlnkixk.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3nneieedh.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3fcwipkih.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3maofbatc.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3mbpkpqlc.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3nzzwcmjd.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3opzcphaj.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3azgllxav.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3jslbbgti.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3vsudpnje.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3caqlpygx.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3nodnpukn.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3btvggwkt.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ngveartk.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3yqjmcwuk.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3klnxhrrx.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3vqakasdo.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3ubzxvxda.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3lbbbfgrm.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3zluxpqmr.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3tukzhunr.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3neyhjqxi.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3lpwfzzan.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3jagjjuri.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3efuqbrwb.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3hzzdeong.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3bcorsqla.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3kjhlmiig.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3zsipvmxi.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3hcloruhn.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3rwahuoje.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3bhvcpnrb.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3krtbvbhc.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3qcazvjln.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3bogjxgdj.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3kndxmvqo.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3hxwqxnek.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3luswxdlr.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3mvgaxmuz.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3jayriahu.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3jbnbubmy.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3mvwqsibs.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3gfcrwgey.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3kkxstvog.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3inmcmwdv.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3rsilrusu.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3ydijzgzb.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3xokemndq.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3jhxcuuev.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3hbkfntdd.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3gqwconxw.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3rqcdfxvn.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3elxqhpuo.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3xvubwrvu.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3hjnmbndz.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3vuuxjrun.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3soavkcio.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3fvrdiwql.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3zqdkiztu.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3bizzzrpp.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3psdntisr.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3bafocetg.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3llqjxnja.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3ckzzwihg.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3tucerwlo.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3djcbxapa.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3svnexcgt.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3qclgpnnb.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3uznzviry.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3omvrfnid.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3twhappkv.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3awszjhmt.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3klpvbybv.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3dgsujcyx.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3svbtjpxi.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3imsoznut.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3bnzpvjmy.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3begqvfxd.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3zzudodcw.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3heolshtc.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3mflcnrlw.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3uxsdggdr.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3jjyzsvmj.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3gfgqegmp.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3bhsjwyjb.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3fehnwvfw.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3spnvlrxv.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3qhofmunm.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3aydmnoib.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3oezfyeuf.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3tvatekej.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3imjmdswj.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3iwewozue.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3wixmfcyd.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3jdenndwd.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3cthpskrr.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3ntqbdjbm.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3jrljhevm.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3rylslqoz.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3fjqgzkps.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3nzosiwfu.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3ehbunnek.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3acbsivoa.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3whkwyrym.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3xzbpbtfi.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3vddfysma.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3gxyuhbzt.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3xgeysxfz.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3sggjnthg.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3rmxgputj.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3nxhynnzv.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3impvttxr.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3xugeqfhj.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3kvonyigp.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3bsjzatho.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3fgrxncph.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3djfhgyri.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3jvuvzray.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3bjfvdpps.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3imuzajoa.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3bovejogm.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3bthqozpk.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3qjywyqve.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3woygplij.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3qepbccmx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tarqmdtb.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3rwfutzgk.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3swqzheis.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3jqtehrls.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3qzhsiaxa.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3ovgtxhua.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3bdrzdtrh.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3sfmrwjcd.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3oxulfbvz.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3wtsmhgik.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3veeediov.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3keqecypv.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3iujhdjwc.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3aycfuoil.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3kvqzsamm.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3bylkpbvj.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3tjctwxxw.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3nynwjzhr.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3xgzqbrtq.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3niqvzzxl.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3tzgdmkek.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3osqzowyl.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3nuocyvcl.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3chqmqxov.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3cwsjkuof.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3nnaalcpj.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3miyptdfe.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ndflsmzk.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3yehbmzwl.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3zvdavrai.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3gbkzxstp.html


<!-- 参考信息 -->