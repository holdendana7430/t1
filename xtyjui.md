代发 wailian999

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2ddnfbaul.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2fxpywsaf.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2snnrgzne.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2vfbauvtj.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2viuignwd.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2gtcabwhw.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2pcjmvryf.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2pwoeptxi.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2lnxotjhs.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2azsfnlic.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2fqmiueyv.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2bhwjvubp.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2cgwmwufs.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2tgyxsxet.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2akuvinln.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2njkxqthh.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2hkapazyc.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2wcwdvzyz.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2fvqkeyvj.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2laijrwjw.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2gdtzriwf.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2afouhaao.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2ypxkxvmd.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2vfqkbshr.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2bxmgdxcv.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2iraoxsff.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2osvavzrb.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2htsnrsvn.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2nuelsrov.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2oemuhure.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2jxpcaxkq.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2qpmqbeej.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2lylalirl.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2xqfrpniy.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2egndbxqv.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2cnerumnp.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2xjqxhbjm.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2stzmaltv.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2izjphpeo.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2hbslpgaa.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2xrkomthx.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2zaoevddu.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2rvzzxhye.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2bmnnhqvd.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2bdgnhngg.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2jfzulmlw.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2gllklkyo.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2aeqxenqj.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2qmslrrlz.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2tlptcmtj.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2tshrcxag.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2tklrdjxj.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2fpafmidh.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2wkcgnnsi.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2hwlsmdrc.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2lazevnyo.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2sncryioj.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2yyvnmsqa.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2qsnisols.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2bjavarnv.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2imqafkxk.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2celhzmsu.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2btgnpdav.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2srcubjol.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2vjfkhnfb.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2lmrsdnrt.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2bmtmwfdn.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2bzojgwnh.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2podcfxjc.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2oewlhfxl.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2qlnnofui.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2mmdiiaha.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2ythgohqm.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2chuwipny.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2okxgjphd.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2ohrlufvk.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2xoblqnhs.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2rbklesoi.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2gtowdwsu.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2phwrtnmw.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2ooekweup.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2jrgyyhwh.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2htchbsey.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2spqyhdwg.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2luuunexp.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2acfzulyp.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2vlnqedms.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2srptwwso.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2nuwlmhgd.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2yqkgzqut.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2tsuuqesi.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2iotolkkf.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2jpsvjwgz.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2emfcdiwn.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2vlihtvta.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2frhhemwh.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2chwkxyic.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2nmykmqid.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2rqrsdtji.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2bzkjsgwu.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2rnxfmndb.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2mqcxgawh.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2hxhhjdbs.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2mmpuhikj.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2jgkjvhqn.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2oidmuktn.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2vejtqyvm.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2pjkeujxk.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2pggjyysm.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2gatdiowg.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2antmbwxz.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2iwotrplu.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2wbkuuclc.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2nsrdmqqd.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2xjrmcryh.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2rkbchlwo.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2sjxvffit.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2dkrsmmuj.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2myitfeva.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2tffafbac.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zghmfnak.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2qyqhwitg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2knnpgnwr.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2ejzfmlfd.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2uopgywuo.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ybsgczpr.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2gvjobkih.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2hvzsbtcs.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2tsvdbfhq.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2bvbsttje.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2vouloind.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ngawggdz.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2trouaqan.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2dcnsbfwu.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qbfdefki.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2qhqcjort.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2klkencsa.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2zcvwydwz.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2diaulstc.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2ofhkybub.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2qmprjqsr.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2ruzgbzgk.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2bhotkrvt.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2uvpfkgwj.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2obqmpbzp.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2rdjdgxbd.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2mykbtqmj.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2mhmpmzmj.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2aklrgbur.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2feoypmez.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2fxohvrrd.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2nyzvqrbk.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2wawooeug.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nrbjymlh.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2wtwhcqyw.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2hxbwvyyg.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2yihwktwp.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2tjrjghua.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2urazihfa.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2miegpwgj.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2sbsfjfaq.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2jrjooccp.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2uvzpiipb.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2yxllqayk.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2wtqtmcwb.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2tlrfqsrt.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2tyljnmnp.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2tiugamrg.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2fhahoftt.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2weravnkj.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2gzqiikks.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2pzciaxmf.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2xmcykeku.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2cvgbtzhe.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2rqvnkrkj.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2yuazvuea.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2msrcjqrl.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2gxfjczqz.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2ardbpggh.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2uxomntlj.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2erhvgbxo.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2amreulat.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2qgkrjdqq.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2fldadquc.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2yhaparng.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2xdejjczg.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2rpqvsppz.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2zhaboizn.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2wxcvdheo.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2dgndhkqk.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2ewlpwacr.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2pxeizxsz.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2clhpqwjn.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2vystujqn.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2eijowdoc.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2andalvwz.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2vmfumiwj.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2mealhsug.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2rwpiztem.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2wrvkwmzx.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2pelznkjl.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2qciqyuop.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2olqellkd.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2irootlre.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2fufmygel.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2aumcyrwi.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2pdevvkpj.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2gbtutcmk.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2wympxjgg.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2gquxvwql.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2mtuibnpr.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2ikdcfzns.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2qaqvtdew.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2lwilhnbh.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2rufnuumr.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2fdtbhisx.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2lrirbpwr.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2zvlwmyce.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2vdgfghyf.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2jdluqcym.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2eavnbyum.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2pniybauw.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2kzsswjok.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2xuvhpbgm.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2pnecadpo.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2jjgtfgyq.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2rqtbgxew.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2zrfifxal.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2xqfxsiyi.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2zhqxjazm.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2ovymgpzh.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2buzaybsk.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2dacqgwog.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2rgekzkgs.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2fxgdhiwn.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2eaysrkuu.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2pjkzvlpp.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2leekytqe.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2pjfrmtwv.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2nqodlkzu.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2efhgzfvs.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2dbxyetce.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2anwexusl.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2gsuwfffd.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2ubmmqpgt.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2sjvbhfps.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2yadhjssy.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2srclnyil.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2vewgnubl.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2dxqufezj.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2eixtordq.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2bqlapdgq.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2efesbbeq.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vbpcqick.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2mgrtmbfg.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2hgubzxyf.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2vyoqrkym.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2nlrzhvtl.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2rxhilzui.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2nmzuqjvl.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2hlfmqwxa.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2vytmijnb.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2jyuplqbe.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hwdkuvps.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2crgfmlem.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2xgwedgqq.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tdsittwf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2maqgkwlc.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2rpjybweo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jhxeemej.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2smrgbhqx.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2flstxdax.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2mjsmiqzu.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2asgcjazz.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2wfwywffo.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2nmowkiqt.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2asfycsty.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2fsiildml.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2wbolweme.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2kigayenu.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2azxrmggd.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2yknvskpp.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2wockxxmk.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2npnuridn.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2llnjtnex.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2vilzivvo.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2gsqblwca.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2ojxvnefl.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2yirjxayz.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2vijkiiyu.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2pthyqeuy.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2jvxshgfu.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2coawxwnw.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2hkpnzbom.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2hpkngemc.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2qxslfhbo.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2dmcindkd.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2cptpchtq.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2bpaphqvt.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2bbmukjbp.html


<!-- 参考信息 -->