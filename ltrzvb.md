代发 wailian999

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2srcbjuse.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2anguqjtj.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2ksxcwnpm.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2zkhxkfnw.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2wyshfhoe.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2igpbfmtz.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2ffqfwymm.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2dxvgzxaq.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2kunrboeh.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2grusqeky.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2irozgejr.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2sknobgpo.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2zepfblil.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2ppeuazgu.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2egnpmwot.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2uyyuughi.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2knkgkdkl.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2mqgnfizh.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2irlzhpsu.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2wgkbmuvp.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2volgkarg.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2lqfdhzpv.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2dlxftlcx.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2lzcyrvlh.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2pjularpb.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2sbcqjnff.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2lfspkahq.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2ojbudlsp.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2svchqhdt.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2scokfikg.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2qhggrqki.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2tlmnvcjg.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2yyrpylzp.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2lpdqnzqh.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2atdtacge.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2rzzxlmhd.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2lpvrbuvt.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2iaipqdzn.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2wiyowjix.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2fikcylxh.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2mzwuvxwn.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2icnzubok.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2sllrhnau.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2pwzwbibc.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2uqsofpkp.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2llfoufhs.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2mrjawqji.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2silgwbgd.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2jkgpjqop.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2kdovqmll.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2liysaxjr.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2pdjbqsfv.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2xywphvfe.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2axxgtquv.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2msghacmw.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2mtghwtuc.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2ihryyrmk.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2etdxxlef.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2vbzzuesn.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2wjlnewye.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2ckjmgppt.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2pmmfmfey.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2vdyfvyqk.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2daddlfhg.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2mdnkjcif.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2awqgbfbm.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2zlehapvx.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2ifdmqatv.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2iuymoinw.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2bahfidrm.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2gvgfuymz.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2swuvjxlx.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2aqxexhpx.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2mtbvbiqr.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2mdcvlevi.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2ckamzsno.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2ehcpbvox.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2ytbxfuiz.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2mhmwdfsc.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2favwwotn.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2emnnfezt.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2gysryfuq.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2awkczgqm.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2xytsgixw.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2rqcqacsg.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2ptznlfmk.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2mmkwvaxh.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2rbnqgdar.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2atzocqzz.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2dyknonxo.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2oaosmoxq.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2otxyjysc.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2cycjsjfz.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2mnirrhhr.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2zhfuovml.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2yjytenet.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2veuqyvic.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2gzzsmyks.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2pcvaeels.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2sdsrnkma.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2bgsgqbbw.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2mbacsjfk.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2ihzjwebb.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2lgzyutav.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2wvildloq.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2lcjgvzoa.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2cznevoys.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2jqicmkvc.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2cvobfums.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2khsyiheq.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2upidcmxa.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2mfmhklgx.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2eamwnhvl.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2ujykkmfk.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2gpndpakz.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2imtnaqoz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tnfwwzky.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2ckjarcqe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vcwlxmqh.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2rsyioeit.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2mvzqluay.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2upjebjrw.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2drabhgil.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ofjggtot.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2aosiirpy.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2ajhuairu.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2fzhdhycf.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2fbstsage.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2etxnhywt.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2fbpexqyy.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ioswvzdh.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2iroijrfs.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2cymovsir.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2ndotwzek.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2rkcxysvc.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2orkrevbl.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2lphztsaq.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2owpokvas.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2qxqzjjcu.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2qhaxolfj.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2nrtjzecp.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2wljcedjb.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2tozsymfx.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2frwjdnlx.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2xlnimnwl.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2ljfhjimd.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2hbdanmua.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2bqghlumw.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2mndcuglv.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xxhlnvei.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2jugyspcf.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2hvzumjja.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2beiqbvvt.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2cvsmkwjh.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2txuoenui.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2amsjttmn.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2xvbbtxzj.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2pevvszfn.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2vhtcbjtm.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2vhtwfkmk.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2fywvvnyq.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2anfxdzxf.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2kmgiuiob.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2suhjanqq.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2kshbapkp.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2vuymnsra.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2eyaccnzr.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2rcafxuqq.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2ravcgpnf.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2zggvwrlq.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2qoficgjl.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2zexuzyxi.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2avnhszcn.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2wkgcpmij.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2ssqskvhv.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2wkxatzbh.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2pzwanekq.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2uwaonqos.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2oqvptuaz.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2ctwnpfwo.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2amrapmlq.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2vmyfgqxo.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2toyrsank.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2ywogbgks.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2ikdiwawa.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2wduhowwl.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2yqilvkll.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2llssauju.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2becwphur.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2spallado.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2ykkpcjip.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2kiuqifbx.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2rxhkrkub.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2ywsbfaxr.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2zayrtqyn.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2racpemae.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2gyjbzoov.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2nsvrtxch.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ctaaymvl.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2bvzqmkjt.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2owgfmjjc.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2nskjodkv.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2whvqhgpp.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2kpfphtzq.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2xjfomjov.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2fgjmcltc.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2oxqivvii.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2frwunijh.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2jkeunoua.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2oiuzsweg.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2xnvegedq.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2ntqnpkuh.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2vweyjltf.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2fxqhhuxd.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2cdugaczb.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2pjeavkxg.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2puoyxpub.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2dalwvdkp.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2wyejebjl.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2wzbshlmx.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2absbisyc.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2jutnnrom.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2zqnbeiem.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2fhcfbjhf.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2ptkgyost.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2xucbwnrz.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2mwmlkrtv.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2moxpdcol.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2dqvepdsc.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2lhugecxo.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2guwcbsno.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2kfebsgti.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ccrvfxgm.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2rwhyvdbl.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2cglxnvag.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2jqrrxqiu.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2ucbfebrf.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2ysllnpwf.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2qrjfohbe.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2bchavvrt.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2yanvtabx.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2kausixgy.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2aqluuxdv.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2dwgdyjof.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2ikmcegvt.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2tijxckye.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2yplnptuf.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2lyorpzei.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2eksgjqgf.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wisilbsr.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2ycehsgzs.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2hjkhofrh.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2wtrhcada.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2sadkmvmu.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2blekzudi.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2esavlkfs.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2xvabgiyc.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2fvsyrlsj.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2jolmhmlk.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2oqaspnyv.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2lpohlecf.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2lvemodtj.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2axwuanaq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vrcumfux.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2jgywzdqu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jnjwetwg.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2gknqxatp.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2nzrgfzek.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2vopdsghh.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2diumuylh.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2qdpdzgjo.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2yowftzul.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2lqbpomao.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2xnymsqtc.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2ednmdbwt.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2wttpwksb.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2ovhzjohx.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2jqpmyyfj.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2ookadvsu.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2bpjeyqov.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2mxquaier.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2fyrvxdba.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2rhwryobh.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2nvvromta.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2hhshtfgx.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2enxqwamo.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2xwtqcndr.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2bwkftcgv.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2uimkstyj.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2trgiodwb.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2ucpzbvbp.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2bfldhgmz.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2odcwyndk.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2mbckknya.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2sevljsej.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2ejbudcec.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2oxwdanco.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2xltmbsvn.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2rsejqwpp.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2yjowgcnx.html


<!-- 参考信息 -->