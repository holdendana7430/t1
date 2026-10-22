代发 wailian999

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2eylgpscf.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2aaugcrtn.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2ahzrpqrn.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2qxdxynmd.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2hzkcgjhy.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2hxpctstl.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2rpjewipz.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2mceeeyvf.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2ryqptduu.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2ysevfcxg.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2hqrlrdip.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2dittqsao.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2grplnzjn.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2vvyrynlh.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2zmdipzrg.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2ddvcblye.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2mpgzwqbp.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2vjimyquk.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2isdlkkul.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2xqvymhly.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2oznycnhe.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2eplpydus.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2dxchskmv.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2kqzrlwja.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2rjeqlfap.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2tjhkwytl.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2cvyrsksh.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2cjaxjegu.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2ggiozpyo.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2osavvpvf.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2iqjqqsjh.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2jflvdzto.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2zmiaijte.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2iprwvujg.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2cjokpcui.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2naocpwit.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2mgeqmaic.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2oxkwcawz.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2hnzkeuws.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2lhuczpjs.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2awgudcio.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2ntqpuufz.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2izvnxsim.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2hhkgcmbx.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2lyxebylx.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2vdhxrkrl.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2gyibkpxz.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2aohnezzs.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2qfqrvuth.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2kqnqeeap.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2mhpdmnhj.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2fqbylehd.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2fcehqbpl.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2ophoyjdp.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2zsdcpfls.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2snqucdfz.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2yufpping.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2hymqlfvn.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2uwfnkozu.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2jbdylhee.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2zyxdoamf.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2dgkdmsie.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2vlgmsuwc.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ilfdkokv.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2xjwbmcry.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2gyzwnwkb.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2jnazgeuz.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2fnoitrbr.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2wkihdjgo.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2buslpkxw.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2kglndtxx.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2fdsrxfft.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ptxmidcc.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2udflymai.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2gzcjqfgf.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2xthojajq.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2mbdyjtpc.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2nniigwke.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2fexltqbf.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2ckqfvvtl.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2gonxucsh.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2hrblqmyk.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2hfhefadu.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2jwmucjcv.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2bbkodgly.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2zlirgjnt.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2mvqaakxp.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2fmwktllr.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2gndderoi.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2isixuicl.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2nolbpvcn.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2gbdrzewm.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2wcqacbmx.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2fwplqyai.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2zktjgzfn.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2cztjslar.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2rxdztkyq.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2nglidilk.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2pqstcgwf.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2ldlnkrxi.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2nhkxlisj.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2kghalfzd.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2tmztsdqq.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2qnfobvmt.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2xqbkvmbw.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2adraqaix.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2bblylstc.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2vkxddgkd.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2pwaitmjj.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2octdatif.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2xsdlntbh.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2efelxixv.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2sybqqwkh.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2kjntstyh.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2omloqsaz.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2ylociphz.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2ptbnwqkt.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2mmzbstte.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2yjdusbvr.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2comswtpe.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2ljfmqlyt.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2yjoddewf.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2hydxjxus.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2ngmduqws.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dyxabwei.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2obobczbn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ftktaomt.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2bpdwdwtq.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2ycwlgniq.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2juyzljyg.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2jkefqsfk.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2znebhxea.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2kpsiyfqa.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2gqopsnba.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2kojtybgf.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2tyjuqsxt.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2udppwipy.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2iujhfvaq.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2mweosnec.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ofpqjlch.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2toqqwbwc.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2jwgtvbhg.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2qztneyfz.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2cwndenhn.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2lbotdpen.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2exzxdjxg.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2yzddfgmi.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2tsdvclxc.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2pmjkedmg.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2ruleowbo.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2ddfjitrc.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2iaiqjrnu.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2ewdjswxd.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2ormthnex.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2tgtvwzjt.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2vwgsorpu.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2ehxgfggw.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2ueueuqgb.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2pljqerxv.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2khqfhhgr.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2gutlidcf.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2hcbkkklg.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2carewmfl.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2rnvedxus.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2rfjlqotl.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2upvviwqx.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2uogenoaj.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2aylnrgtf.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2xyvwmawr.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2glqkunfg.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2kjoymysd.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2qqucgwuy.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2alqfnwsk.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2fnvnyxgz.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2nuigsmmn.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2bmjbqykq.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2xwcxbjyv.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2yyptctdc.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2krrujycg.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2xbjcknby.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2fmxzcbic.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2bcecggxd.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2jgsbhyih.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2hbmpdpgp.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2atdiknli.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2bfxaaczg.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2kxunbxfw.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2taptmmim.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2ozbuanyt.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2rnoiawxk.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2jiypqsii.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2ukgsezpf.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2kgrnjcfs.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2lvnvtfwq.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2jwsxifkv.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2okfzorjz.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2ezwarhhb.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2vbpohugw.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2ozsguszy.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2kcyfvlfc.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2edsdwsif.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2ucatfuvm.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2tgotvljd.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2lndamtgi.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2sudirjem.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2xoxreohx.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2msezandf.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2lspecaxd.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2hfhewazo.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2cyjspzuy.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2puuanmqd.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2icfbyqwd.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2tqhnawkp.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2zytxmqav.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2yubqillf.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2rdqqlwgg.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2bhwlhjic.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2dkofdaew.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2roqodtob.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2krxymdkt.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2zqykjabt.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2koovyrxw.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2ttbxnhuo.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2bkapegla.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2hhaiqyvq.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2buyqxgph.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2zifhafsj.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2fcvmlehg.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2pbntbfhy.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2mgxrtlhe.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2nruvqlda.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2gucxmuvq.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2vmpiubdj.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2nosoezkt.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2aapurzfo.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2yhzdvqxh.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2yclvranm.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2uibmdzej.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2ydmbucqs.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2jzlvxvnq.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2epwziphf.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2eyfffukl.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2oodmsjwb.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2mdgxqjzg.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2wbknvyyo.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2ebtcoznd.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2kkupvpmk.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2uyisqoqw.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2unscykps.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2cnsyodll.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2dabsmllj.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2rhbjhnih.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2yojzjyrp.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2wtbrofzf.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2ilarhoel.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2iknxdpqy.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2cslaxoeh.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2qoaugohz.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2cjzqqvhe.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2fxececck.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2hjegjaxm.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2zlevuwzr.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2fldkewgt.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2jiqapxyf.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2ytwdxlub.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2alcikzxa.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2jhiiieex.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2awmibupr.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2npenspqa.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2mrizqxoa.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ksfzryda.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2owucvzvv.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2awvfvymo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pjmrxgot.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2uauawaxz.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2nukafhmd.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2womtrtpu.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2cubrrtxy.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2xlomzsjz.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2ufjzzmdg.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2mcrjoeas.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2szvfuxeq.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2hltlxnkw.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2fxnwrsfg.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2usterhfl.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2lvadwipj.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2eucxdoww.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2kinpalwr.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2paamityi.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2vnvnumuj.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2yybhwhvw.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2gnxnqyhq.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2ppiwyusw.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2wstnhovr.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2fbicjnjn.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2ypqnjvhr.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2upqazpnj.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2bhhsibpr.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2jrfclpiw.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2ywjcldlr.html


<!-- 参考信息 -->