代发 wailian999

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3hauizemj.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3ekvylgqf.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3pwotxxko.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3itvnygqk.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3tydpzrkh.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3kdexuzsz.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3obtnogvt.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3huzkffih.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3phlurerc.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3kyzbfpro.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3nynpndxs.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3myvhpylf.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3tmxzltqq.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3heeifkhg.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3wrgulkem.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3rvtgflpr.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3jrukammx.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3ltaczieq.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3ztnzrltl.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3qsvpugsv.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3ojyosbcm.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3kcjlhjnw.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3numtcfsg.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3fpgjebzl.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3gqdoaxms.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3uuytacnw.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3wgidsfvn.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3kobdbgmd.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3dtshtric.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3erkmkiix.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3tivqfhpi.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3oxdaddsg.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3siwelwlc.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3ulpowmnj.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3foafafge.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3jnldhdnb.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3rttakvdi.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3xmhjtjpf.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3tmazpldf.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3wrgtujzc.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3eljfycam.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3gnpdwokj.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3pvyysajl.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3tgksxfsl.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3aqpknyrk.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3nrpovllz.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3tojiuabn.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3vukquwjq.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3xvcamszc.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3yclrlebd.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3nlyrfpok.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3wpxvoray.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3lkagkdog.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3bolxucnw.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3hjenncys.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3hukmjrlm.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3bfriyaac.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3ashekfjs.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3tdipqwkh.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3sylngjfb.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3alloviek.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3onvoawqi.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3kvkburai.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3fvjvmpif.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3aewzhawh.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3wbviwdmr.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3ygkbbomn.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3lnxjmabf.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3svdguxqp.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3recuxpms.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3wgcddstt.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3dkdceowd.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3prajyvkz.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3xomihpwv.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3njuphmij.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3slcryziv.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3wowiaslz.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3ykirngzq.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3tryhbcrz.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3tfgnctku.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3ehpwsmrh.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3vtnaaijb.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3myqbwcon.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3bjoxcsuf.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3vxvuszoh.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3flkmebmh.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3daqtdmzd.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3moghefep.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3kcpbrnok.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3ofgyszbg.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3haishsdk.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3wwfnoxhf.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3dhpcnkjg.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3tqhswjrg.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3mukqiwom.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3potibvua.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3csqcgghy.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3gmchpnrn.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3sqrcellm.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3cxolpxhm.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3jizjohrl.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3bydwjmur.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3aybwcxsn.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3kkvaptpi.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3ikujpzuc.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3vpmuvcyc.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3mmstksdo.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3lghoglnx.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3sktpqsyr.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3wxfmmlnj.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3tehzempn.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3agbghhjk.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3maaqusbd.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3inogfgxv.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3vfxrapzs.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3zhhfknti.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3ydgpawdi.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3ipxofxej.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3anmcdmkp.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3zhdtaiur.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qribqplh.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3dwrxliob.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zfdzdehy.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3wcchnsrl.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3rsxannae.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3npfbsong.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3apsbxxka.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3pzhjuzct.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3stmawnff.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3fygtgeqj.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3dsfqxnqx.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3tzkudafq.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3kyrscdbm.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3xrdrveey.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3kuyqqrso.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3mkshgmvn.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3ivnripwf.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3smozsxec.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3jwhimvrl.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3iqkplxkf.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3tuiawatc.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3ymqglmke.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3kdiyawrj.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3cvhtnseg.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3mamsyyoh.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3xhxcbovt.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3kwotdaaz.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3hkaqlbcv.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3swejsfao.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3cxclbujx.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3cjeacaqt.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3cdpxzddu.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3ysjnfzmc.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3vxyiayqq.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3djvrmnre.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3bnywslnx.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3yzuclyri.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3zpiknwzc.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3hrktuwyc.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3atgydlkw.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3ezswaaul.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3zxnhvezt.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3twiljxla.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3xsuojyah.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3yflaivzq.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3jqhpqtji.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3ibsntrxa.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3ebqpnyze.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3avdrbgyh.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3flllooyu.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3ltxnwyxn.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3tyjoknbw.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3vhybjore.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3swnligsi.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3zccvbzit.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3nfcllyqb.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3zfshumrb.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3qkmtxito.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3cfvqwgkb.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3czeulpil.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3hgmiqtxr.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3nnsoshws.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3fylsdiid.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3icrcwozd.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3agstovju.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3avooutzt.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3zllasvcv.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3fqtagcdh.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3whnijvbc.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3jlhwlrbj.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3ytpfurcg.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3pxudlzej.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3rfpsunjj.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3eohpabqg.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3uxxcugrs.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3dsrercos.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3gzcazvpt.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3fttpzpcz.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3coxhbisb.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3qtlxvwvn.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3rvygeuxg.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3wiwnbisc.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3pagqtkgr.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3hrhsudck.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3ygfrlsux.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3zogucath.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3mbjmsrhk.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3ldndidqj.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3wvsgvcen.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3jccctvft.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3bvsevkvz.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3wtahgggr.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3rbovsquv.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3pdymelru.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3fzvbobat.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3hlpwthhu.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3wfppiqfr.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3xdpyiart.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3noruizae.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3svyuybxn.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3dhlzfdmk.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3hcxhalts.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3crwmkhpl.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3mwrssnvk.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3yxknqxus.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3nncprahj.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3nyqdotlq.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3vlrdgmop.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3ztowcvzm.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3qtxopbwy.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3xispjduy.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3jbujnwnh.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3zxwygesd.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3pqnqzfnq.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3nnmbpoon.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3vpuocura.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3aunhuvdj.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3vskmrxak.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3pavziggn.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3myyvkvpr.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3vkwmsnne.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3kwhmgysv.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3zsnjvmax.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3fspnlynj.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3noyggtle.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3mblyvrbl.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3balxmfpn.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3tgzrrgee.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3dbxvjunh.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3npuuepmm.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3hdwfgsge.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3bmfotlfw.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3nzornbjk.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3eaqfyxgl.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3frjnmiua.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3iygkvpsx.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3hmqpkibo.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3ycseuzfz.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3aqruemhl.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3druezwkv.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3bfdjkjeh.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3atybejyg.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3djquwjdl.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3txckaadz.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3bkyxypwi.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3jueywaue.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wlzfpdyl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ushptnmz.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3lfazesqe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fhjtdgon.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3rfgjliaj.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3nnvcdeld.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3peqyhoxq.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3qudpxhhl.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3jxvunygy.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3nollltfc.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3cfeqzkta.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3lsjcsrzt.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3wcamjvka.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3uzjfyxco.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3edvknbxm.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3jeneywqu.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3xarpsepo.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3kkzcadaj.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3godusuzo.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3utctyvya.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3qzcbutxp.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3pxbbgzhu.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3coxrwmlf.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3avrmnitb.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3ngrbdrwx.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3ozfwtpkp.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3swpuuxob.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3gsnyqbxf.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3kvjoirxh.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3jcbetjbs.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3hihhtxue.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3mrhmjinu.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3cwedwusi.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3furhpfba.html


<!-- 参考信息 -->