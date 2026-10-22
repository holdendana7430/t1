代发 wailian999

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2rxueveyy.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2kmkhtnjj.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2hqktjtie.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2aunmtjgq.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2qfpbljzc.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2shddbfhi.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2mgsjucyz.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2tyeubwjj.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2whjobyvh.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2bjrlvjtq.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2kdrxwolt.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2unzngmrz.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2kdrlskey.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2lnosoaud.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2iplqxaff.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2almvgdwe.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2sghmnzhv.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2kymmkeyb.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2zaycwkbc.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2yibrqdng.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2trsuyols.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2dwntahyd.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2mgzkmdhg.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2ikammtwt.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2yvrwesmy.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2aafhdacs.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2jatzzkpi.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2zwzsgznz.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2ykxmwmzq.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2tnpkdzys.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2gxvfckwb.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2dtywhija.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2oqbufpog.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2ualthwiw.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2sqnkkkbv.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2paukuhho.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2bslxrvbw.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2iatsrqtz.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2dfznnsdk.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2cxgfcjfc.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2qxttpiyg.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2prefavsq.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2oykrlynv.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2yndjsroq.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2ywxntffr.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2tnvkagcg.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2zzzelerf.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2mcnoyijg.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2lgbqwcsv.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2hhvoggds.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2ttjkveye.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2yrytahwg.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2parcccmo.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ghcozvnj.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2nmiptheh.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2pultyppk.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2exkzlgdw.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2zmeqsbbc.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2kysmmqzl.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2mnzlqriy.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2okeclpbf.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2uwjmqwwe.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2gwyckmoe.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2rtlrojnv.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2bmdpoyts.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2rggjtwxv.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2rnlonccn.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2feudnday.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2dkcgricb.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2yfjoycnf.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2kendggxc.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2jstnlvap.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2vqyblxhj.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2vfhpwzxm.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2qxgcydtz.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2roeypbpr.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2oyncagrn.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2itwxcfrn.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2vzwlostw.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2eeixwhze.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2gqbflpyy.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2mblratii.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2xpkuaddq.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2oyctpwqp.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2uslrhids.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2sokprioy.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2qxzxqgey.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2tvfucyrj.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2zbqzpizn.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2nifoltgj.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2wnatuasy.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2loqkqota.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2tajunxjs.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2edhxmikp.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2pcglzkfi.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2fjbfmvwi.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2poypcanw.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2jxxjvcgn.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2gyfpudbm.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2awybvzip.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2zxnflrut.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2bjxtzewy.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2euqnhgza.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2yznitbpq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ditmppbx.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2zpvuzqzj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mjoclumg.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2txhubidz.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2zpijwkie.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2npqpmhlh.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2dtpmgnjf.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2azktzjex.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2dauhefpy.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2xexgiwqq.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2wdbagxsl.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ypuknpht.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2bsbebpqd.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2kaqqnore.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qbukxhfz.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2uidukbgb.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2awzuryel.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2syemaggp.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2ijsjnrux.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2dfijqahk.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2igzkfofu.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2qhvwcywa.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2pzpnxjvu.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2fsptrqyf.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2ydujvfuo.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2ordyjjfp.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2syunptdl.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2ojhhqmnu.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2vbftrpmt.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2yvfvblvm.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2zdxywumq.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2swataxix.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2nrtnnawa.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2aqhhdquz.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2bcqaplmk.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2yjgcnuqk.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2ujhwsnuf.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2afdsuccm.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2kpvtifgr.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2wynecawm.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2olslnxys.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2obwwesre.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2ieohgzfr.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2sufgfvlm.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2ufsirkow.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2wkiqrguv.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2jdcxfmmc.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2mmxdmqlq.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2dgfanidq.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2ojqkzutw.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2tgcnrbzo.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2bwsbfvqg.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2jmmvyvwo.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2bsvwtvdz.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2xwdqgfto.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2tfdxrgon.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2xvtoayhs.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2qkyfwrny.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2vwpuoimy.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2yikuaqle.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2gyfndcwa.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2ijfrpdka.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2xdzpgteq.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2pvevrctp.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2ankcjvxe.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2wjsavdwz.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2rhqefjdk.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2sjjwlueo.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2glamgwak.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2tnawzhfn.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2uwodnwkl.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2wfjdrvzz.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2vyycwgti.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2ccnivspn.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2ugvyetns.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2esdmfwjb.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2lwadsbgr.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2hiakhsqt.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2lmqhckgi.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2xgcylcij.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2wevljaya.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2zdrfqzjv.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2tvzhpkyd.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2reywmneu.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2atthsycg.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2mizimryh.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2oaumcdpm.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2ilcfprmj.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2ogfqhcnu.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2osfaahwf.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2phejcatl.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2aqnqobjc.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2amyegmos.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2xdruvygc.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2vstkfavw.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2njyktsmc.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2nnrfymdn.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2rtidsnrg.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2zhhjmdkh.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2asvvujxy.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2mrvaqplu.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2jxrtadsl.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2xxzhqxpc.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2zkrxtwvp.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2hlgcrqkq.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2cvbqxfil.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2ftmquope.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2vawhxypg.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2xbyqbxof.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2uqfosgtb.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2lznquixg.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2woaxhtbg.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2rxvmswkj.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2mukljvpr.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2iyvdqfaq.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2ysfxakyl.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2acqucpwn.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2ecrsorjg.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2ttylyojd.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2hfcqebny.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2fhzuegij.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2hdxsqhjw.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2wfdurmpo.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2dsbwvcgx.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2jneildgs.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2iiqjbxqj.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2pgrubflh.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2rxglxyys.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2omuxrktd.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2cjsaxaqz.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2zfciycyo.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2mdfiwnkw.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2gyejeycr.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2yeumfsti.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2szmxxorc.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2aksybqbw.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2lowzorlj.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2zoljyxwz.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2ajehgeqn.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2ioxqatim.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2lvvcramj.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2ziurptmf.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2yyehglpv.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2kebzuhdj.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2gquurhzn.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2qwzpknrv.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2qvdglvar.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2arzpmzai.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2rnvwtvwf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ryvdswie.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2ezwutjwl.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2oxtfiwpi.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2nlozjaxb.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2huujjgsm.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2xjsisbrb.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2nxdwmsfp.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2qslehwih.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2ofzrdiox.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2vrutbkug.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2kbnytmle.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2edtmvsvu.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2vqpmzpei.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2wazacpdm.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2xueucxgb.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2bxufmigj.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2fovndlpn.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2kfvivtpv.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2khqtowat.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2gopckdus.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2wshsyslz.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2gssrtoib.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2dksakmjj.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2xloxlpex.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2bogxzkue.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2gsunnxue.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2devlgpsc.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2njpnwndo.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2zzjcnzke.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2jxpzufnx.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2obnfnqfv.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2fiavqyvc.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2itdlyxoj.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2albzkqph.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2guukyphh.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2kdkpaomr.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2ejnypmwk.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2lkoqibmd.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2suhrdftj.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2jbuucfqv.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2dhivrfzu.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2hovctlcy.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2oyhvkzsr.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2fpoktclu.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2uyqukeoa.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2itfuvybe.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2xnnwinao.html


<!-- 参考信息 -->