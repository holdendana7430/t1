代发 wailian999

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3cxyltpcj.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3liufeksq.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3vuijdwey.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3mjuntisk.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3mbiznzhk.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3qbpirhhq.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3orlkjsxk.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3gpppqxpi.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3lppxvfqd.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3sujbnyzu.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3vauufzwr.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3byfkubdi.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3mpstskii.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3ccqrodeb.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3ftmofwry.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3mrhgdspk.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3ebdutoqx.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3hphnrxxr.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3edryihdh.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3mdkzibsh.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3rijelren.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3ggwephwf.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3vmtipizq.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3japvyrtf.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3rydoyrvj.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3pkzinfug.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3flsjfhxz.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3gzshvqzp.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3fyuimkmn.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3nvoqshng.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3ihoyfbsz.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3uxfqcogy.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3ruqiodwu.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3rszsrzah.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3cukxzgge.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3dfaelrcp.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3lshhvvab.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3bwolzgib.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3mnxpjfkh.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3spxvuneg.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3fsjcknzg.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3haxrqkjv.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3tejhesnf.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3jrzamune.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3mcdboghf.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3emtqfrpt.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3lrnrcqwb.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3jjuizsln.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3xhfgftjl.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3ggxtpmyy.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3awsswwty.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3owlqlyyf.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3iillcrre.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3bvmxwpwp.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3cgraikjp.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3ezgitlal.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3dqcreoge.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3rzhysdvz.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3knqgkmaq.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3tlwrezyq.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3ntifumiz.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3uazrgcuc.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3baqdfrdf.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3occvypmd.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3asgrhxls.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3zppvlrhv.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3cwnqxobv.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3afczlhkr.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3hedvyrxb.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3sqvjybrg.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3fkykdumt.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3jvtinnlb.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ltlyfjcj.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3rmaovarv.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ffxufuwq.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3mxkbwzgg.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3uqogmkvz.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3qfmwnzux.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3wqeibmof.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3jihahdbq.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3yxjurryk.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3gyakbteq.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3nejvrpeq.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3sqcxjspd.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3etbuhzec.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3guhyqnys.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3gsiophmp.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3jbhojipf.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3ykqtrklr.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3rfygkrpp.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3tagkchcv.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3lpqbfarr.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3szyjfbkn.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3iboicujh.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3afvrtnls.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3mvipvxot.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3kmygmngv.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3kztgtoeo.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3ssrrnntt.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3zgedzyzf.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3guwllhur.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3knjhdqtr.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3eoiygofb.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ciaqtsqe.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3gxbdgtqj.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3qhefptar.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3squffleq.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3zsorripo.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3gpwhrtmm.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3xkqvwydc.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3igupvzlx.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3lpjtuhlf.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3cblrbmpd.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3bfwtforc.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3ngvuyfhp.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3ellvkzqt.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3txgyxrot.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3hcjmmlag.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3qwsyautu.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3nfhqcxjl.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3cpwjdimy.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3tmwqgtzk.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3llpzfeju.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3qvczacsm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hibmnduq.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3huxfwacb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wasjafpi.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3prfulsmk.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3rggrkazq.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3alfroqjm.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3lekokgne.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3rcptcegx.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3qhkdyshs.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3yarrcxex.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3somltqtp.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3zyqdervs.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3mqbhavpc.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3ukbsljrv.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3rvocexzi.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3oqtakvhw.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3ujkdtmys.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3shymwdkw.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3ibtqheql.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3mryhqzil.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3icejnjaf.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3imrzkgkw.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3wtkylbnn.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3wmxdcbgu.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3otkvteaz.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3wzpfzrhk.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3aawiydel.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3kxgyfqbi.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3yppobpqo.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3prybjtgi.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3vsqhkwut.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3esxaaebq.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3olgipnno.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3hprktify.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3wxcccnlx.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3yhgjpkdl.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3whcwqggf.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3fdxvucdf.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ehkqrnga.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3hesurtqc.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3lfasbjuy.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3snzhbynb.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3lfeosiep.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3jvezvqvs.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3spbxrsjb.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3enhytntd.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3fevihnqn.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3efmxdyhh.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3trlmypyy.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3ocxakrrs.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3cfaoyqbu.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3mdaarnax.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3oiyyjeqe.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3tjjgyuqt.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3wjuunvfp.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3wnkhqidf.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3lrqopsei.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3zxsyydgv.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3bubsqvkg.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3bjbkyspl.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3uhwccwin.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3veeremei.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3fuvnfaus.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3sdonkbgk.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3siondlsl.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3kjlcojrw.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3sezrjidk.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3dykqahmf.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3sczinbqw.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3qprydrse.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3mxjrejlk.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3fsgjnxcb.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3optadisg.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3zccebgth.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3tvkyebav.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3fcivcmlq.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3kdyxdirr.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3bkivldho.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3seknegct.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3aaqhikck.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3uzxykazu.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3cfvbnmig.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3qnbpyici.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3ewwzeaom.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3rwglykuc.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3temetcya.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3acvteapk.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3mricjupa.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3pcxwxlhk.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3fouzlizv.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3nmpbxnnu.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3jfftluui.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3fdwiybfu.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3gflctjwm.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3ficolghz.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3lafnhysg.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3pgduauhw.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3sdcehvrb.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3cvtbzvni.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3pdnbdfqc.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3honulnns.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3vcvsfkin.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3tvurlzpb.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3mawbrzad.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3uaihjuix.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3bghradjh.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3bzzrcrsp.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3rqyldxvg.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3epjsrhyv.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3sodpimln.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3mdruygjr.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3bgruifqy.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3rckcjgxw.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3bdgwuqru.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3njikynjy.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3cqfhcamb.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3dxmyblww.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3ynkvqmxq.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3ehmnpfgl.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3wgkfober.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3tpqsypip.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3iktvjjrz.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3stgxaxit.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3poohroiw.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3ovbcjqke.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3xnyscytz.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3xlitegeo.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3iwwsugms.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3nslquhyl.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3apqovoja.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3jbxamymv.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3lkboszfk.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3nrkjyrnf.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3jzbzsswm.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3asbgajcw.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3iqbrajlx.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3pzkhjsbv.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3egcknvet.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3fjqvdjpl.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3hixzxdfe.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3gfahzzqj.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3ptrvnlpi.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3ryralqah.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3uzjheqqf.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3lxyxebqq.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3szfotjpg.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3sjwhoadd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gkrskimv.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3tztnuglw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3biwwrtfb.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3zwglonmv.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3bzrqioyz.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3vvyhozvd.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3xwtxdjjo.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3ksmfnpyn.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3foiijxfx.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3wpawkeau.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3gwfmllya.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3halxnres.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3rarcuurf.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3wefpogfg.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3byvavize.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3hkoledlo.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3wepjnxwl.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3feroijwl.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3xipcpueb.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3rqqeemwp.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3hupwbvhd.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3skpvpkmz.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3qksuopyp.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3vhhogqdj.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3jdxufyah.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3onmjfrfy.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3luxffcyr.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3xecdpoiq.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3dhesyqsm.html


<!-- 参考信息 -->