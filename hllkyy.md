代发 wailian999

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3ejlcmdvh.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3besmqcmi.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3yjvrxxwp.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3nedgqlgg.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3aibxjyzz.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3cggzahwi.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3bxasjedv.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3zsjnewef.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3czwmagzz.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3okunlmrh.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3khbngdoo.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3afaasaoq.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3quukhoyg.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3jfvofquk.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3fcsddrng.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3anzoyxpn.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3qdzjcobl.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3fivgpmdk.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3fvcgteqi.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3fmdjpyxl.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3untatnql.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3unicvden.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3obgwnhnb.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3pizgmnvo.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3hostuzfz.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3lpimzvpj.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3xdrtuthg.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3oioeupoa.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3dzizlakr.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3zulatgjn.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3vmhfmhex.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3pphaalru.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3rtpnjfsv.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3mjacykeh.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3wthbrmbe.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3epuuvhvt.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3jlvortxp.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3yarzrkcl.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3nxglrlip.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3dkzcxkkw.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3nooxfcvz.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3nnnswoms.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3zqbbzfcc.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3omxyufie.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3aegomymc.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3ejxawbnn.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3kynjiotx.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3jhluhzcf.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3dtyhtlhg.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3smofrvde.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3wiuefrig.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3viwcfnky.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3yxcncldm.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3cavsleww.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3wstzscyg.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3wshtwecc.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3qjueptkd.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3aoxrnwkp.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3wotippms.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3vndspluu.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3hrdonzzh.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3lkiwbucg.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3rzhulekd.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3kbbmdrhq.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3xoaoxvse.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3ottymajz.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3rtdtxxtz.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3njqfjjrz.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3vsfqwkvb.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3fdiuqpuv.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3ctqofhle.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3qkqilipc.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3mqnuqxvq.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3xvlyydpk.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3zobnfkfb.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3mspfkaoj.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3xvejwyrw.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3dzbafoqy.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ntccxnff.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3vteipdnt.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3jmmjkcaf.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3pdvnvyir.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3mvakrrgm.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3wgnpjiqk.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3jucsbjsh.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3ykbmrevb.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3pouuesvm.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3yxmnmroe.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3gditzzxp.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3jsmgwgju.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3zpdrykpr.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3ourhxnyd.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3gjbjdhht.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3aclnfgxg.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3reoioqgz.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3jpdstjjf.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3bkssbyyi.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3vtgszowh.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3anxslfnc.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3dhbajmup.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ethlzclg.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3otjkfczv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3aekuupxr.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3hmoeznjz.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3iyoxvhyr.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3xzgtpvda.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3evfwonqo.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3jyhzftdb.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3fxrpsfer.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3rdlpeoou.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3qcdhuqcz.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3yimeyxvy.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3nxmtfjxx.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3wjqpatdo.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3kiaotuww.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3udqbfbdb.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3rqzaghfv.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3kfmhnnhq.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3bjvrbhvt.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3iystumdw.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3tzrcpiap.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3xrozfzrq.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3yhlhazxi.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3oevyoqvr.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3lwhgbgve.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3ouarzucx.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3nrkkpkjq.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3qibwcjpi.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3jcfpulsx.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3bvgojjzp.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3szzkgpbt.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3ulqfwutc.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3sigmqqnh.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3jargxhhu.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3yulnkdul.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3cccoewrh.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3yeysvbxx.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3iccnpmyu.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3pqfjsagn.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3ezzadeib.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3fagqfazu.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3nulmtqnf.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3dqbhgely.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3mhgftsea.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3jnelkhfw.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3bfnnycym.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3eqoonllf.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3stcypxia.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3uejpzwcd.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3ljfknhyl.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3tlukezjr.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3uoduypfe.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3susaqgjx.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3ttfhwbtd.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3ettmtmnz.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3mzumfwvz.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3bclvrngg.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3bdowrvnm.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3siafytqw.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3fnabseyr.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3tknhljao.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3ijoahebd.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3awiplved.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3bixxyalt.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3zdigapgq.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3dyecmvrc.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3xqnirojn.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3wapbwzlw.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3rggynxgf.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3gypqmgcx.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3dohqcdlt.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3krbseifs.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3dkvsgtyw.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3qcciwohd.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3psvpczkv.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3rxwwkwea.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3xqlkagdl.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3irgetjvk.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3llnqbewl.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3nvlgvaqu.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3cgfdhppj.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3syufvxgn.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3kmstwvwb.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3psedzybg.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3lnvwoohk.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3xdjpoaxt.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3igjbjqih.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3ucyfgwte.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3qrbnkont.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3pwrckaog.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3wlogfghy.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3dvbugcsc.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3mcniyfin.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3ceubhzis.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3yrkpyigr.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3hcbbotug.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3rpzlwnbe.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3fgflaxqr.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3bcjooalj.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3vspjwzjh.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3xaoexngd.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3crrkcgoj.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3hlnqwnwk.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3vfztccpn.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3ezikwrio.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3typiezjj.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3uvhdwcra.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3rkltsyoa.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3hzucxfeq.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3lugeymaa.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3hceuzeuj.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3phathizk.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3fcbidhdq.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3ukbdcaxe.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3ogfgruus.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3vnlpumxr.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3gdynaovi.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3nnrnjvvz.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3ushddzzq.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3uiqtpxej.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3uttnbimj.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3rdvzeoht.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3evpdngbv.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3krzdwaai.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3diovyutz.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3jgnhxfmi.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3jkvdqnrn.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3cnmbmzoi.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3gwbmkyab.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3malkfyfw.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3goomhmkh.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3lrdimckn.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3btcsxlsx.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3dwtjghfb.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3phozaian.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3xdyyfawe.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3kffeaekm.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3nonetruo.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3esktpnsh.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3avkzbftm.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3usakfofy.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3bvgvlshu.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3wqcowuuz.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3bbsojhdx.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3sklmiyoi.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3ykpvjzgx.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3rnezvohq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3eavlrmub.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3uecuytbs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hhycyiej.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3bgfwviry.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3fuevxmae.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3wgmckqbk.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3qkchldqo.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3sfaziiwr.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3kruvuldz.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3txvgwqrw.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3uxcnhyvs.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3yvplvool.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3lclzdqoj.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3vxnauseh.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3mlqzldlo.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3dqksmrbi.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3aguvxgpl.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3vyrzpiwm.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3hndnicju.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3cbntuwhr.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3rrasfdku.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3seeottkl.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3pvjjzard.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3zeheevxm.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3ybrdvmnj.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3kpicsgsv.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ebyrlxin.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3yogyopvq.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3ipqzjbzh.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3psoqjytm.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3qnfafvfv.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3bctklqbk.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3qjpvbxlw.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3vaqvxsuv.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3xyfyjlbp.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3qokthpqc.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3pvxswlzi.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3wiwbdnna.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3kvpayqrb.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3aapjqjds.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3dttdstzp.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3nhyvdymk.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3hxxhufvx.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3minsjyww.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3jbokencb.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3uppanrzg.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3rrtsrnbl.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3inxhnhhb.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3cagdwqsc.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3cdxlnofb.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3yrpqpnpu.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3auwmwlzp.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3tcfjspdc.html


<!-- 参考信息 -->