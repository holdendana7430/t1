代发 wailian999

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2ecblnput.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2pwjscggt.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2stohsktc.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2fvqscvkv.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2ovqxepdf.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2npovutgy.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2mlgzcnpv.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2igzhspvs.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2iklsitlj.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2celjxkcl.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2dnkziljg.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2iqmzgmfk.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2uetogujt.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2ruqzbjdv.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2sphijgdg.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2lzfxhoiw.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2tajfagsr.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2pqjbsutf.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2vhqfvowp.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2ujdbwsti.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2eaeluzdj.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2amspkfld.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2kqvulxve.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2qgcsnsax.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2jqzesvju.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2rwhwffmw.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2pmjklptx.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2zekwvpxq.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2nmubpzjv.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2qjzshqgt.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2omnqildn.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2ziykijkd.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2qdbqojvp.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2pbwgehrj.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2qatxjnqj.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2uhvwaikg.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2lnbmqchb.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2vumopzbu.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2yeyhavkp.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2twjuynub.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2rsjrahhi.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2eedqlyjh.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2jvlhqqjr.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2xddzlhip.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2jlqwmevl.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2letxxktt.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2mombopmq.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2yzqyyhnt.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2cwjgfmtd.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2pxaabkdo.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2ppxkjmea.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2ugjvgqiz.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2pvytfcrw.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2uydvhypl.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2kyzvpgaq.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2wummzfgg.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2etzflgqv.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2bfbbcaeq.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2doildgkf.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2tldipwvy.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2pypwvjbm.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2zpjpllkj.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2liwopfcc.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2rfrgpbxr.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2ztnqthsj.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2awmnhvxs.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2nlycymzd.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2rldrgpog.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2zbnftdtb.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ywpvcvmp.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2zyvgomhl.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2mcejugvs.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2itfftnob.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2igijahvk.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2yefgyvxe.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2sjxpuusf.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2ohpgcjxl.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2aihcnocu.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2jjpqwbej.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2pthsuubs.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2pxscsjdj.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2xnszmymv.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2dfmojsco.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2yyianoyp.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2qjxdxhmo.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2yxrcdnpy.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2nljxewmw.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2qlxalpdk.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2fhwmuliu.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2poouqkxk.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2grwaedab.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2jkkgihuz.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2tsbjxyva.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2ieblduse.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2jxlczfoh.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2symbyxcd.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2suxnxgau.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ftwwrzmk.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2xqdidxws.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2oszddprf.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2pcsksluy.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2defnhzlj.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2yenlvsgs.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2vlnxsyom.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2fgxgqjms.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2ujbzayxb.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2qohlhuvo.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2qtywjoky.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2tavmvtjl.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2jiptwctr.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2mzxuulus.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2szuvklrt.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2pegbhzzi.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2zcqwgnxk.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2jxaztrkh.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2beelijkb.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2wzeixmyo.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2ouidabjg.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2tugxjhtq.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2jnibxndp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2aycwrsyx.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2wlbnkoks.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ncnjhcaq.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2nhcvaphw.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2lrgrfrfh.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2uucdqcwf.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2csaafiam.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2wefaning.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2hofyixyn.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2cpkfxctg.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2kgmrawnd.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ncvsdbrm.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2pxtkeipv.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2sknspalh.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2dizzliue.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2wnrsdgdy.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2euzucjaf.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2ahziqvch.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2cikokcrd.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2lyoaxgis.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2yumycixa.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2gzmuuxff.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2aenqffnx.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2heghynnv.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2lxpbipov.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2vcpzwmxo.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2fkphhwmu.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2khjkfkox.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2icfiwjjn.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2enfdhwpk.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2ucavawhc.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2cuzeghdm.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2pkzseoup.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2oebwqkem.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2fxaohmod.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2szwdkhtr.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2tdfgfvah.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2uxcdbmhz.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2qhdgunlx.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2nccdstwt.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2ukkmojeu.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2jqtvoicl.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2qqwbqmor.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2hhkkgaac.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2jeqlvhlv.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2xdylhsyv.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2gikvojlh.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2xudkigom.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2cbcoziom.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2pqtwonjo.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2xdpmpxvl.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2ahacsmtv.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2uozgxexw.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2fbixdunk.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2gbatstmi.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2jpdvxesc.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2lwuesqkz.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2rfltrufg.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2fakkpjtd.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2ybghkhlw.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2dpjiwvuu.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2ndcglaxe.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2wnrmvvdt.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2tbetufbq.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2vovakkhp.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2gxiouvxs.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2waesuoiz.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2xfjjpnud.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2uuxngdhm.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2ebcxoxmi.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2lbhiheah.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2uzrmbbem.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2uxvjputu.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2ilbatdpg.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2ejammdcj.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2gtmtpggb.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2syabkfji.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2knyitift.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2rmewwmqn.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2cawbdttp.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2ylljiyry.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2ejyvluwq.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2pordhbkl.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2zxptzhjg.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2itjzgynl.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2qbkotjqg.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2trzcxslt.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2gkcmlmzj.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2jbgjovui.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2wovbwjir.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2zzauqbrf.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2toyvhoty.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2vywbxysh.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2wgfkvlhh.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2kbomiurb.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2vjgiezhk.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2dtakwyrb.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2totaaaie.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2uynwrikv.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2crcxpvpc.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2apoatkbj.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2zzckyfyg.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2jfkxgqbk.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2jhgimjzn.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2ancaeyoy.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2jygegezn.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2yekurzkg.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2jbuaiwmp.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2ihwvkwos.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2uropwutk.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2mmakiaxz.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2zgfkbvef.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2pruzogan.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2eewmzmlq.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2taorfcyz.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2gsptqrkt.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2azkifcxk.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2pfovvugy.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2fratkppy.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2jdefuebr.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2teqvuicv.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2gkxdkpik.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2svlbpofd.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2ulctizqk.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2nfxguqdm.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2ddgugwzq.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2vkodzvpu.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2ymkhamqp.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2ygkemjdm.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2jvgrxmjd.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2ijsdlsbc.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2yqsgmgry.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2kdevmhir.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wfryrzfv.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2ditycmyw.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2tnbouttd.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2ehhlhvep.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2baxerowp.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2dvjnjovf.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2xpdlljcf.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2natxjlxi.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2ygcpzdza.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2afqwfafg.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2ezvyxjuz.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2hufpnvid.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2mbcfyqor.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2ntqbxtho.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pkdbpyvp.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2ihnmudyy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gwhjomsw.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2cjehggiq.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2lejmvuwa.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2wrgclowy.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2tkicfyyz.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2kymnosps.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2lmworkjz.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2pvgmtvtn.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2pxkffpla.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2betiiazh.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2iyitwuph.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2aqeunyop.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2ruifsbqn.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2toahcmms.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2ohvbhpdr.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2bigilnir.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2koyhvwlx.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2kubnghdy.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2zfyouezr.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2chelapfb.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2wvzmmahn.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2ctzxzzhc.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2okixollk.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2dufdhfjw.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2yshljzpp.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2gctelttx.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2amqdcfow.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2spivieil.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2fnizalkp.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2ibdadtmn.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2gavdmdma.html


<!-- 参考信息 -->