代发 wailian999

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2labsvfgd.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2jatvowak.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2xpzglyyg.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2azrmoxhx.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2xrmnolmm.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2jaqmsnqf.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2kydygcyt.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2mgvvlsbw.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2xzamljno.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2dynunqvh.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2etchdiyb.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2rqomvtid.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2eypopuev.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2iltcolvm.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2pqwyeqnt.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2duqcgphu.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2uaodhpds.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2vcymljhv.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2jfhvkmov.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ehznexxs.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2hjdraezd.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2tpwmcqyy.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2fqfmgmvm.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2xhhystin.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2emppxwsu.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2ptuzeexh.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2izvdhmdf.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2ifooznvg.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2plhtvjlw.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2duzpoxvp.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2gcgoxltx.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2vjvnuipe.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2pmyztgib.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2duxcyklh.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2aqjdmtzt.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2jetshxhm.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2renefkkr.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2xxypblky.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2knlguiot.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2cwyoyztp.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2mnygjxai.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2jrpedmnu.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2zkyawqjv.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2lfmedpyo.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2osqafnxv.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2ythakkuk.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2ufojvhvn.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2ctrpklng.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2vukmuqok.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2auklwqvu.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2nszjbbqj.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2xphfyjni.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2eztpvhgf.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2vmepbqrs.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2pljjcyta.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ddbehkun.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2lbzdfgbh.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2kiqmordt.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2eslbtsmk.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2mhkelfgz.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2pphferhb.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2eugagdic.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2usnvwajt.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2woiaohvz.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2tcynxgkw.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2kcgbshun.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2qzevciaq.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2oxotacyf.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2nwgabnrq.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2htwucjtt.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ekiwvakz.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2qyuybrih.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2aqrwpkir.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2fspfeycg.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2wceozapm.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2nrfugfyq.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2gbcpcvik.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2onmxjfst.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2qswqwutv.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2vleacifa.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2yrbnwsef.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2ljqhxxbq.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2bgxxxyej.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2wivnuitt.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2poduucou.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2dmzeecoq.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2etiontdw.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2aavgqimf.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2nqjhhvcm.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2bbxqjutj.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2pivykbhr.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2akmuabin.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2mfhgtnrz.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2kqavpyom.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2kmcelism.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2hwafaahh.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2lqiygzpu.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2octhdrta.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2jbmdaejb.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2wfeommpq.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2wlbpcnbg.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2pqyxbgzx.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2lnmiylqs.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2qmzniphj.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2ekuxjjhl.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2xpyfogeh.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2vqpaujtc.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2qwhpmnbw.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2mhvtjdqt.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2uoebjuxp.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2oviqxmau.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2ehwngaws.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2qqxaywqg.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2gsqjdwki.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2ijwqheng.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2zrqggmxh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yctyyusz.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2tnzwufya.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kgjavllw.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2nhefiiyn.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2rrwkdfih.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2mdrqjwag.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2tzpljhqf.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2mnxtrneo.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2fghatxyv.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2omacxyih.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2tpglfkax.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2jjesrhxn.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2rbsvavwp.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2kquiguxy.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2bqifhdnt.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2dzbmyigk.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2sfjnhaef.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2jtcdlmra.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2grjuxcii.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2cektfbrh.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2fggydomo.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2gdlbzzap.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2hdiylzbt.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2nzhqltqb.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2fcinamvl.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2cjdhspbt.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2utoecomu.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2egwcwfxj.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2vqlkpvfp.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2sombspgj.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2hykdzioh.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2pgcyslyc.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2hamnatqn.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2hwmmosnj.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2iynqkusw.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2dhbxshvl.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2liivayhh.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2cnjzzwyz.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2imarozpg.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2ocfhbivk.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2rkwqwhte.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2jmlrxppe.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2ifqufomr.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2zgxioymh.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2myzggsop.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2hgbadcyc.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2xforszng.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2tdbflayz.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2lfneytjj.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2yoktkyqe.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2cjjctdyu.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2dbkljgdo.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2zohcddvr.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2ogrewkjo.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2pxbzxnwo.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2tbqkhcnv.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2jdqjxpfn.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2psuvbhwt.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2maflszwa.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2ezfjbetf.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2wafymrag.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2hzhyapaa.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2jvjgbsav.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2gargbdnj.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2yiuqswrv.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2jkkvfund.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2zmdkephp.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2nfklqpel.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2wyucplgf.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2pycjxkqj.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2sfrucbwh.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2cnvvzyvx.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2ztgkqdim.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2qprtyvyy.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2alwmwgzg.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2fajfmyin.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2nzeqxvip.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2dtjgzmob.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2mtsdljdv.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2mthcrqnm.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2kgaenuhu.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2bxhnomlm.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2fwnddnrw.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2vdqzshhr.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2ledmldyv.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2vdgninzs.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2bcqnoldq.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2sqyvmvck.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2mjizttxw.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2fhyzfppx.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2ltwjydft.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2nrneatwo.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2hssrfjtw.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2ivkusmkd.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2lhsttdkc.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2nptmrppv.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2yovepxct.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2qhkqmtxx.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2uhgpoouc.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2jlyoexuj.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2ppocjezs.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2jeejbgly.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2vdzyejii.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2haoskqxd.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2yngyeeal.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2uhfilwwy.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2sdwsadxx.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2zeivnahv.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2ptqicmeu.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2axaixrai.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2qmkixdkl.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2atabzsuu.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2gopppcgo.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2wdhyooxr.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2ipnguwui.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2tdhqwokn.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2qmjieeiz.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2kduervqu.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2vienrdmf.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2ooxtlfff.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2gfknawba.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2lxuptfwm.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2xefjxnzc.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2tbxvmvhx.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2fmgylxvy.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2brinjhus.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2dlyhxujs.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2mafjechh.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2lzzeqqie.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2iawxdrql.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2pfpgmoji.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2kjguejvd.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2ygrcagss.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ilhafhuh.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2aahvvrwx.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2vsfzsxsx.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2plrldgjx.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2vgzyvflu.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2hiqgagyf.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2wczpdonx.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2thlfbuom.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2cwpeuzve.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2cphswtlc.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fryitpso.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2ugdfecui.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2ypsbiqsr.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2fvwlfrmk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fgynkjcg.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2wnxiumnv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ugoelhev.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2pwlmwlaq.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2lfucnxjc.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2trkhihvx.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2hgezreya.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2zacufvth.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2dvsqqaef.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2bowgmgga.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2tkgwrhua.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2nvtdyuos.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2avuhgshk.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2ppvdndjw.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2kdujpvaa.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2oklbydhj.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2blglhqwe.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2fpgsbsks.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2oxvxplpy.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2vwpszxzv.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2leonpkms.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2ivunnkot.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2torqbelz.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2qestgzth.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2elrxcbhn.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2bqkklsby.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2fxpbdmge.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2gykwpafa.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2tkwbetdb.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2lzquyoiw.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2xqczlcmv.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2atbbzhrj.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2niwmdpsc.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2mnpwhmka.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2wbznnvbb.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2euexqnxu.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2ivpkoobu.html


<!-- 参考信息 -->