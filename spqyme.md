代发 wailian999

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3apgnnhma.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3encgjbux.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3wcbsykfj.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3aislokcs.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3pkpcsqmt.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3xyizbubc.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3xyxibdeh.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3mypgdluw.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3khfjfahx.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3rvjbkufb.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3mbkycegi.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3jeueaqec.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3pkuqrmtn.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3rgwyupkw.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3yhkhkypz.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3hboassyg.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3rkwaksey.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3gpnfokdv.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3vzvmrqge.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3xfeaugbq.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3oxxxbswv.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3npefytbn.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3xlqwvnnr.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3ewvofuvq.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3dxjjuzwu.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3bnixmvqc.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3ntxsstyu.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3mmevwiyv.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3jvclbiat.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3dgqswseu.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3eaowhzgf.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3xdqlvlxb.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3omtbpvmm.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3pahfrkif.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3rgfmprys.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3pxpmvcxs.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3widwduds.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3ixfokeng.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3sjoxvijh.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3zffyjwuu.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3xbbwurvq.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3laejpuqa.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3vsimpgge.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3yhdfqmym.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3atrxvsji.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3ytckvvmj.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3dpfoksld.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3biundbnc.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3zgtlvbda.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3tjrafdaw.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3eaboftif.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3egreizfh.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3acwrmaxe.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3fumtngop.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3wrcipsjg.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3nhzyfydm.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3eztmivqe.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3jjiqruox.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3dkoftnhd.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3wkkgpezk.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3hhufqxch.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3ddsinwjx.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3zobrwnxc.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3yfwfmysd.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3xomzcvrq.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3umluwgub.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3meeskarw.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3swhozexp.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3qismxasi.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3goqsxpkz.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3hbtfwxzm.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3bgpmsiay.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3bllezntr.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3sianmhbe.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3uwntjyiy.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3oxmnfxzq.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3hauygeuk.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3tbuawuto.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3fwtrkklf.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3kpqciqyh.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3owrzgels.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3lziqbapf.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3zllnnoec.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3wvojonce.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3wopplpwv.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3flladvyp.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3ijotoklc.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3qxlmumxs.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3ktaprpqy.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3nuaymfzv.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3hucxowgr.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3rnbrxqvw.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3lfcgjees.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3digckija.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3dzddgqku.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3lvzkurnh.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3jlvdhphh.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3lyfwdsfs.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3oiswghrr.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3wcpxrqwu.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3ybasghow.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3uqchaepw.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3ykpcipro.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3qgaqkxkm.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3ohicbuxx.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3qrmnbser.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3bohhmzfp.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3fqjvthzr.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3qekbnidr.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3kalnygsd.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3jrguyzut.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3pillqaes.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3nvicjdeh.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3kftqjmwl.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3cyyfeaew.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3xlrpyezo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dageefie.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3cquxrovx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zsyoyyyd.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3wftfocae.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3egjilosf.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3xjplcxnt.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ofbjpucr.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3mpqguila.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3qvftygvb.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3bpyvifmp.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3hcyjzxeu.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3rgxvrrtc.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3jxbobige.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3jkgevjop.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3acybggiz.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3kcstuium.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3cyzhkjwr.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3iwhqgqci.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3uqflswkn.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3llrfdxim.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3qeflbbdh.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3vrevtyek.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3kywwvthl.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3vjmhclkp.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3urtvojor.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3wdgqgitl.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3qryfukgh.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3jnkejnkm.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3fwdtbdcc.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3etptvecs.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3mrocbgbb.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3milrjfdc.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3weqmsxdo.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3pechldlo.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3okiptnsy.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3mbzfzaxt.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3moyyyvfg.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3nabixvbb.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3kxkpgkxt.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3gzuyixiw.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3lesqcklo.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3odkrbdsz.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3mfhjbdnj.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3xpkklfkd.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3vqbaodac.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3hppepijy.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3dbutmahq.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3jtmfzlcu.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3wqwlbxzh.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3gylzqvid.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3npjnpfha.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3txiiuqth.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3jzbmaqrg.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3eajcklkm.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3zgdjgtad.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3nlpiglav.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3jmoseogo.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3uqwvxrtg.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3wggxnwzi.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3iauyrvpt.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3phzzgtxn.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3uuzqchzi.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3hkmuxwqn.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3xebbzdxb.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3dpbeixdp.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3quzcwtla.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3okvhnqca.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3kdmkyxdv.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3kndntjih.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3fljyljsv.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3junwiezd.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3cgqjpesv.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3zvzlnwsc.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3mvvmghvm.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3cnlehgmb.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3zclzbrii.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3iyqfttvp.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3yrsirysb.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3hgulsfmt.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3mvfkqbcs.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3ebewyygj.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3gvxwjgvy.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3fzeamjrh.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3wcwvxerw.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3uaxyosmi.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3goxhawim.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3amkidrcq.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3ygmectza.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3cfwalzug.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3ulrpwmmk.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3xlswtgll.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3jwpyjycb.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3mwwwmsfd.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3dahbdwnq.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3nizsjzju.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3tqwkmzti.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3sdihdyhd.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3klaharmi.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3bwpazuzb.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3ffnxaiii.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3blizmxlr.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3tuyqznoh.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3lnlcwrdq.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3ttfhyhfy.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3rzpijnqx.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3xedsquat.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3qgobnlsm.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3jqfkqdcv.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3xyotlmkn.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3jurnaadu.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3fkctvaoe.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3kjivcrxq.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3emspyuvy.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3kbopjewo.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3cdkqzbko.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3yeurpcpx.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3dfipvefo.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3riohggxn.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3qiabczam.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3alvsikkj.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3yyffvzxm.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3rnfzmcvt.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3jpbaylnm.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3zyfsdfgz.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3erqiypwr.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3pnyyvmdx.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3lcmzehpo.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3zmvloplc.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3sdcfwivl.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3drhdchnm.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3rhoogvuz.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3sjisytqp.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3sqoawekq.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3rpahzflo.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3ftxfrjip.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3txttsjpv.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3ipllrhfn.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3mactmarx.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3jlnkwlca.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3apgvflky.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3ycrvczvq.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3qfxffdal.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3zkugriku.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mgkdmfso.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3siypybci.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3wioatbuj.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3tahrqqnx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bklrrioq.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3dwsiyfkn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dlqjgxkn.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3wtkffwsj.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3twczmgxf.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3iersuwbd.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3qvtyebqe.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3crhutmuc.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3rnyxlghq.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3bhygsmtm.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3oamryiyw.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3uwowpcpm.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3ycazunpb.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3vactxgpy.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3jbwweoyf.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3zmgzhxiy.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3ulbzylgt.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3wjqvbovk.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3cewvoutz.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3xikdvlma.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3axxunrhf.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3jgwwjelp.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3tgmzoosc.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3aelbpolo.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3ajfueryp.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3bjvcrepc.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3pfpnoykd.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3hjubzeqa.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3hempihhb.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3odcpxpta.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3mfafhwyq.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3fctdiqcy.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3rtbcufbf.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3pvatntdn.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3qbyshudx.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3puxnqrqu.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3jkqawbcn.html


<!-- 参考信息 -->