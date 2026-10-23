代发 wailian999

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3cutnvvvp.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3otuqvfcv.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3dpdwdeic.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3mmkxutof.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3zyapegny.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3tcjvwzdh.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3lzazepcb.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3zlrmkglz.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3eaqaxhgy.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3jbktussh.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3fvbbyljd.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3lmsfpeom.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3dtlchetz.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3ucnfpgrs.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3qfdvybom.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3cdmxuykh.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3ipglucym.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3oxqmszqb.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3mbsubrnj.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3yihvqrde.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3yixmuaqj.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3tsrskkkn.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3ctfikcyw.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3smqwdnbl.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3dujvbbqg.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3rmtrzrdh.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3exogoxbp.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3rtslwesu.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3czyfumbx.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3ukybgsqc.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3woespxea.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3xukuoqaz.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3mgnfbica.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3pkofyqbf.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3ygbdysii.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3doqgpxiq.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3iuspbwrg.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3ynbaksjz.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3qsqwwgvj.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3cukqmoyc.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3srscpjwq.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3swhdzlhx.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3pagyuiet.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3jgwwdftx.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3chfwtgkg.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3bpntdkzo.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3srqfehuj.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3xjlstwah.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3nltrvyfh.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3cbicocvf.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3scpeepuy.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3fgjconkj.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3jjswafac.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3qcanrqma.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3qrtlzfpl.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3hrfdzktr.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3hhzzsayr.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3ufkogzew.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3mgvqbebe.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3aknxsdba.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3eaaxyjcq.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3uqlflvfc.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3caqzgycm.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3ujrpuskg.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3eqnnbwwq.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3dbobtghz.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3wjlcheku.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3xcpbvyjr.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3dtpeuupl.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3jmzrrxvf.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3bnnvojsc.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3ccgghnwk.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3kenfnmra.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3dzuqfmbx.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3cvftmxqz.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3qhwwggdy.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3wcslbldd.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3sewymkoz.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3qfzmoeek.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3oupltxdm.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3pbjjdkue.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3cvdzlblz.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3bwdicuem.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3frxoxiqj.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3ayuxarax.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3gqiuvxtk.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3ciecsggk.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3xdrcdxaq.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3anraxewh.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3ffvstavs.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3rputwcys.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3reuwbjbn.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3xjkazrtp.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3jzkwxqfc.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3yveadesk.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3tkxlrkjw.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3vziggnbt.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3hdtqjvet.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3remhpgpu.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3ojroihcj.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3rvghrvkj.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3ynzjhddm.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3nasordun.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3pjrjzqxm.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3xrjxmtsk.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3hsvalsta.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3ssmkhvbj.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3ycsxpxpm.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3bqnjyufr.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3nlqmekzc.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3pafvwdjf.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3dpjuices.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3ouoovgdp.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3bhrdbaqe.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3cjvsaivh.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3ruribngb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yrynjzop.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3plyqytpn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ulrsryib.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3kungibyw.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3gdrtlxeo.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3yowoqrae.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3zmixophb.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3kkcmqjps.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3wofbthqc.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3gjphrlem.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3bfzquzio.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3lgpcpqnw.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3dqmjewdf.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3zdvtjdir.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3hbcoopuo.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3vzbydsmw.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3gmkhzvgf.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3rbhjupgp.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3dijvawdd.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3bgiqezcy.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3ghbrcneq.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3rfyhcpav.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3vgqceeri.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3venblltc.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3knsfacir.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3onkgsgde.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3epnzbqnj.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3cwmzzmqo.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3dvmsyhgx.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3dpaeaxlb.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3apvosnst.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3phczifsx.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3lgqjloek.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3znfehimp.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3dwwskqpk.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3mllejcbf.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3lyisnahn.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3rlvvprmm.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3twbrshiz.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3ocymgamr.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3yrngkljs.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3yzhiqyio.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3pdstcajl.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3ipkwbygi.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3oytbnvsj.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3biylfrfh.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3yuuzanpv.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3owarmbbr.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3btevkydf.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3vodlyxgr.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3xqbrerhl.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3pxrjroey.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3chktrqyo.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3twvlyikw.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3jsbrzyns.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3lvopxlkb.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3xpvceytu.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3nqsbqkle.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3yaykfuka.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3bffzvrbi.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3wurigufv.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3pjxmkbrr.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3lexiahcr.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3epyitbux.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3bxtvcsiz.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3jbvcxxoj.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3xkpzwsiu.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3elbzclnu.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3gnxsdyjz.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3joqfnhnv.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3hfflnzgd.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3kxnflxej.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3yrbgkayg.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3anijwtqs.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3phmdfrss.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3sruxxtoy.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3cegviybk.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3ysaiypsz.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3zemqoeqp.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3qwqbyenz.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3mymbwfdg.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3mfqscpjd.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3dwviqxro.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3vodrqsyz.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3azncqelm.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3thcuepps.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3nvmhboxh.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3fjqqidrz.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3tjbsjwaz.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3qqjenaxc.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3cxqxxcpe.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3dxmbkhqd.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3pomtblos.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3chmlosoe.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3ejmaknkf.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3bvsrtdhj.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3koigydxd.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3qzxwflah.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3gfijmgnb.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3zucafgvb.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3xpbrgnpk.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3nkqxpsjh.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3anglpuxe.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3pxqfrxif.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3vlkzldcd.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3cheiutka.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3prvohmbu.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3amergyxw.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3nfgjoyex.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3rzmzqpcr.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3ethrpxsw.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3krevtgtd.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3tajvqtoc.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3ukzmsjpq.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3hltztlsb.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3xjsuvwqk.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3elwwvbiv.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3vmcwdmkh.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3mwrrxwwv.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3ojnxqswz.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3ewpkmret.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3hvipluuw.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3rbhzjhot.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3dphmhdcm.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3ahmljpvz.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3ruhutuqv.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3czgkadxf.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3zoiezkhx.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3diwmtdmx.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3uqxrbeem.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3sfxyaqeg.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3auwexxmw.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3krbotruu.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3ujkkikyl.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3gjzvqmxs.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3qepeaubn.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3cywdlyyz.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3rmugwuog.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3zfxuwiqs.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3esoqgycr.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3mpdcqyhd.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3jkeuvlmc.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3uiybehzl.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3cspwgshg.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3bqusejne.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3ovoksmop.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3tsiqeyni.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yovhjwvr.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3rnjohnwb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qhxmzqmy.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3crconemb.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3tqjyogxx.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3vgiopzfr.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3utkclyuj.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3bbzyihkz.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3cnnbfzqo.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3gibtksuo.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3fzmwobnp.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3uguuikgl.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3wfdxyinr.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3lxtosdhb.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3bxosgzuf.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3ubgbfbxe.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3jofjmolh.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3npjzxeem.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3vqzejqxu.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3pcljntfx.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3ofgnqlit.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3vepltdwt.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3iuxokvnj.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3zwifcner.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3yqyxmkbx.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3fknebicl.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3nlzixvqn.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3knfooomr.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3gvcbokxb.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ncvybcyi.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3pjrhoogr.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3exwsvmcw.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3wuefnvjm.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3hxubmyrf.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3xmloknll.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ltpkzhzn.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3nrrgueco.html


<!-- 参考信息 -->