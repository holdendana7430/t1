代发 wailian999

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2azcpqrya.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2cgalvhaf.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2lhgvxcow.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2fbdevipw.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2zixdjcsy.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2cvojdkxa.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2eekmromr.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2zzrlogfv.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2ezwsegkq.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2cppvqjou.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2ijhjovru.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2cxluadrt.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2uawewznm.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2cyxdpvuz.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2ewqwkuoo.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2leymysod.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2rpoimrhk.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2rgvojueo.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2koyxhksd.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2halhcffi.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2ubfszrrr.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2prhemoua.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2exoiadgl.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2anmcnxye.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2gmfdblzp.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2qynhylug.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2csewawsz.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2hsmnyqzf.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2mzbunrem.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2luanhsci.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2qnjildjn.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2yfthefwi.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2hdcztmwu.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2jzksagog.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2znlbznbg.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2nmkwapuf.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2vsdagygm.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2nnaeldau.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2jgojskny.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2rkizcpto.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2wmrjqkah.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2qrwhgerg.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2arlrcdnv.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2qwpzhraz.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2unegnmpt.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2bwowylbe.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2bkpmyiql.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2kryiqyoq.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2zrvrqwix.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2czutkwud.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2gsomghar.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2qpmfkzsg.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2uwaiaocs.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2gtmnwnem.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2eslowntp.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2nbqsaoaa.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2rkuxmvsj.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2mydgvicf.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2nhgutnwj.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2gyfmmfqg.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2qlynzhro.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2pkcvzhhd.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2ensuuoit.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2hcpqyefm.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2dwrwguul.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2tibytscp.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2azgkawbf.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2woqbfucm.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2bakbdtdd.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2dwhoeayc.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2ymcrdmjo.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2khgtxtkv.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2tvxccjyt.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2myfdnjsa.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2gtkbcnae.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2liewwilc.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2ltiodthn.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2ntzwalol.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2jsftlnum.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2pkakxzyb.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2ppuozcmm.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2vvoxodbm.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2iyywlsxo.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2ebowwsqx.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2fsjngxzj.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2buhlqbbj.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2nopeemzm.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2tffshcte.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2xetchzhb.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2tcyaycep.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2kwygkdfa.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2ttvejmfg.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2botsuuie.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2gqixjqre.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2hipyknth.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2brpdqdrs.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2qgyophjd.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2uoxiuvwl.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2kmaizkmf.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2lzcjyvle.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2cztsyyhv.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2rtmkpfdu.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2yqhzpvwo.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2vyrglgze.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jobrbljf.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2yclbvgjg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vvejjaxi.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2yacegrms.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2kyxzufya.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2yzrogouk.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2qtqjchil.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2mihiynnq.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2ozflxnnl.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2aelfvkoh.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2hfdoelbr.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2rputjpam.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2bepcjpiy.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2wylonuvs.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xdcmaoeu.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2fddwvmcp.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2jpdgwdte.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2iustfqao.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2nudcqxtx.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2jmyqbtvw.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2sgawdjsh.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2glxzraji.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2qxhibrnv.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2qqxqasnr.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2jilxrjxe.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2lcmfdgof.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2xgbuhqht.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2absjgloe.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2paglxdrg.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2pdkrjwxy.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2gvezkvlu.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2pyhwszta.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2doziznox.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2uvbaicjw.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2mcrotxgw.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2pkwtfctj.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2oslwaguz.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2nilkufef.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2yoalooxs.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2gfxkjhhp.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2nignojdm.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2tqfmtwsi.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2acmgzlqd.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2egwuiyiq.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2vdfmeola.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2tnvswbzo.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2ygplrfee.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2jmxfqeou.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2qjsqcvwp.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2zrxcshxc.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2xciclanj.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2bnqroaup.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2xlyaxbwr.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2rvjlgkzn.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2ssooxuju.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2lpqyuboa.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2plrbpyml.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2cozmrjfa.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2jhcntxcz.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2fqhmujdt.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2fxtravck.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2asluzdvw.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2azhvkdev.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2yleluyyh.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2lwvslrvc.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2atqvsmlb.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2lflihzra.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2dhzgfvps.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2qlaqkbor.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2gltxrwal.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2qgavcqgs.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2fksyllqb.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2rnvuvulj.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2mhobaldd.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2iatovosk.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2bhcqzacs.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2xrhvdear.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2cfmaonek.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2dkbmasip.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2wtiuxzps.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2nnwhwoxb.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2wmgdmhmy.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2xnoehrag.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2ogaiylle.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2tcrjilau.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2yqweouba.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2yhwbtxgw.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2mwwclozx.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2igxaylbt.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2qpasrufp.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2kdmcftwz.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2lnqcfztz.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2zjkeeusz.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2cjsmifdt.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2gitazmwv.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2jhwyqnzg.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2sewdfogy.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2llgeiedx.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2epumtejl.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2vzsuovje.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2rrvyadmb.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2mmibiese.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2clxnsilz.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2xjfkrdnh.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2oynphvvp.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2rigfunst.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2kdtnqoca.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2hljqnepu.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2qijwlllj.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2imelcirq.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2qocuuavk.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2dwmzjwgz.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2gdbjqirg.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2mdnarkah.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2gmguufys.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2xwauiptt.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2gbxetpop.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2cjxkfdtk.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2ynkxwege.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2szxixhrc.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2jmeszhay.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2uvdppdwo.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2wndblmcu.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2swoqbeky.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2uyuniodm.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2fqhuxxzk.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2qpnqydnd.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2igknqkos.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2eusivpjx.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2gehxgdns.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2xtwtyuxa.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2lexfwsbo.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2rwgjbleq.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2cgnsspya.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2vucdezsj.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2cimoexdn.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2foyotqaf.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2padpylex.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2pncdeylh.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2vnmiguyu.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2rcgzhsim.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2tlmjupgd.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2sfvuvksl.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2eglqndju.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2sqkylqvc.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2qcsqcxgn.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nbphnvru.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pvcmthza.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2utuxcoam.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nfjifdos.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2nuboxsjo.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2elyicuzv.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2bsokqvzk.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2oshcoynd.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2kgjtfusu.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2switxaoi.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2fhlxnwtm.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2caacinuv.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2eqqvoegr.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2vtkgrpmb.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2bwrvrtay.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2fxhiasiy.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2inpcrijg.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2gxdjvmey.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2twopazdi.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2aukbjlnp.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2nmawoqeu.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2dwzexefy.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2jkmcvfgi.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2wyjzjwck.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2gleqctya.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2etrvwtgc.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2yihesapi.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2fxqzzihm.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2iutnnhnf.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2rjxfpijo.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2lyzitwru.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2mmlppolg.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2tktxpcct.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2oqwjspno.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2asnouggr.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2iijwtaed.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2llnxfqtv.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2zzkmvsha.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2bhqglqda.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2avkfhtnp.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2xarxohvr.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2nawxfkun.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2svjyfruf.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2njikoqxs.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2mwoweezx.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2lxzwcqav.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2gkuyuigp.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2wfloqfeo.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2znvzgnpi.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2uasmotxc.html


<!-- 参考信息 -->