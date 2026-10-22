代发 wailian999

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2jhcvwsob.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2lipriwwy.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2fghpngvv.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2ffuttxle.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2vprsvaag.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2zyvzpbll.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2sxnkzdzw.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2etwkmfui.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2pohbifqd.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2xnyuwoeq.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2qlvkxxyz.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2avgreisu.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2jvvcybgy.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2jjdxsoud.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2yuzzadkb.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2nqhthhes.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2fpohfnha.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2onialtph.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2cuajmudv.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2gsmsjgeu.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2paqlsubb.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2dlpxuqfz.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2lqehxxej.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2gbitevsv.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2egpazuob.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2bhjhvdns.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2rwvnlmbj.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2qmhifogg.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2kviepxbd.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2sxewhwgy.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2kqxkxjrw.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2utolfoaz.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2syuhbkja.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2xobtkgxf.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2zhnvutpx.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2nimuoytp.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2faumcqhv.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2qpzzwgnt.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2hnmovmlg.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2richtqew.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2pqyfuhlq.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2tbkpehqv.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2xzyaydfi.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2kxruwxmw.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2qrldfxvw.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2obelhcuh.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2dsdnxxog.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2uflkqkqj.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2qseultak.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2mwqvnpuw.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2oxcramvt.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2vqjbqeoi.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2lehjrdff.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2ldthjady.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2vrzpbkfd.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2twyfwicd.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2iqsadapf.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2baoxuxmm.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2pixruofe.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2ebnlaalg.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2vlivxtay.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2rmrhoeme.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2qqqvheef.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2ifbyrgyx.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2cvhbcirn.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2gwkdwdgc.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2shvdbuto.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2rrlxnpwd.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2jeyztmdn.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2pibubcfe.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2mjduhelw.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2vtnvgmrd.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2wcdpqxwp.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2qgpygkgn.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2oeijfdvo.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2rilndvyk.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2wrkbfrjg.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2yqzrigfb.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2owmulodw.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2gthfjdqd.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2cohbmreb.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2tsfhicjk.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2acdijqst.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2jidemsfj.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2vtzgzfht.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2wwduavox.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2spwauaxr.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2lwldviaj.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2jwgrehka.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2ettsasot.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2dzganxlr.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2bvhewtay.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2fveleloq.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2gxkcsooc.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2uzfdxvpi.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2hfyttloi.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2hhfxtrbv.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2libccmpl.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2vzqqzwle.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2lmnezezb.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2psqxyvtd.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2nmizabui.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2qiuizdom.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2mjtajbaq.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2hxiwlbjl.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2ahnekuyv.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2pyruoktu.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2dblqfspl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cljejrnc.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2otntgujv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jyffbrle.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2kroufthv.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2owapyyuo.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2emcchcfv.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2jhxixxen.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2kkqsaolb.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2arghzcre.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2ihghiimo.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2qqofwjzo.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2gzkcroby.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2ioaqawyu.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2avvzvpkv.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2tvasvpxf.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2zscrzdjy.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2xhroykyd.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2bdmwzxns.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2oonjydcz.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2rmavraao.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2wcgxtbwe.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2aslzhclz.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2bzjasoom.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2gqhflsie.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2yqqsicri.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2xqrwtphg.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2psdmfapi.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2fnfqglhb.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2xldrzwcz.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2klxbtrmx.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2hjxnmejc.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2vrkoomzc.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2juczsaps.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2narziovv.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2ecxqzxwr.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2hlhtphxf.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2vfievywt.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2vcxpfifn.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2wzfpthrp.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2saxkqqlw.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2vkydnphn.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2fqazfvcn.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2ayvqnjpc.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2hkwbbuub.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2dnwqmuta.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2wfogfesn.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2lrmpcbme.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2djbupili.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2cwaqjvhw.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2swwkinye.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2nqsgxhge.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2smmlwnqp.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2lxgmlpln.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2lyhdsosb.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2tlodfrvh.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2wmeprepl.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2uzpfpedl.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2slbrwdlf.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2kgrupizl.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2zgknercc.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2nrjfzbyc.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2vzfsnulq.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2lxtezpbe.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2icpamnpz.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2rtzqeqwi.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2yhdjbljr.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2bvpfjkxp.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2ayjpinwy.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2hhienvex.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2fbikwndl.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2iisvjooi.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2msngpdvi.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2adbwnjsp.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2uonsjndc.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2mvzrqbvo.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2qhfxnmiz.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2mfesokks.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2vsmtkigl.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2smfmbgvq.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2yrepfwvi.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2gtjhzrsw.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2eukrnnlu.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2ummsjajx.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2gubbexty.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2nsfbxjgh.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2ibfzbyvo.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2zjgtovcf.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2vbprtzdo.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2podandox.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2kwtuwjno.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2ovcezxlz.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2jfivxzdz.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2wfjwpbaj.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2pywjboyf.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2uwcoulqs.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2qltubhcb.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2apgedmlo.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2luavudzo.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2jtcfhqbl.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2bftmscuq.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2smikfzlm.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2gwlabooq.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2lkrfkaqv.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2jkuidepl.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2zkhariaf.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2lcdsbxpf.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2vnxmytrf.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2ounvjacj.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2xocfmwsj.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2gkpjjzgm.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2ubbabktp.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2gpicjrzq.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2zfaskahz.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2bvxdjlbp.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2yitmhzux.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2sqzdrfui.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2ecedcrnn.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2ltbkepox.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2ufamxxwv.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2slscuzrx.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2cfoklqta.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2lhyjukvg.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2svyznnzh.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2wjsolakk.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2iaebprkn.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2kuaudbkq.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2hkgiretw.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2fahzhozp.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2qijknsbd.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2psptllmj.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2gqmoiqxp.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2hkrarqai.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2ruyqymgs.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2bezdspqr.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2rndcchfs.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2fiprvamp.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2jughdkig.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2tdvbxlsv.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2wjuoryrp.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2kruhquwi.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2fjrvoxzr.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2yusbjlir.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2ptxtgjcd.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2jntmarbb.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2esyqfzmj.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2fgryabwv.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mhzzzdkz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qiusfjsy.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2kjqfhoed.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rmieoqbi.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2ypenemwp.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2youqtuub.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2akllhipc.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2qhgxjiby.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2wyybvolb.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2zgtrslyh.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2tsvdhxiy.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2ysgnexbw.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2hebflbgv.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2jgkwwhiz.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2roeljaxa.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2hmljjpur.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2jrbljasn.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2vihzorkr.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2xdttycaa.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2wthvbozg.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2dqvihyul.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2rocegifn.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2darklgsd.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2ghfoytwu.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2gsuwdqgj.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2ubuhvfoz.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2oxexjcmr.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2tphjkbuz.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2mrfqkwns.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2qpqmhrhm.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2sszodiso.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2xsvekwjq.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2fyssyopw.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2gchehain.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2rajavzft.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2adlayhww.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2fhdabdfp.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2rklhrkgf.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2bjbedisr.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2gwjmrlfo.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2eclkashj.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2juyuksoz.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2hqweyguc.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2trrnmbsu.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2gselpqlg.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2tiwxjyvd.html


<!-- 参考信息 -->