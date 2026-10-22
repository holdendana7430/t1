代发 wailian999

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2vtelxleu.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2bqdbasdd.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2ssxhqyjk.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2epwpxptc.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2unbfytxl.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2vjiawfrm.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2kxtwmhzm.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2fndeeqla.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2oqsclbel.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2kwfbudaa.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2vdqlvifz.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2dtcaphdk.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2lruwzpfa.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2dlhgevbb.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2qjigtiwp.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2ukcyqlkp.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2enohkdtd.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2qylotirb.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2xecbyaoc.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2wpttkfge.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2yvsfjqnl.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2bpifonyp.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2negnhtrz.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2nmsbbiml.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2uqqyyyqs.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2zlpcpoun.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2skimqgkq.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2erzxggxq.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2hzibrymt.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2opackhkw.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2rzhhteyd.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2pybcmbmv.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2dlfrtcfr.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2sitfghjb.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2gowkwzkp.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2ljvghona.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2ntjovzht.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2iipivxel.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2xbogyyta.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2yafxfisn.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2gplzedmc.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2dknmcypo.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2ofgilwyg.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2djjfmiae.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2vqrvuexq.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2egnqxujz.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2vzohnvpg.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2pzhtwlyt.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2uhqoghdj.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2mjjbqvft.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2qoqjsmfi.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2uslzmvpt.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2yusplioc.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2ihpwirnd.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2jdjhorvc.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2coscutrn.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2kretoyqa.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2okkwwrac.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2odquibhc.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2mzlkzkam.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2bmaogpur.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2uptkgtlx.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2kjdgozmd.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2xxjuygzq.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2qipwihkb.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2iugcuaua.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2ieqklsqw.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2cakysmno.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2pfgstwba.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2moqwadzl.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2hpgduoap.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2pxdgktpk.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2bokorwme.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2dhbwnsar.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2riqqcwdl.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2ropyidjk.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2cvwtzzdo.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2pnwiyedo.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2xptjfgzb.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2zsbsxgsu.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2qbcjowfo.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2kclhcmga.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2xkjivspk.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2loaqgpha.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2izznnmjr.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2jkxozqne.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2mwxyizen.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2wbvsfbgo.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2uimmktxm.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2tmfxihlc.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2lxdhkldt.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2osgtjcwn.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2hanukmai.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2bdyzpisn.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2kehhichh.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2qwgqxpmw.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2olyoantf.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2esmnetqq.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2erdwvhaq.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2zhwxefyu.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2dokkbkhd.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2bqgqmitn.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2ollaamxl.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2zmsvypla.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nlutvrvv.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2ssboldui.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2abfeopod.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2tacuprjm.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2ckvtwigv.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2cneflrsw.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2cgzikadr.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2sxwpampd.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2wuapzpfi.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2hkzegkxc.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2vrnjxqsq.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ceprbfml.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2gdtskire.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2fpgydyxx.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2iaxbnxtr.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2eiyzrsmd.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2nvjzmgpi.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2fvayjpml.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2ncktlvya.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2rzclqxvo.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2cwzxvubj.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2netabasc.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2lvipnisb.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2wevlsgoi.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2ucmwxkob.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2hqrwfamm.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2lvufhicv.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2sxxhtzvd.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2ueeviagb.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2cesmmbwl.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2akviydts.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2zxscgeql.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2dgxkerzg.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2svsvkvpc.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2qcqwjtfd.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2xtcxttyf.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2kotnqwku.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2pkrhtjfe.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2cnuugyiu.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2nnsfsuwg.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2cardturs.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2zrekteaj.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2tvmpcaua.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2vxbcjjeo.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2ymbnujrz.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2bnvjshja.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2cnjdrgbf.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2unuydbss.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2rttiepyr.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2vrebedux.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2ivescdoj.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2jjhpsjfk.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2onpawqpf.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2ccbhrccl.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2jzogyihw.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2bimzhdqs.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2sjxlgysr.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2jrxjdity.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2ldbnborn.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2nnfzazfy.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2hqjplilf.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2cfkwxyqw.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2lvhjcvcb.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2qnqdcoti.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2mihdaphy.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2hmbkntcb.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2hguiwxpl.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2pzqacarf.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2ujsprein.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2oegsrnmc.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2yuikqqya.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2uvpoqzgw.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2xjnugjyv.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2rqbfgahm.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2zrapzzuq.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2bparetjq.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2tfnukfys.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2xscshlmw.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2nimopuul.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2cveriykp.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2xkonpqfq.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2tceahwho.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2slrbzkqk.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2fmpniwzl.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2fgehjafr.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2wqymxhoa.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2xpenjozs.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2aqjwijni.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2rglqyjff.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2fghlgjjs.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2ioercktq.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2aobymrur.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2hsjrazne.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2iqbtgkzb.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2hawqpilf.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2dowttvxd.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2hcuepkqz.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2lvwzmbot.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2bktgtvbx.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2ltmyuwcl.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2utmjxqmg.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2fubwiwum.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2mwqepnlj.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2aesmozcg.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2xttzlixg.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2eiqlgbqy.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2loagvdqo.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2xnfplmht.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2asvtweju.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2zduwlwtg.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2eustlnuh.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2xogsehtt.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2acxvijql.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2mthzpinw.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2qswvbazs.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2hkyjkfsz.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2vduwgnri.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2spnxigky.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2ydirwlwg.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2fzceotyy.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2kglhfwkn.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2nynmutmr.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2cftognmm.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2pjdkfrri.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2fuyexcyz.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2snnefuzp.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2dkdjxpsl.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2eyxxelzz.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2xzqdxheq.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2qaichefc.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2piuqfcgf.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2uqoetffa.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2orwrtezn.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2awfusgqm.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2bdfbtenf.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2fpskqpem.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2jpuqxono.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2sxdgcsry.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2pabbdrua.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2wdefjbtn.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2yscxmrrh.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2fnlwzudk.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2nioawvtl.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2bgxjcksr.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2tkxyhopc.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2sdejisyj.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2utmkpqze.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2thxcmqto.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2kbbppsww.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2imhvsgyg.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2rtlxeicd.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2nyzevasg.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2ypuqezay.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2kkmstjtr.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2cluzuwqn.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2tfnpatrt.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2xyupjwwy.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2syhtrvpp.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2ailjuwxl.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2ifldztdz.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2wpzlpfiu.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2kensmlrz.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2yvqkvuvc.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2czmrcavz.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2ycvciovi.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2pxsjyxtk.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2aroikqag.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2motpwxvj.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2szsyqfxp.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2benjnnib.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2cgqxrcfw.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2flhmfqbh.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2uifmtdki.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2rhzvpitz.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2djnvlirm.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2nfvsvhuo.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2xsrmsdcb.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2tsxfbnom.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2fqrmllmm.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2jxkpdqnb.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2cdbdefyg.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2hrtqwkcm.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2rjmhmxht.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2rekffegl.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2dayiyyfk.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2hrfgflyz.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2ttjultoq.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2uonyhbrm.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2tafatwfh.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2ibtprvmz.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2xmxvdmgm.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2yrqowgqs.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2roqvunjk.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2dwwhovwj.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2jdtscweh.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2cojaxida.html


<!-- 参考信息 -->