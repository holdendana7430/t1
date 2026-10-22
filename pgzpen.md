代发 wailian999

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2mxyzlwua.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2pljwvzlo.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2sxmpzeyr.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2eftofndx.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2bhadyyey.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2ixwhmkaw.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2hzsziore.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2vykwxefj.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2cquzpvnw.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2zefadrob.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2nmvwphrh.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2pyesuxfe.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2awqwwfva.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2blxbvfrs.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2zgsbsshu.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2hlakkosc.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2sltkledj.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2fqoagkfq.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2btibiwmk.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2umlbetby.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2ouowbrep.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2chebyzdo.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2jjiffypl.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2ttierbba.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2wljerkea.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2pnaldqdd.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2jpwkjhoo.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2rmjhakjn.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2xhfvaxew.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2cmsqsklp.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2bqfzzaqb.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2htwisjst.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2qcponqjy.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2jclgjnhi.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2swmvzogj.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2qspldpqm.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2wuncdhgw.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2nunshuet.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2lqovefnw.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2hvtrikba.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2qzsampcb.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2wwtzysse.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2jccixugk.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2afjgqrkv.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2sxmdbrlx.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2pjhmdxxp.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2qvflzcrh.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2mvorqxgr.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2boxisgzw.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2dxunjqff.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2cyrpgnlo.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2ulalbvtk.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2rsqcmfpf.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2ssuegjap.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2stzenxnh.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2isvtbgcz.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2mwxgebcn.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2fuxnnufd.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2jesgpfdc.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2eixxugsb.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2njfpnebs.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2nyjiqgzu.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2elrilowb.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2lctnkpoi.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2ktqgzcjc.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2dknlyvgd.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2booiixgq.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2jtatuzfy.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2neptwukv.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2cnwnvgby.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2fkbsvpvu.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2yuvriltp.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2ohhrohik.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2gegqqmwq.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2bxjnrpyr.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2qatfzdtw.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ixlhpoxz.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2tsdrzxqt.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2wbzdyjnq.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2bpdfdmlz.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2cyfpvtel.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2fmsbsydl.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2tzrblcrj.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2sdgteegd.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2bcegiigu.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2mvctsexv.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2fegndqfc.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2bogfxkww.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2xxntqngj.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2dnwxmuet.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2xbtotxua.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2zqfcjfdj.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2tputcncj.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2vdygajqw.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2optonfqa.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2jxonbziq.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2xlkgyjjl.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2flpuwbqw.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2ylbycynz.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2mngffvdh.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2mjskcffb.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2ojysnyxz.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2dnajgyye.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2bnmvelkc.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2somhxmad.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2codnpgyb.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2spxewrod.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2ggvmyclj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kuuarjkk.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2zwctqcuw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lbboakcv.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2tjmqyebi.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2qvgmxrkk.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2littvnvo.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2naidixtt.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2kyvdjbhl.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2srorrzez.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2byxrjcxs.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2ekpnlwpm.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2pbwpjmul.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2uejkbirw.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2pmbsvwtm.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2derrasxo.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2ilrfwrgb.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2ulrqvgxn.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2ltmutlym.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2zeqidufo.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2kdbnavhi.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2jgpguyub.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2hsibnpew.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2bssvhoab.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2kpuzrkln.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2lecpqvkh.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2wlaxblde.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2eefzsgff.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2zrpxmezm.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2tndkmttg.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2jtwwrlxc.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2zrlpeaab.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2iuqiyfsb.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2fovnvvan.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2rokqxhwg.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2aiylxvrt.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2dmekafwg.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2vemtjwxj.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2htrjuwxw.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2syozjxmf.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2dqvrrhlo.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2uckpfzvu.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2diutabef.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2kpfjqzsv.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2llzsamlv.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2ibczhlbu.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2whqrndip.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2nqpgciug.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2sznvdihr.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2rlzvxtnv.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2jrbwjlen.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2plylbrgo.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2aqodxswm.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2yjfhtruw.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2sudbcvyh.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2efsvbdkd.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2udvbndsu.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2rvzxbine.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2ruxauwxd.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2wpwrrixo.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2glerxrpa.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2qzcjweyi.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2cikweior.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2mssgnegt.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2amorsqyd.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2kghnsfhk.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2hurnemoq.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2neqacgxe.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2jiyqyowf.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2lfnmswpy.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2dymenjni.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2heykfbtc.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2fozkjcey.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2quwgbswq.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2gwjqoxrh.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2sfrcezxt.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2vqnrgwxg.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2imhzqphe.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2semztntd.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2fxigpmki.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2drjwgojr.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2degdohdm.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2ufmqzdrc.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2jqasskrn.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2jorvhwbi.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2jncdnvtn.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2rabzvwww.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2knptzkzt.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2iaotgizi.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2tinhtxcf.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2vxvxvowm.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2kilxyktx.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2kvciaqux.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2grfcoynt.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2pyyuhzcy.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2mnvltggg.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2vsogtmix.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2xdqyzbqx.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2tjpmncmz.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2dhnejeof.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2scagbgag.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2bwwzddgv.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2wszqpppi.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2ddjnwafv.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2wbxicdrh.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2nomtllix.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2vkmobqym.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2lnthyhps.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2rjizptos.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2muardclk.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2dudwgbfe.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2aobzisut.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2nkpwmgdc.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2nsrxpign.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2bhexmxvl.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2vjbkowwv.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2lfpdpyin.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2dyuluibq.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2hkeziynt.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2mbkvxaov.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2ryjgqbjo.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2zvkxnmqu.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2ssgphuzx.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2nkutdiap.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2rlzcopkp.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2rcxhzlot.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2ahxnjddv.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2vzoecznw.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2hoxnnkmb.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2zvmuhxaq.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2nzqhryhv.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2lhwlvjnu.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2tqvmibta.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2haidduqc.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2iajddgus.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2jeqbdsmg.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2bozqtcnl.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2scahkxlm.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2lsmxqiaq.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2zwdftcgu.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2skuhvewk.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2denfjsif.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2ybgyitns.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2gilznxss.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wievjydl.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2mdiubldo.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2mazpvnka.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2ogvptbhg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pkukolcn.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2clbbnaqc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yaqgzyaa.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2vrwknnxl.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2smrsbmgh.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2yowxugra.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2zzkrjchs.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2dxxanwxu.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2vftfdofp.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2ikcylfoy.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2aanypnvg.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2evfmdymu.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2tdjzzgah.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2dvzaaxlg.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2josxfkfd.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2nqhlllba.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2gpyaoadr.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2zvjkspcy.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2paojiswg.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2nlfwqofz.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2edyuotqb.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2yevvwqpi.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2lihgvfuh.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2dxochfpn.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2rdrpamyx.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2shdpprrh.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2bnlujuxh.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2ezgltupu.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2ixvmioox.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2tcdywwun.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2yoiushmt.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2qpcgguqy.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2iyjmltgx.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2uglrdtjh.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2acaoeceo.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2cuhbkbph.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2bkgaxeak.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2mllbrrgf.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2kaohrttd.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2amhhphrs.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2jpdogkoq.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2fgahiuyt.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2vlbfcgle.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2gdnrrpiz.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2uzxdmwlf.html


<!-- 参考信息 -->