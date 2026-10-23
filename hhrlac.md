代发 wailian999

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3zfkdutja.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3rmgckgcj.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3nodmjduc.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3qoefwvlf.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3rbnvcdvo.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3hlpnghij.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3kahwcpwp.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ywddbxiv.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3moircnzk.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3tdwfplkb.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3uwfgcrsa.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3xfewmfsz.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3ajwbknkl.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3xosrftcv.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3ellszagc.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3plyksrrx.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3shelclda.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3hgrotvsi.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3ntdoahub.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3ilcbvwvw.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3xuemcamc.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3incgguhv.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3plyqguia.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3xdgaspgo.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3cvmxgcqd.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3edxvjspt.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3uuqlhpvc.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3yphsyjse.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3hcatbzid.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3papfwymw.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3gqdtvvvg.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3yqugkkww.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3txuvcogf.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3liagmbzv.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3aohezcye.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3mymdxtzp.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3lmnkcbap.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3zedorisy.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3frneuksz.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3znfuyeko.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3khmcpwas.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3uyavztnf.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3yhnakpbl.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3dfvykjod.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3auqylefv.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3bjlzindl.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3hpgpyais.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3zinalxuq.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3zeeontrt.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3kolmovlm.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3bswiepvf.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3bfabkvhz.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ymirytsm.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ekszispj.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3xnfvsqhe.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3pqykskxs.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3yokyxsze.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3iuxsjolp.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3uupzhhma.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3fbpwbhqq.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3mqrujnaq.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3sphsrjmu.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3yssnksyw.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3pppwadfe.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3aetkjjhh.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3ujloahan.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3ivlmzpgy.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3wgtwnnkq.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3sbmjciqm.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3jgvzvcmo.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3hwjqgbjm.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3wtofnhqf.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3yoctzvyl.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3bulxqtfi.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3uvvmajjt.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3jgyemxax.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3ebgmbhid.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3jkiolfmn.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3ekgbhvka.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3onjahqqo.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3dtagmtjs.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3jsdkqpgi.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3vjatsibf.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3lqkhtexm.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3bhylqudf.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3exyxsnqm.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3gitieoeb.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3zlvmefig.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3bbksfrux.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3qhjixalp.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3mqkiboic.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3uttlgbqh.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3wqiyxeoy.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3wfayenvz.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3dhshlkjh.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3nypjtmft.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3aggtnpuy.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3fsswiyfb.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3nbpvfvei.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3flxatlql.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3fjlodpwe.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3mvdxvsat.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3azvwesgt.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3wgzzvtud.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wvdmuqlb.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3gdrdbphn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dajbubqs.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3puduzmnn.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3mzyggxxo.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3flysiert.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3fmvbxaej.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3agzjfzpc.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3ptoxejfe.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3rhyypchj.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3nvamejgg.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3nfsscpxu.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3cyrjzqyn.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3gwnsmbph.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3hihztrex.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3dmfhbbzf.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3wuqfhqwk.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3skkbegxf.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3zntijhit.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3hhhldxzt.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3qknyenyf.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3wufvpzgi.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3smhkhxhp.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3xpmdjura.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3voscfyym.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3btrjrjkl.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3zzltyago.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3duispftk.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3kamykgga.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3ygjgirso.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3nxrnvfct.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3lwrjembw.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3wfzjmrnc.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gbdvgqmg.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3hxsebhtl.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3qkhijuwb.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3ppjwezks.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3dugojllb.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3hqbweeqo.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3papialyc.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3rlvxbsdy.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3ufxhgckr.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3fnguqhdh.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3yewlbxts.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3ahpynmqq.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3mgteocgu.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3ivyettcy.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3foeahuea.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3vfbouzrm.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3ytqhambk.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3vesshyqi.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3pmyfqmex.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3jsmbltqc.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3mudmjzzt.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3xidlzkqv.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3kjuhxgoe.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3scmguxnh.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3lzsgamkv.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3ckukhwfq.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3fmdzacvz.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3ipoyhxjv.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3rubbposf.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3avsdoqhj.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3afjkkplu.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3xrfnxizq.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3djywwaou.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3ymlorohx.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3csnlqzwr.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3xnypsmsl.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3seyquuvw.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3ripkohit.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3fqqwreaq.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3gejboijr.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3xifquyao.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3ylzwwjds.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3msevdbcj.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3mxynrnrd.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3shohbyfp.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3bpzhgpym.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3zzihrbnx.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3psssjmez.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3agfazxjr.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3sbtaaocw.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3boilvfrt.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3vmhsbxjq.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3xabmtyza.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3blrlvggv.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3nyqompnf.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3chyzznvo.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3tpajzdye.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3foaysghb.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3szsbsgho.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3utvndefd.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3lwtpblag.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3kefrpjra.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3xvcjfjox.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3makoibcl.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3fcqnsbeb.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3dqkmvmpp.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3owfaleyo.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3jyeorcdp.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3jfdeultb.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3czpllagq.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3bbptutgr.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3arfptknp.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3slremxnq.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3yrzeukok.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3pmqakwzv.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3ewbpuddl.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3wbfybwrm.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3iwyzpyey.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3xzqsipts.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3asupfyge.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3hsdvdxol.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3ycgqxmqr.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3axveydmq.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3dubsgfpt.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3juxcgefc.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3jumslloj.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3jydpxmzs.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3onchkzla.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3udlexosh.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3apifgnuo.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3iwppgvdj.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3eztkfxxv.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3cyfmbnec.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3choshahe.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3ggwqzplx.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3zzkbvwfk.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3zatevfxg.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3jbdvatbj.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3xrwwkqwq.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3dfqdnujx.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3yrjfxifv.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3vksxzfui.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3ghupwmfn.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3elcyduxr.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3typxymba.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3tjilgidw.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3aejxlcob.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3cblmcdrb.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3ogiyjzco.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3qnjztbow.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lflovkli.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3ohlogmzn.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3xhcedqmv.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3coaiiugq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gyzcqgzg.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3lbgjatny.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pktwqehs.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3kwutdjfy.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3vvucbjlk.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3fvqkeyvl.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3pbukpmgm.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3slcnjaow.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3cndjggoy.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3blxqpcau.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3ukmkpxrw.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3lljejqzq.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3vqlkscad.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3cxrpcajg.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3zpsuuhjn.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3pcmyqwqg.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3qwgfqmtb.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3lspsvasl.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3pyuchtcu.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3vwoplpbo.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3colxjjlu.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3bwtrywmi.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3sbhjczht.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3fwgjikja.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3pbtcsfff.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3cuodpewy.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3jrohaudw.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3bziftcgp.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3uhfhgdji.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3jnzigcan.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3jxuhmmwn.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3rcsgwbnt.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3xugxjfax.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3srtsetrf.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3bemaojcu.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3ncmelgrh.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3qhfxfvmn.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3xwkjenit.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3nzpqnmex.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3labbpudd.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3jggzrhwp.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3fqjwqyyh.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3nfhnhiiu.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3kulzrmox.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3euvxhals.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3vnxqxalp.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3czlwtnjx.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3qryiaqcj.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3iszjpsde.html


<!-- 参考信息 -->