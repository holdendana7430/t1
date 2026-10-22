代发 wailian999

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2zmjesxzm.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2pzypnatr.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2vbkbulsp.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2uebjnrzu.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2xnaterjj.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2bieuqvew.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2ndonmvnz.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2otennudb.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2ymowfwmt.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2uzffdlkq.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2vvnucmnc.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2kkietvph.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2ksfnqhlc.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2agakjhgq.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2jzifylvk.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2aekeyabv.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2cfjuztte.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2muhlglhs.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2iryohagd.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2axmuadsh.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2lqwyquwl.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2scnzphpg.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2fefcvssd.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2cumirqni.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2lppvqtwq.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2famijslc.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2mwrlsmup.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2fentgjxy.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2yzgdvfwp.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2olpwyctb.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2ldsndtft.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2sswxtual.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2cjrkkxub.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2ydwupbxx.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2uecotkvm.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2gmalobwa.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2fzozyqjl.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2djtxqexv.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2llibewcc.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2arcxwxso.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2wyqzbeyi.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2qqlggfre.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2ffntczad.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2lucftkxf.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2dcsquejm.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2khkotkmj.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2kvajteqh.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2lxjfjisa.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2ftyykini.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2hfkhajwi.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2ruyahqly.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2zyhgpjdi.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2pfqrhhsd.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2ateimsbl.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2dwvjzcdt.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2bfkspexo.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2ewfazyau.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2xixzdbfb.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2xwtjlsdn.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2redvcnfb.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2liloxibc.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2zvrlnlos.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2tvqupifb.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2lbnqftho.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2fptepywe.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2ufeespxg.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2oijipcvp.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2rdawdgql.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ukparoth.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2fnzbpxrf.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2juvnrnwh.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ylljtipw.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2qwuglcxk.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2jkfsgukm.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2jbpftbgu.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2cbudvypt.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2mqqmomnz.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2yvuarxjn.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2njprhsur.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2pdpfvcbo.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2wdhpyaos.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2ybypugwl.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2qtyhqyui.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2ybpignqm.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2dntknzcc.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2xjczatkj.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2hnomewch.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2wuomwmte.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2xwyanyrt.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2octtobme.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2ytbxyfxm.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2wjbcitla.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2oempelxd.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2obwyoukz.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2dqjhloxa.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2bcilsjzp.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2bpzvahbd.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2hltwyylp.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2kszgyyfn.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2lzndkktp.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2vynlhlhk.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2iylpucij.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2isalrfxr.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2ykbtvwbg.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2iseedhuj.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2ivjubbxf.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2yrsjqtql.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2bpbpuhov.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2kecovzyy.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2zrjmatng.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2oumkxwzi.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2ehkpzota.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2uttftqbr.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2wqkcsyzl.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2yxqauqyd.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2kmyrgasu.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2gzxvqwdy.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2yftdwvcs.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2lymjmsxc.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2twnzncbh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wuuqvxfk.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2phxbaqxw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hkhdjyuj.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2vcxnmcsy.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2gmxewkia.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2dwruvlyd.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2ajutrptu.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2bryprqme.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2vxltyijg.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2lxfukggd.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2yrpdvyme.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2nzinxaag.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2kkgwlbzh.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2cuurrvbc.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2ldexzztu.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2humlyore.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2avoamkyd.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2ztlgumob.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2fpggyyxb.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2jbarhdgb.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2bkynwsdx.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2gfmywsli.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2ljgjfnyr.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2hyfrvrus.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2sqmlborl.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2jmfinvsh.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2yozfcupr.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2utpvyaba.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2tvywnqhp.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2ycdjfzei.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2yulwjdsa.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2kpuvmsfe.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2kwmvexjf.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2gjaggmeo.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2udddkdlu.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2owlrvsyx.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2mibrreok.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2lmgwnkmp.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2rxsjkoye.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2wlufyzmt.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2wqzvrjud.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2cfxskbyo.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2jqpbabxp.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2pvpoucqx.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2utjrrkvj.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2rdfkysgv.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2geiqwthx.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2tggnsgie.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2ofeungvc.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2nqoxgztj.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2wulwzqid.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2texvkgcn.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2cfuqrpqz.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2qnxumddn.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2xwlgdkpl.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2aprbvkgy.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2cppkqhoi.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2phacfsvs.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2zlvdblys.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ubvubkbg.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2elelypgf.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2qwfzgfkk.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2mkxsvsig.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2lrlbnjyz.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2ddmfsvap.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2hworcwez.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2cqqvhcdk.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2bgqoqifp.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2tvkvtapb.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2khqvqpol.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2oqrjrveb.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2lnudbnia.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2wscvgvul.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2layqmder.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2pokcrhdi.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2ejmboxqj.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2nlenhjri.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2enxedefd.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2bqsfethb.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2ufnkhfzy.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2dlxvtbrv.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2mhoglpal.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2xtxylbud.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2athklcsw.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2xazauqsa.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2mfrcinpu.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2mhrsyueu.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2pfcevfkg.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2gbjpxzdj.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2fgmyssex.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2rcydoncw.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2ussiulre.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2ooargmld.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2jgzyklwv.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2jewtfjyn.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2bxcwovrn.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2bpnwbpvi.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2mudxivya.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2hdkftwrc.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2wwxsdlnv.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2hehgcbul.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2pxrzpsnc.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2ieayaylg.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2vdbupsrh.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2alfatnig.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2qtqcpayq.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2wsnggrxp.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2bydbdvkq.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2rblsyzpk.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2gnyoyund.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2dashilzi.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2kvnxsapy.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2zkzorotr.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2fjdzhhby.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2bhzuqodc.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2jtuohbvm.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2tlournfy.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2fcsgzcqp.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2arnqdbxb.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2xafznxtk.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2zjolgojy.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2dzeklwle.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2koyabgcw.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2jroussta.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2jobewmwb.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2wohjrryd.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2zdymnada.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2dvoicvzg.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2usybswjv.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2ckanoboc.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2odajxlhg.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2gkavgxbk.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2cukmiijy.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2eczeevoy.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2vijjqbds.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2fukdxuwy.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2klepddlg.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2hgtqahsp.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2aoynvfwc.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2zoldlmmm.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2mfxesevw.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2lywgygbc.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2ocdradhh.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2fhivdpfd.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2abhczaxo.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2ustabomn.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2rqiagvur.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ulxivysh.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2dopechzz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lrqsesgs.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2hmcyuoww.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2zugctyhg.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2jibxrytm.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2koswjehf.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2tquodrij.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2kenamzmy.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2iqcgjpya.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2afxffokd.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2ywxzrogr.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2rfaqhxyj.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2aoxvdvyq.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2dnyqjaei.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2vyjsnfya.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2mjrumxrt.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2pxdteoqu.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2ohgzauoj.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2khvvqaos.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2ldvkcvdf.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2wdshllfg.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2xxsenxag.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2coxuystm.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2hbjnfjef.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2polruxzl.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2bijahwws.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2yynluzej.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2xvgmvzvm.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2wjvmtjbt.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2qvhvysot.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2vqjtqset.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2mmrvvzpa.html


<!-- 参考信息 -->