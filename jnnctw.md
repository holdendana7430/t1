代发 wailian999

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2defomzjp.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2nrszuijp.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2fehdspal.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2fpqsblpo.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2uulwhsyf.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2xhltbham.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2wefhdoew.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2dqdodour.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2epeoffco.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2lebgvkei.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2sesuiqag.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2vyytqrmy.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2whoxlhnk.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2frzagzjd.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2zizdcutz.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2inxljqrm.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2jukrtwtq.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2aqipxtan.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2bwhbrqqe.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2cnxilzgx.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2zxoasodn.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2ewlumwos.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2pqbegwqw.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2brdtdydy.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2hoarxeae.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2ykvcddda.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2shsxvksd.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2pwsdhfal.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2dbabcniu.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2kbttjvid.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2bnstrfoe.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2hcqkkdpm.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2stittkdh.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2rdpqmdja.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2tmeekywl.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2dcuaodpu.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2bbwxfsfa.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2fhlpqkzl.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2prohiosz.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2epgbysxn.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2anccbmsj.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2zjqaxzre.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2forduhsv.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2afmadylz.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2htgifcth.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2zebkvtsw.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2bpwdasot.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2unsrrqdg.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2esnzxpnl.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2urieazzw.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2eguxfotz.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2kkzvfwut.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2kmevnwod.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2hemaykqm.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2rmbrdwyf.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2xxxlrnbg.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2fzorlpjf.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2fehslsdj.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2uwgyfcay.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2bqlydunq.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2qeqicyzx.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2zgkkezdp.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2bxjhyudj.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2xdcrbuad.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2iujecxhx.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2puncmust.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2mgkvvlcb.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2qmakfzyp.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2eqxbpscg.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2gllshdjy.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2lvlcecvm.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2rzcpbnqz.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2zdpzakqs.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2uozauzcw.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2tjksntlk.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2azqiiqqd.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2tktkxmxd.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2iqagctac.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2nrdxpfio.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2gneopxzs.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2boecgktf.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2vnjycawr.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2vufbfarr.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2ulqkneib.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2kymgutrf.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2khjsfvjd.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2huaozmdr.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2nukzstbg.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2evlkicib.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2ienkvvii.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2vjokhnvt.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2bepdpgos.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2mcywtjvb.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2kcharqrm.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2yzkdvwxv.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2ufiqtztd.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2txqtjfzo.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2pwdmmgzp.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2bknlvepx.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2naozsxyk.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2mbegpvix.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2xfmwrdyu.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2zwqcirtu.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2jsgyjigw.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2xfeiewea.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2ykxomlco.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2wltrrvmy.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2eipxfclx.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2jblhdksq.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2ftzgzcxq.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2pissfmps.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2whuxaydm.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2irxygajj.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2skmlwldy.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2dxthdxrr.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2rjcxjuup.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2mgtinrks.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2sriszmba.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2huggates.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2vxhasjwb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kfxkpefi.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2opfcximz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mjtwsjub.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2afzfjumn.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2svrctyvv.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2eavmbpbk.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2kenzzrre.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2lgvblstk.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2dizmoowo.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2yfbcerbv.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2rjydhedq.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2zadcaxqm.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2qmokmaxb.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2pfcglhah.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2weokljxh.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2rdmuobfa.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2devxcsgr.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2xstersdo.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2iridlojn.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2cfefpnpy.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2czzszcaa.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2vypruets.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2fapsyqke.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2eihvrsbi.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2iqvldfcq.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2lbjhvbom.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2uhkvdzpp.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2hsnwjxtz.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2kbilsxuz.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2xlplujwr.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2bjapanax.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2skaverhe.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2yfzvukrx.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2sekcwmiz.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2zulsthms.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2tfplnzeg.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2chqjimds.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ecloerwi.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2bnihakri.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2plwrtxxe.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2qjyusunv.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2hqazhjxj.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2hylavgaz.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2dkaqdgea.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2vghfljjy.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2sdecabvo.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2ovjfvlpb.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2qzszmwzp.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2iircvrdw.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2arprluqy.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2ujqnvxjv.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2nrmtmgmo.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2tzcqdxtm.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2lugcpvij.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2ltpijasf.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2buzocrlk.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2gdnpgohb.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2xouauojl.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2ioalcvxu.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2xrrkwoeo.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2fnxbqmel.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2vkflbkop.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2sbwpktwj.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2jerwkcaq.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2ldpdzgoa.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2idrpmbzq.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2eoxbddst.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2hmonmhtw.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2othebnas.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2asmgoqss.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2cluabpup.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2isckybrj.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2asmbqetn.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2fhnoeett.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2gstbclcv.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2txetqfbg.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2smhwikss.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2ueqtskcf.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2nnfvdmaz.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2adcufful.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2mavdzcva.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2uashmuzk.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2zkwettsa.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2tpeongjl.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2yhjmeflx.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2stssyoij.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2kupaszvb.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2jjdyjwtp.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2pxmyqcxq.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2ytclgozm.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2rjpjuchu.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2fscnaefr.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2witfafjd.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2lkbsazie.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2bnwopmqh.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2bkoeznoq.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2ajiqewvv.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2qnajwuxw.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2fyadcfxr.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2ksjdydcf.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2cnwfqgbw.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2ttviqgpo.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2ekawrgeq.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2qnnvvsnk.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2uegcttjs.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2vqubeecd.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2xqoccoal.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2tmcbardi.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2issxrsuz.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2cxbyogpk.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2sioefjel.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2tsykfyhz.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2bmzystgk.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2kdleqzpv.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2zzgneamr.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2jcqrrmui.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2lxdgugou.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2gfrdalnn.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2hnvltthj.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2yzcrjhpp.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2vkhqyztf.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2qehrscrm.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2ywxnookt.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2ttegrucj.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2dgaoojgt.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2nltfnrbg.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2qhdbzvhh.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2qookmmhp.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2hqcsuhnl.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2qxgquymc.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2fggcqnco.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2kffccgqr.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qkpzawma.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2zdcjiflw.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2reimxixq.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2pjzwyndp.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2krggeokp.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2njrclmtg.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2kzmcedck.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2hxzthedu.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2aflxijat.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2swyqhmef.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2idqqflkz.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zadfrrkk.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2kopumbwy.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2oiipyqgs.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zncrrdiz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gqgxyyye.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2bgzhvpuf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tuouxaxc.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2eligvvuv.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2magnqred.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2nponjfgh.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2bqvvuqxf.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2kzdclixj.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2bxyxgfvt.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2xoozjzee.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2kbcvisqd.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2ipgkobyn.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2azouvsuh.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2tgrazpdq.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2llvseaon.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2gsmowfkf.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2evdglmsl.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2svaoiiby.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2pciifxmc.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2vioxlmct.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2dlpxhobp.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2qcqkjkio.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2fvdanszj.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2khncyhel.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2vqqwevqo.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2sihyjmst.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2iuamodso.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2yeywkpca.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2dwdttzrz.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2sbeepmol.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2zbryttlx.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2ceudyjfr.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2bcbsdsuo.html


<!-- 参考信息 -->