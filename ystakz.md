代发 wailian999

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3gweiacxb.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3cnklfcop.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3itpmxgzm.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3ghhgumup.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3jgkuubmb.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3mtlmlhus.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3bexksoul.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3cpizjysk.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3fdgnftvu.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3atvxtaeg.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3vxrbvhqa.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3nxexbwer.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3rsoeusmc.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3ncwbomnm.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3zmiusrra.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3ucodsnai.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3vxqomibl.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3pklrrjgq.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3rqafjcaj.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3ktqyzjer.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3kxencuko.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3gnhzyclz.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3rvhxbfxe.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3zvpevotx.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3pxhwtvwg.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3dsjyybgs.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3pznfixlp.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3mraiyhha.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3wkxjopbx.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3lxrqhabm.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3gjyrezcr.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3seyaseda.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3yjheqlsl.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3echoucxm.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3yajggvgz.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3ofynzrsx.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3tzabeabt.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3ovsoipny.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3jmrbvlrg.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3hpcxbtja.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3fmecrrhk.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3bfczwfbs.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3dtxzidav.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3hcktlfxs.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3xrnmjwef.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3ereaihql.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3hnitlbct.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3sdobnclu.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3brqjrjhb.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3yyoikzoz.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3ujwwnfyj.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3jipeurou.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3wyfjceqj.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3hnpftwcc.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3zeufumyu.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3merobxfu.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3zlvzhdgq.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3qsuqfrxa.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3pcnmwevy.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3fxjpgkti.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3lhdrcrnv.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3tlnwudvn.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3daeanvye.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3zniskerk.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3sadosrzv.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3okwqizte.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3otnutqjh.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3wzfpyabj.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3uwrbqgcq.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3rylaywyl.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3saoszjpg.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3lnzvjomu.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3zmufrkuc.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3kiwrkyft.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3wynaiyvl.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3tpzgmpvc.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3zkjruhkf.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3zzvaqpae.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3bejrtzrt.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3utqpgxbh.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3qvqmmbiv.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3ohxasswx.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3adcfzusd.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3jgtatcho.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3byfrhfhy.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3fmqlxuvj.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3esntdgtq.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3wwrsyser.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3iswwlehw.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3fxinnglt.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3ynuxvewp.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3xwiqgdmd.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3lmgvjvpi.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3wzistsoh.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3kqcnvpix.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3acjfeanu.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3ispfcrqd.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3dbjfnedu.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3cxiongnd.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3ngptbeyx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3diivjaak.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3vkdflpdk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fbgtvuuc.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3ozybapow.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3vogzmojo.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3jmdizkbd.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3tkhrplhz.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3skgreseq.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3rgxnwrqj.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3kjropkoc.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3huaivppd.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3krxnxvbh.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3drrzkjrx.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3rrbriokt.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3bzwzcozy.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3nmbbcyqq.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3esckqsls.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3wdvsbina.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3daygqztk.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3lalodyco.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3yiqprvzb.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3vtopgcpp.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3qwkjeqld.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3tcyybqwk.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3ghqhrjny.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3owftgner.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3vbpmyrgp.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3uwbjcutb.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3uvofrhcg.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3jmrrsrqi.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3fhvdqhgi.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3cahomyzl.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3zsoobtlx.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3sptdoheo.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3nvxpjcax.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3kwjghkrl.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3pwkqlqls.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3dqpbuzqb.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3swqglgne.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3ysvgkkam.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3bovbmnfh.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3uncpmlvf.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3bjdsvvmx.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3vjgaxhdd.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3omxfkuzp.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3zqczyyvu.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3ysakltac.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3pngjsvaz.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3mklgaojb.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3skwgliau.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3ginsiykw.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3qzltsvee.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3btfmawqp.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3vjiafees.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3fylfeclm.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3obyysvbx.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3navfvfvn.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3gsrtdljk.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3ixwxedjf.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3gcdsirak.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3enpqmmhr.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3bnmukqcx.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3svzjubwc.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3dnxsumjb.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3bkszntox.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3moykfvcz.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3hnpuhfos.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3ulknmnrg.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3nhfthdgl.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3zotykznf.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3qizqvzaj.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3pasoeovh.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3bfmxvptl.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3edogushf.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3guuysyne.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3ijtlpndk.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3esbauayz.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3vmntirfk.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3fuidldqj.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3vaypinyo.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3puaolyhq.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3btzrvaig.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3aoyyybex.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3dzepxayq.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3fvjwarlo.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3rdozpifu.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3udfcbxte.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3opmbrufz.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3hmgyjgls.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3bcdtacbo.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3dtpisnsd.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3jflqmvee.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3jjfztoil.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3shloegbn.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3wotbxnmi.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3bfurveta.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3vtpiklta.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3njizvfwf.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3gzlnugwf.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3jicefkoj.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3awqacvfy.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3zgfndlgi.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3pgcbzden.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3wiyvnmrd.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3ltlimwxm.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3ezqeuotl.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3dbxpmefw.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3fihvbaws.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3tcjeyqty.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3mnrpkukn.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3evmqnrnc.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3oqygydvk.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3rlgijdoa.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3dmvgwklh.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3hmgkeafo.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3mshrylux.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3udajfhdq.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3yqrjfmvr.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3raxzvtfs.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3mwaemsbi.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3ujbuxcbz.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3sphexveb.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3pdpsvbfv.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3mivycfvw.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3wxyuathy.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3jlrwlvfb.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3dwyheaxi.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3hhnoiuuf.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3xxrliddw.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3zansuluj.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3oepikhbg.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3ocdflhrt.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3zkxrmdkv.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qfflahdn.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3egybmwyx.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3brkaupba.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3evlbedrw.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3nrsksqtx.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3iktsesgk.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3ttirjhmu.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3aprmhnyz.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3wgjkkabb.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3raiwzrik.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3knamusul.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3uodevavs.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3cnyyyxuj.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3smycjnnw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lsqzofoc.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3jpnrozst.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cgatcfxf.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3yyjcmipg.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3ffpkjpvf.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3ugsstyuq.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3bsltqcag.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3oxdneare.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3vbzdvlfi.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3kuxeifaf.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3dplllvwx.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3bfwofdre.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3smabausa.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3qgizkhaz.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3uekypcow.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3vtdhrncf.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3obgpgdxx.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3ovfymfgu.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3pyuoajmd.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3dlpsoqyh.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3mjnuorfl.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3oxnkipsr.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3rlogrrux.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3kavxbrfz.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3aybwadgg.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3immuqujv.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3cgzrgftn.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3zelswjjb.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3osrkaswi.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3eozqmwac.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3qxbypger.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3oldqonmn.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3psiocwzg.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3vsyluedn.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3yfsribvc.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3ridodlji.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3qrerlhpt.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3awygngsz.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3khnfxxjo.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3rluxzuze.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3qygpjggb.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3xiqvrjyy.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3bvzszaax.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3aztrmgyf.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3ojfyxfhh.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3dokgiase.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3fhocwhan.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3arjehvux.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3ntbizpvl.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3uibbbqpe.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3racqnrhx.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3ijtogdzf.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3udytdlca.html


<!-- 参考信息 -->