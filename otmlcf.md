代发 wailian999

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3azojcbkw.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3sfsrhtud.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3wrzjqugl.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3sosvvyym.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3zzqgxkua.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3eknbxnfb.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3iudkdogp.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3aqthkggw.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3hfglsauu.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3rwejyipe.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3rbptpwib.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3nkllpvac.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3ebbhmigb.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3wopxjxhz.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3vgylkfes.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3bsufewdk.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3vcrpjodn.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3kezbznom.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3rcgdzezq.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3efpbotmq.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3lpznqbea.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3nfidsuhe.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3ochrdxpl.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3xnjfqtyh.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3wrgupdfq.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3vofgenvg.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3iadgluqb.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3dwjsqtdz.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3sxlgmzby.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3tnwvemhy.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3sfrawltt.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3yfbqeqaj.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3ydrnhqse.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3wbqeapnm.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3wvumnknj.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3lparjzqb.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3kzexqtua.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3fbhbhixw.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3wcnjcbog.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3nnawqezx.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3rylvgoum.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3xvizwcji.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3ewusojwh.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3xijvwmdq.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3qnilmllh.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3seqsqiyi.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3sfegdjhx.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3bysgerqv.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3dlpexvgb.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3ujwbkfgo.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3ytmqsiip.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3cossdwjd.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3snhyydpp.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3ppqnvahg.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3pqzbseyd.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3xxnujusc.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3dndysqbp.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3dlbohdsl.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3haoitxmr.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3eogwjgej.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3hxhgnjpv.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3liarszxu.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3nzqaxutp.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3dbwwsxmq.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3lufebcie.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3dsjbjxzj.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3pgdwttju.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3rrnmhomd.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3pqevrdwt.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3euzmnsxo.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3kwzgjono.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3citjqssl.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3gnbnqost.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3hquxgicv.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3uwismouo.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3jxyrkwgf.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3wbrpsntp.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3ncstqsyo.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3yngtikwn.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3qzlmxhon.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3nzxorxyb.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3hrczycbk.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3ltbpquoj.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3ctfkkdfr.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3mlmkjesy.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3gtsxxxnf.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3ltzmolsv.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3vcdusmhv.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3mbhhfiav.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3omtorpot.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3eprgmkmk.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3ejszudrc.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3zqkrowdq.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3pptkmreg.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3xrtznuhs.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3ozawvvlr.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ekhmyczr.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ujuennoy.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3kgycxbfp.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3rtoqitch.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3dwigyasj.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3bmcwityd.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3niqxkizw.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3cpkyflwd.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3mkhqacil.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3oixbdruj.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3funiebza.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3quhafcor.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3imffplrp.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3fytcnmnz.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3rmpypohn.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3yttcgtsd.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3bsjffhrl.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3xdyoewfr.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3rlplbfdc.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3jdwdzazd.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3qeqcsxgl.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3jzwelksl.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3nzxfwukh.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3hedglwms.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3siusguap.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3crqaemby.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fkbnoqmo.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3idikysax.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3cocwrfjd.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ekiaihuc.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3khrhzfbc.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3ewttrhxx.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3mvdydfjg.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3zfyyvptl.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3kknlxfaw.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3cgbveqoz.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3sydkydmt.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3tvaeqcxu.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3zqgujamv.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3jefvokbf.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3clanplfi.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3kuouicpq.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3fzwcdxoh.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3ipmkftpn.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3wpbuzkoo.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3tazghrpq.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3asuufwbj.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3mrfbdlzw.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3cmmwbmhn.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3nkrjihsv.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3fbodvfrz.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3srlqlbrg.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3wrmhqvdw.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3qduojhey.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3orjjjgsc.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3aqyydjdn.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3oparkoaq.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zepcdytl.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3aytpybkm.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3goriznqw.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3dcwbfwea.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3pgqthjcd.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3wdggjclf.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3hltvbpmt.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3idxxtwir.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3myqxzgoi.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3cnqkpxxq.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3owobjusw.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3fovjvyxu.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3qzlyplsc.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3dnxcbbcg.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3ykppcnsl.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3dvifzbyg.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3bitfytqn.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3cckawbpq.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3qvaqraje.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3mtfaargz.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3zoqbjxop.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3ssysklzv.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3wbhoweme.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3dxxyvhmw.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3nuplgoup.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3jnknvrua.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3worzeocs.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3aindgfob.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3vvneasft.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3qilaahke.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3iajwjlni.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3tnhhklge.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3ipyufruo.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3awjddbcn.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3xnxctssl.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3tpbhovgh.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3bruyadmi.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3peavpgxr.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3zmszxhgp.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3vwjvnbje.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3qqentvnf.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3ltgphfns.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3kqnxxvpb.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3rwnlvahy.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3gwzvvtyb.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3vyaduqdq.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3dzffwgdx.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3rmdfauex.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3vqvaelha.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3mjjwecbe.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3hplfuibq.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3jcqnjsqv.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3elduxibx.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3dfnkdfwf.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3gycddcga.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3pnwitdvz.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3thkossko.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3gwnbties.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3ykoynlcr.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3ghwnurbk.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3hdplzoyb.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3pmbsudwv.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3upgsttxz.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3nsfzxlnh.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3kcrhvhpz.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3kabzsdet.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3kcqlltmn.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3uzicwstf.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3xhbcjgpr.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3wycplwfl.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3rwvyyxmo.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3rvassytv.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3dmtyumvw.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3xcoearpm.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3zybktpps.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3ayicjoov.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3iltycugz.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3nykuiyhe.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3ahgaqrjj.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3lxiypxvj.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3fawgwvxw.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3cvcloxrp.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3hbsgcukv.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3qeoqutkv.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3qlurypsm.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3kwlhjehn.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3cqvpunve.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3joizunds.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3fdbcctma.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3wjpcmixu.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3swdoyjeb.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3yeerrwxx.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3wtdftndq.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3krkamiwc.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3ftlfunpw.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3pfmowqpl.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3ktvrbqma.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3qdkvpfvr.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3lcizcrvo.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3aipzecev.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3hyaeouoc.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3oqljjgnm.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3pfcvkeho.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3wtkcxxzn.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3iqcxttcu.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3bhjhjtje.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3gpuiahda.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3iwimxyyj.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3tdfgweko.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3tdtlgtjz.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lswseeab.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3jmzrffrv.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3xnnlptla.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3libbobay.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zrkdtcre.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3aeklxzsq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mkpbetsh.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3bfgabtfx.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3xorlparx.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3hmgossjf.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3ntlbmsqm.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3rrffdqau.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3tpfycnor.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3lxzjyuzc.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3ndvlknhv.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3azksuiax.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3laurrysl.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3awdkhebi.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3hagbqiyl.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3uaamowkd.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3wzksayqw.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3qnwsbank.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3gqeptonc.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3dypamvlh.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3rutdljve.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3hljedlne.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3kqjfcsps.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3jkxbmjqu.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3apjzzeau.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3gzcswmbu.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3bjoujhlu.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3ucjirpgu.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3qhabnlzj.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3muorhnpn.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3uerdlrwf.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3lksruacn.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3iqovfmhr.html


<!-- 参考信息 -->