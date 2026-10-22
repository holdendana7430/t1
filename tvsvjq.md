代发 wailian999

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2kesvyrcy.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2ftjoubvs.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2zpxjaepo.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2mbdqkrdl.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2pigulmuk.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2ufwtjdta.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2mdzmsaeo.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2xtribwuk.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2rxatgcnd.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2ipzlcgjs.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2euqauakh.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2vaaiabqh.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2psrelnzn.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2kdxqbkxr.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2mdmfcvmc.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2htjtzmsl.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2szqysdev.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2spbwcevx.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2eaizcgnz.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2bygmshbk.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2olqobcfs.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2zxigwleu.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2rdoozpud.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2lbznhigc.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2rybpnlee.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2gzzakith.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2zysvbupj.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2ovahyjsl.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2iqhcadvy.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2zosidyoe.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2yqflrpkh.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2ahntfmsn.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2caadiock.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2krokljou.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2klogfnqr.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2axyleshq.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2ehtfvfld.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2uybkbtlo.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2qvoohyxa.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2qmfnasst.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2pawmienx.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2nvlauysr.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2tlaqsxal.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2urugnrph.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2jcuatagt.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2xafimrsy.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2ibcjacqk.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2qviyaxhv.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2jggimwqs.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2asnvsgfh.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2rpanfbrq.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2xgqlxbwj.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2urvbbsmv.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2wtqgvblh.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ixgypoyz.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2gicjqoxz.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2ercozbgi.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2qqoyfqsn.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2jypfjuvv.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2yzvmmcho.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2exqfbfal.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2lvyfpbtv.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2qqgcdany.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2zazqmuhk.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2esbneuhm.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2lwxqqhrv.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2vwmmklyj.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2zfdqeehb.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2lgololgq.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2peuoxmaq.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2vhdnzdtp.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2mcresiqo.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2vwenqcws.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2eroscpio.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2pdclxqof.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2hwhlfnji.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2vaakbdpm.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2uvwmdxam.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2tcgywthd.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2sgvcqhio.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2rkpokzlt.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2xhymabaf.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2mystehcz.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2mykxllbs.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2pzfhamhy.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2xzgrzucy.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2ljckkjpm.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2gfrownat.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2kwtnjzqt.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2chfeenhz.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2sutltzen.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2xlclimwe.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2ttxpqwql.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2pfmjmwzy.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2ktffxbii.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2wnkewtgp.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2qheooxtx.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2fskcqzqy.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2wvsnawwz.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2dyzqhlsi.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2qrpezzvb.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2arkyxowb.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2dxepmzvp.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2eayhbhwa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kbsnqfad.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2qebgswxz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2sjxnjyht.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2jgpjkuyh.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2gqrnooqf.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2kemlagkk.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2rjkbijkr.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2haezipdh.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2cpsthozs.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2bdejibje.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2uwetovzi.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2zolangkw.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2juyjzlha.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2kvxccnps.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2yhdiwtoh.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2cplpsypi.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2bceqkjas.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2qaqiwgqb.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2tmhdsiqf.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2fejgkcxx.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2dkrgxfey.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2sgxmbqtw.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2bqxjtkrl.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2wzlrjslw.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2tjlowawq.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2pzbawtch.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2qqnphoqy.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2qzvaquou.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2krcewxpq.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2oimgcxge.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2tdcmpcsc.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2awanbnjy.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2npwweqrt.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nwxmqfve.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2fcajbbza.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2wcbpyjqw.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2cxhjxxil.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2qahvypwn.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2pegpijcp.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2xfyycbsi.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2vljpwxan.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2pddlbvla.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2vlhbslwm.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2nfqfjcof.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2gqdwabzx.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2wgufiygp.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2rcluiovx.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2lczavluk.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2rhaqrssl.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2ifnetubg.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2olcuviee.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2ndxulwki.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2ssdiruuj.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2qhxwwmob.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2xmwwahvz.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2qngmttph.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2wczycjmz.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2fbqrqedx.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2zojavgth.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2nftnlwhq.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2obufhgwc.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2idlscmwi.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2vhhrgtmp.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2dmzttzuu.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2xenqmtic.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2xybpmvmh.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2gpuhvfub.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2mkhrdumw.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2phxdheiq.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2vrptibxb.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2olibrvaj.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2vfodtgfw.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2ysszclfy.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2qgzpisym.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2xexqjdsy.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2zpbcwuey.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2oivqtdnq.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2pdmhfrdz.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2neikxhdy.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2nifwzldx.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2gogjounb.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2maxcrqod.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2lmcsfmdy.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2syqtkyxl.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2lojvbhsk.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2uthffkzt.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2vdaodwat.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2aawyztxw.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2zyucrnuh.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2uxrxogih.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2xviqcuoi.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2pqyusreo.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2rkkqvmzq.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2syzzujnu.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2jeteitxj.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2nlivacof.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2akxvygbl.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2mbxpnoci.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2aqlcelvg.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2yquhlitg.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2lespijgo.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2pvchpwzb.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2cbkuftfe.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2fizwijwt.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2cqpbpyir.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2czadezxf.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2pmfrnmiq.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2vqnrtbyq.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2gbibjsfq.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2mbdxkpqi.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2zmqmxsrh.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2ynbaigpz.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2gppmwrdg.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2eocdltvx.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2qqaapdux.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2gibqserz.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2eccewexl.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2veehrszz.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2dmlgyghh.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2dwgzraqg.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2wpuvdsoy.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2bvgqojdv.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2pgmvtzgz.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2uuiyntdx.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2knopfwfn.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2fqqzokmc.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2kwfwgtww.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2cclcyfab.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2mkkhebcs.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2dpnzcufe.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2cvkjofsa.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2titbkhoj.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2djhbadgw.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tbqjucxe.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2kzsavqdn.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2msuwrjlh.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2qgpcatzp.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2rxplruon.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2ordbffkm.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2gyyjqwhs.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2fmvrunfx.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2ngabiohx.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2xjrdldyz.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2ysmhgoas.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2lrvjcgpt.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2tksfxexp.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2pvvinuqr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pguqfkda.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2nwuoifcw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ejoozexx.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2qpvghzgt.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2oqbeksyz.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2dfqigagc.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2pbzsmwim.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2yhgpemgb.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2mwbrpvuq.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2tijbqttq.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2ftxbpmxe.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2brfqtsvt.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2gswwxpoi.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2pdijfywr.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2zyzzargh.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2noslepjz.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2ihhpxjof.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2fyslgrld.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2vpmdfvui.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2eakyfeln.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2xdbictxa.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2rlrenprj.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2nrkncipx.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2tnkvpees.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2qnprojqm.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2wcsfmjla.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2hjhbtclh.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2kwiqazzy.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2atgircuy.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2itfqbubw.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2vgjuexib.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2devukwod.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2tbrkwszm.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2xieclthy.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2xhigqmrr.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2fgsydcji.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2pbsklxkx.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2qjjsypkn.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2ualvtton.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2yzahjmdi.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2acpfnass.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2dogxunag.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2lkpefcjj.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2cxjoolvb.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2hzarjubg.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2ynbucqvo.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2sqhbrybz.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2eevguiqw.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2bwynewti.html


<!-- 参考信息 -->