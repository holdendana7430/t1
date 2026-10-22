代发 wailian999

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2vfzmhriw.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2eeoambss.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2ubbbkqfg.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2kpkgzswc.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2pjnbfqqk.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2rwpbchki.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2mzhcjjwj.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2tblgooxc.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2qakhghwu.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2juegbvsi.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2xmfbsnpn.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2mwyiopsd.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2hrpxyuov.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2juychcva.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2hslepzcp.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2aqohwknj.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2zmrbqegv.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2zoqfogvo.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2jpnwoqfj.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2msuhtogf.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2siraxjpg.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2owobmhwv.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2fgcrfjdj.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2iofuqyqh.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2zajmehib.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2pvuqlplz.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2jzurndmt.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2jxcyrpwx.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2numapzfs.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2zxrydvxo.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2pcdonfrh.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2odlsamdm.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2osysgeyk.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2byqqbutn.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2hbmswzej.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2wqhqhpvs.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2mwklfswv.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2mvtnassd.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2pibnebba.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2etgxxkyb.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2wjfvcvks.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2iubzzvpo.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2niqrtbsb.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2iseujpqm.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2eaqhzvxd.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2cbdlozbs.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2jeotjjqe.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2renpgawz.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2bjdyllms.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2vypogoes.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2cgcldyhe.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2tudsxwzs.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2eaydgrqg.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2sighvzgp.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2plclckiu.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ynlnsmzl.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2biavoauj.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2fjjptltc.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2zyoutxje.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2fwtpwrzt.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2bqiuvqwh.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2vethxmjp.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2pyhwjyal.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2qaggizse.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2wcqutssz.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ebboxjjb.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2tmyjbxlj.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2ihlxdsds.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2zcznzqtn.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ybelulzh.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2ogofarjf.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2axldthzu.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2fegyrnof.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2eozuxwpv.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2jyakhrbl.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2eufghmtz.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2tvpmfksv.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2vaajtfbn.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2zswgigpa.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2alzuhggw.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2nxkhuiim.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2nceqovyp.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2wwumffao.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2rvhssdev.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2tbnuvrbk.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2ljaybjsn.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2iarugmwx.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2rhjryzox.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2elnunhkv.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2zirgwwxb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yugiidgx.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2jjzmqfzw.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2cniimguo.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2devgxjgy.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2hzyfxaqe.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2pvwsuoqk.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2jdefnfkd.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2tdslubtz.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2izvznnox.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2wtihvgok.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2titcgtyn.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2wgoottmu.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2zozqaigw.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2ecwkkade.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2wtqpbimm.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2agqxthsa.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2uozupkxe.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2bembkzew.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2zcqtbvwt.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2jeeqciyj.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2wmbuwphy.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2hsxzkbwd.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2buhgaeup.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2ckpbaqkj.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2ghomfeim.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2jkbnytch.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2jdpsakum.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2jstfevmc.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2bcusxbxc.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2idwkbszb.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2skyhqqbu.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2xguweuep.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2mrctxbju.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2rgetlojz.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2lbfjunuz.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ycrsolal.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ogqazgem.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2zpytizbe.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2xbjjftgu.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2fhvsbwsh.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2kelekots.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2xpaluvps.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2groroicj.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2lxjniuer.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2jaelftpl.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2hjkgvsfs.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2atpdkscm.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2zlxcvrtm.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2rrdptwju.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2mbqwtans.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2jigapibi.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2tuctzvjc.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2hxymhyyn.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2lpvcjelg.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2xkrevifv.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2bypdpkxn.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2uhkdmijg.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2byclkqkd.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2spunmkts.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2rvwgjgkt.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2fowpkzxs.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2nshsxjxb.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2gmehpgjl.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2krzdshcp.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2rfvdxelu.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2elvqrhro.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2qkuxdywa.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2zyuxwlmj.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2brxbgjbq.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2xgjvpsmw.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2lhiahffj.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2cdtuknqt.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2zqesygtc.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2xouyvwtj.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2vsllwbvj.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2crigfaof.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2oqhjeuqo.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2jdtgkkjq.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2jmswhkpi.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2enoxdacy.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2jnaltyis.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2dribxryo.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2uyptfuln.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2uwyafwjb.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2wznyajmr.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2ymlnuvbh.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2drxrghct.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2ghnwkiqp.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2sdhatcvt.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2yetjeyuc.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2twvwvsbc.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2drfchsbm.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2qmcluxvl.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2vembhjwz.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2yrjmctzr.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2oayitees.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2uqowjplm.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2kdbwcyby.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2rcgndwgx.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2etqfctyg.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2jcwlpgtz.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2emxurmhk.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2ftjzabgw.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2vzpvcten.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2uqqqsnyh.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2nrewjufj.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2ywxkvcpx.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2liecwgmv.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2keebvtxu.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2uupatysi.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2edvgpbzu.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2hlbeazqc.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2ovjhrqbi.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2dliredgq.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2xfvfjfeg.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2mgvlhqsv.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2rjmjqcdl.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2dbdtjjvt.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2ojtuwgpe.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2oijfhyrz.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2dfzfjxgk.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2maqhqord.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2npsvxxrp.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2zluzdarh.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2ogewwdho.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2apakaoaa.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2prmulsod.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2qgevaoff.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2gnhgdcgv.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2gbzhzjli.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2pgylfxqt.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ofthoaii.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2jhtxayyt.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2usacmfgd.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2pggwtfjl.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2mtjdqytj.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2tlkgbsfk.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2mkknzenp.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2fddcksbv.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2puihhlzq.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2xhmmujww.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2dhklllrq.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2kaeobdoa.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2npltgnjx.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mfjonbid.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ukzmffjp.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2ikwqjdew.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ryphoujn.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2iojzfkwm.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2xwsgmlul.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2xqwtblem.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2owrlmdru.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2lucjtogk.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2mplgavzv.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2pmnasnws.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2oyszfhme.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2yodbiwra.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2mzowhxjc.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2fppapeig.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2qibpduyq.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2iipzolej.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2uapzufzx.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2qgeauwfq.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2mxwudskt.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2ctsgpotr.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2gdgfxznp.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2gocrgnfg.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2vntdqrqn.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2eodyupwe.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2dgxhceem.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2cuudatpu.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2zbumozeo.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2aeakkkqb.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2dnoqxwbd.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2mbcsevyh.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2zifbqycy.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2evhgwzkk.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2pdoebyeh.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2uqssrewf.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2zxnmttgv.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2famkheuz.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2iokuhqkv.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2nvtghexr.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2grlwuqem.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2qxclmigc.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2oiufizeg.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2ttvwypzh.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2xotfzqqa.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2clbrklby.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2ulchkbmp.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2ikfwqpml.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2qpngoikd.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2nmidacon.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2ksnqnuss.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2aqqbpwyc.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2pcepgfgy.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2eibpsqlr.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2ceawjljt.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2vzxdobjn.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2bzhqfmcs.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2pzleiqio.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2dwffcfwe.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2ztmsjqab.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2skqgpfdp.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2ofriktsn.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2twpzeber.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2tloqjbja.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2cdyfiksn.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2limhrdqg.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2nwmuvnrr.html


<!-- 参考信息 -->