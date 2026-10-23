代发 wailian999

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3vnvslrhi.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3whusouca.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3xqwjduqn.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3hzmhgfrm.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3meivkjfe.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3domdrbwa.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3qarlssde.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3ifmtvotj.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3phmbmood.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3jqbvvhbz.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3bdshtrno.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3rooekkib.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3cmfmdgiu.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3smcsovau.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3eiphzdoo.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3ueyhhdbv.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3rcnjlptz.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3yzykrbkv.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3apkrcvbf.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3lrshmyyy.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3edqaptul.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3nbdlrlhh.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3ukzwoavf.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3urkpebca.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3igmficwc.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3euktxvfx.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3zwfueroh.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3kjaryfeq.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3qrbufzgr.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3rqaqmjtl.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3nnywjhfl.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3okqbjoej.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3ioyfnkee.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3hjwglamm.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3jamnyfqx.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3sgrhvoal.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3oylxgydi.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3yuynsaot.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3gckjigrc.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3nccscfui.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3ckepufss.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3pywaxufx.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3alylsjux.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3keraqyiu.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3jphjsvuk.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3pvptzvbm.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3bdftvaon.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3guamexhg.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3zrcuagxl.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3vmoiqlrn.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3smhgpxsb.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3manikdek.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3rqbozmbp.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3duvfzvjo.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3elpugxsr.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3kurdbzcs.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3ezhguxwj.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3uxvwmolv.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ouibgnva.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3nnlqwrdk.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3xaldawdm.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3ehrpmwjp.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3hwsntxec.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3bkwrkarc.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3zdctrwhu.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3qbbnvyil.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3wddnifug.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3urjhkptz.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3mbbsxrmd.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3qvfpozrm.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3fgcslrza.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3qnzlfnyq.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3zqapwpox.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3mqgxtfsp.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3qmgjlfui.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3iydwrfmt.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3hwbnbhjm.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3bdvafobu.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3fqzavaxv.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3xzyjwbtj.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3gzyiuqbe.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3pvarrajt.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3fxycqbdk.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3emczjkkl.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3muaceeey.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3qtxcffpp.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3yfeenwle.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3gkkrszte.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3smnxjaej.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3opmenjfe.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3rzfiwwqn.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3uvugumez.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3pkejavlp.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3pzzoovge.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3qtnfbvhb.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3sbmsvvxq.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3pzxlbfjb.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3jkydqzkt.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3wypwhgbk.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3uylmpeqq.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3nxrugtko.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3bommsldg.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3zbnzgluw.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3otcspfmt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zdlfuual.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3zfczbbon.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3oamcjfwn.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3rbonzypn.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3ljfqetnu.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3wwrwrqql.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3ujkgpgjp.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3dzwtbncr.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3thwiybmf.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3ywusnufm.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3onobdoal.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ksgismqd.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3peuvzvly.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3zwsnwiph.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3tigqlckk.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3gqsyvdcb.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3eqqrsmul.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3vzuwbnfe.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3uwcydkay.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3umyfbaau.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3txgdxwye.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3bsslwcoz.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3jmafnwmz.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3yfgehjka.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3oqrjeeny.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3yyncedci.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ousqwvga.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3dkuzazjy.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3pxdhcqid.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3tkvftgky.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3jtppheny.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3olywrklu.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3thixfuax.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wyydrvmx.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3wfzsonnu.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3vbnncpce.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3thpisnyd.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3xuylmipm.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3iswqtzbi.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3iqregehu.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3thljgscs.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3xvpqummq.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3obplhsys.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3nyfyrjvt.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3udugbdgw.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3ykufvunm.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3fggxwqxw.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3kdhuwxml.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3ydkayfpn.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3kcwodrzy.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3jhalhjww.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3dkakduve.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3ttrpnovb.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3krmnotyn.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3efxisdyr.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3zsklenxy.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3hncijiuf.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3glorfqxc.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3rqsojlqe.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ccxjyepd.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3msblsshu.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3bnhodpyx.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3cumifomy.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3tirznbxo.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3kxekqrkt.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3rsdcovzh.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3dhysyqqw.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3jpqjxwxe.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3edlndfnq.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3jpmdruyp.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3leugjbhp.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3ykkqqsaj.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3vylxnjss.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3phjzwvpq.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3rjxnailr.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3avexbyvs.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3wcxtnxko.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3nleqanou.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3xwurbkkh.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3jnpkcant.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3gbbargnu.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3dgmtvydk.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3vipkliwr.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3gcgzbbwf.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3btnwlnuo.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3pjkhfavk.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3hhwzesyc.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3tfjcyjjb.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3zoziunsg.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3nmeflury.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3ijqpcbpt.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3pzonyear.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3twydqjxt.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3xwqwooid.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3xgrytqsx.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3hbimrnjn.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3zuhtokug.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3vacclasq.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3wujavivc.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3khxznbts.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3rdstnvuh.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3lsawxlri.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3ozcbhxdw.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3kapbdzyn.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3wltvbvri.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3tjyrmjco.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3fihvhlwu.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3uryidcdw.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3hxoqnrsj.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3bhhtxqan.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3bzdwdgwh.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3rslqicue.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3aefzbiyk.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3dbgpejaw.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3rybwomlk.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3atzdubnh.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3ufsaeeou.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3tpnrfobi.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3sbaycjbv.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3nrlmzyhj.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3pjfibwac.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3vjzezpcd.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3zuvybwyu.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3dlgfzdov.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3qdqjjfdf.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3elwmwruo.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3rvjmmovl.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3dwwzhigu.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3bfszxxus.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3yqjnygki.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3viclarsg.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3zjupuwnv.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3tfurjidk.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3tzwzrbyb.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3bptllhhb.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3clipgmch.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3ibyrzjru.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3dvauaaft.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3ljndyfrd.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3esrsyzsw.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3ktomoeqy.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3ekncfpet.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3dxtrmscn.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vxrbuxgy.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3jgbcsosx.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3dtwxukze.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3exlloibj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rfyfdbns.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3fwdepbgf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tavtoouk.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3kzjhnllb.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3cpugfvxn.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3eoztvspw.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3qreotncy.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3pfefwjzf.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3wyfdwxim.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3gzdtltzl.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3qgpvjgpy.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3ogaerqqe.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3wslvpgst.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3feyaenur.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3fkaxqafk.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3evrwwzqn.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3cxwtlokp.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3gblhlgdj.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3pgorwgpt.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3ubjqrdlb.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3idgyvxlu.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3uaxsnnxb.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3lcciubum.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3zwxthwdp.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3ucdoyvwo.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ohjotgmd.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3fhqplflq.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3wrdplpug.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3vpdnmexr.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3drfevxcs.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3iebyecfo.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3lccmmtww.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ddqmqsnc.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3srpvlmkm.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3vnlpwxai.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3phnswcdt.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3zslhuszz.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3viemhnmo.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3wulfimgj.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3pznelnjj.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3mmzptyqm.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3nhtheurs.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3pndigvar.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3zncfrsxg.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3miykubvm.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3zkfiiefg.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3vgaurivt.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3hqpkbmhp.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3qpqoricm.html


<!-- 参考信息 -->