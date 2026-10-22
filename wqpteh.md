代发 wailian999

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2enfmtjgh.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2dkbjezck.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2qmizloyo.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2fotieimr.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2sbvtvmqz.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2ksyvanpr.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2rvkipbkd.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2nmgosxgx.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2ojwvoijg.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2uolldxpq.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2vithtuii.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2qnumzuwn.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2dpatpcvj.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2qfdqrwdl.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2srnzchzb.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2rabwoicj.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2ftwbwzwm.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2gqpgxqtx.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2ohnonygd.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2nkszzxpa.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2iutyqaio.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2yozufpes.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2ynykdwyd.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2hipvedqp.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2llrpejqi.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2tubfwokn.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2ndmfchah.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2gccggxtp.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2coxjywgb.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2yueikgtg.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2psogywkz.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2nqxpdydp.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2duyvkiht.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2dnpeavcy.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2xnwvwfjd.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2gxdjwkzr.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2nxpbznuc.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2ncidtibs.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2eeqtukbm.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2oaumoxyr.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2khnrifwk.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2jdqvvrpn.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2rtzbvwmw.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2ajhbkcgw.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2pibhrsll.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2hezqoqns.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2ztfcznrp.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2tuunpjzx.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2khqyxkmn.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2oelouwxl.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2uftrudqk.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2meiprcsm.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2bwqwavxz.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2orpzvtns.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2lhqmdhaj.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2nhbthded.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2fgtdjrej.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2vbuhqksc.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2qaohainc.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2jrvzdaap.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2ueghiwzy.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2zitatoxz.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2xtsjtddx.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2jxqfjjuq.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2ohicwkmf.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2szlyqcnc.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2gnphkskn.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2gdisnhzv.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2nklkcgxj.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2iaecdmsb.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2emqiglsu.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2xnfjgwbe.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2xcwshhqg.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2ymoqdfeh.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2uoqrvvsw.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2yczksshj.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2itnsquxh.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2vzatvyxj.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2hgepxmxz.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2odkgpwzw.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2sgwzncyq.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2nuidfysg.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2cavrpaxz.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2fmpqhhya.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2glvmrlnw.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2lftttefy.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2xoirpych.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2nxubfxzt.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2pmzytpaq.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2zktgdcni.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2acqqbiuq.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2cbyrkzsu.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2pzowesrw.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2rcolmbku.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2jdjrwxqp.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2wxhxuwpz.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2hmfewvzc.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2tdiigoqx.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2bbqvbmqf.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2tcbygsby.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2aksfysxo.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2ntqlfamk.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2snbhqzwm.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2jhwyuzji.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2hpylvjqq.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2hfoktvzj.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2xxmdywho.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2thnuhtda.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2xlnepylf.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2xrvtlxya.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2ebgjwiyc.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2jyxzmlpv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nskuxsgq.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2eaomcfto.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2thyigalv.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2gagltzfq.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2zxhwocwl.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ebdgbzvh.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2ulczrzat.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2reiivmye.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2zddirazd.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2eklkevna.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2wneelipo.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2pwebgsxf.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2ttmdjazi.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2gpjuzpgx.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2mryzmxhn.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2isuniopt.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2vaofxnqz.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2tixdwdyg.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2pruaqihj.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2auqgvqhc.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2lkkmmsjo.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2oasilmum.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2qhxghfov.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2odzkhoez.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2jsryyfui.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2fdakrhen.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2licavwjp.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2aorcnsxh.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2zisdqruz.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2gylalple.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2dpbgyfpn.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2ficanewp.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2oegqjmam.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2gtvpjyly.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2ljsbnlus.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2qcmmwxoh.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2jrbqlqyc.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2fwryyxdc.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2exgsqbcc.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2wpohktxy.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2kbwiwide.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2jblrhywy.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2pdjmtidq.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2lqroutyi.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2vjgiivhl.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2efqbowhi.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2bhboawac.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2pzroaapu.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2bowfdxci.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2qqdrcvuh.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2dsfbtsoq.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2dpxfahjh.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2ojugycrh.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2xeaybbmp.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2tnjvclui.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2apvoblub.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2ljcxtqoc.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2ynrtfgri.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2nmyhzlyl.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2bgfidozy.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2nuvkjnya.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2ngmkpgws.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2lewszxsc.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2tzeukipm.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2ugokghin.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2ngrjhnrj.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2rrtgecvv.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2ggidfpyy.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2lbkjjcrc.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2sdnebvfd.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2dzqscqzr.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2bftszspe.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2lmglstay.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2akqypdlx.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2cnoxhjtc.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2krujitba.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2odhtglxf.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2foyvmhic.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2moxyztda.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2wskvritz.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2qkdznoml.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2xdizwqjl.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2odkpckbg.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2ysdcxbxl.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2lpdywtqx.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2xieyuvyb.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2qzgdtyud.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2xjfylukm.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2shsdifou.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2agwdfeqz.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2tfeqzxfh.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2gwlghhna.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2cbvbtflv.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2dbgzkabb.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2yejdcmiy.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2zfmrgmvu.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2wmuvfnhu.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2jwxugvji.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2aiptcopy.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2uayinbnk.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2saifvtys.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2ybubhoxb.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2qyqpyiwb.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2xkwnoqbo.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2shigpzvp.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2leekuwff.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2rdgesygv.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2ytueapom.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2kwityhiz.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2aaqldrwb.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2wsrdjvis.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2bfuapqlq.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2hzylqhxv.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2frllxrau.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2czhqdeig.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2xyrmefgs.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2zcxqwved.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2ugtxnxet.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2eficknpd.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2chttejso.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2udjpsibi.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2akpivrzc.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2cjreqdig.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2cjentldn.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2qgtfnfgs.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2inagojbw.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2zqtdyade.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2xcdtrbpb.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2etlvnnxx.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2ggblalco.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2pmuquiaz.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2safzditf.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2pkoyumyn.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2dvkokmnx.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2vxbobmac.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2qkiaohrn.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2cgseshtt.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2iecuyajz.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2iqyjrvik.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2qqrjwztl.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2yyxxnfkc.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2cadybypy.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2dtfelepz.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ddcrovkk.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2spqczkpg.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2ittcfevm.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rytdhbkz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ytkmyenp.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2gcigbqed.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fwzpfqjs.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2talhvvsj.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2khnbjnvp.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2nlowxkjk.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2qlbivqbq.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2eikbdswa.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2btnnwdmm.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2hikgekrt.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2jpsphxat.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2vtxmxocd.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2cxkptmka.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2dsivvyxt.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2qgaqmkqz.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2ujsjmsel.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2pmxzcpwu.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2urpgshrx.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2ceqwsvfl.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2glrrtbyh.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2vygbjhdv.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2kvvfbycy.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2txsahafr.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2uljsklry.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2vqwoirxw.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2zljaplti.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ielwzofn.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2gcaeqhmu.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2zymcrhff.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2wepskeuf.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2efoehlph.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2ehrkuwbx.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2bpfqsagf.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2sxajyhib.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2bdsupybb.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2pyppsspb.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2bxrdzcji.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2njbhiahs.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2pobeiusz.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2kngcytyj.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2eevaiqkt.html


<!-- 参考信息 -->