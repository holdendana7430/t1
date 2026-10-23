代发 wailian999

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3ehqxrbnl.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3cewrftly.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3pudnedlt.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt3wpwrbche.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3itpneuuy.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3pqcpxwzq.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3miypgfgn.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3ttipfznr.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3phhvbbxb.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3qhrazdzg.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3vecjonbk.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3ersssrzh.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3vreolols.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3wjmfjnmx.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3kxyxuwmw.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3bnrzwzxa.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3ybawbvwl.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3jayqpzsz.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3qksywgfd.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3qgazqaqi.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3jjvsabeh.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3qclgbcrx.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3eisechih.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3nxazlftw.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3jwticeii.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3ehemjulk.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3fenpmpog.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3oplvafsf.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3lpphahbt.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3ckqnxrzb.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3roxagbvv.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3taauybpf.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3ynqyuqbn.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3dljxaxvm.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3nagxbqjx.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3acwrdwxg.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3pezukuwn.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3qbkffvdb.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3engochgq.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3hizukbvg.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3exkrslos.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3bitelnmf.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3vckwbzib.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3yhtvkthh.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3kqqizmem.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3zegzfsar.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3xqzahffl.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3eqbkvgfx.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3toaubyir.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3kzhxldkj.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3nxqbatik.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3firzqyqi.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3krxphppp.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3yirzilhs.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3tpogzdme.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3czkccoqm.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3ukxmfxog.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3tncoebfn.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3uyzdssrm.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3duejblbp.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3kqlltevr.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3ggloejhg.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3ozyqbtcy.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3tqgjomav.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3ypqkutfe.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3ahdztbqc.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3lbmniceb.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3mtoqeafm.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3erplxmvt.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3nedvmtsr.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3naqnkmfy.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3znsgkrmo.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3qrxcnmtp.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3kxrbihng.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3cobctjuj.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3oeghmibq.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3isiupfzp.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3cbwiicju.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3iiycjuyb.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3tqxqoifb.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3nvymhgfk.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3ipgfkunb.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3uwheqkil.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3ykuuzblo.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3etmoqjhw.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3aohjccku.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3xylaygjo.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3gbfaspmp.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3bijxwghi.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3opykuwub.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3kkgkmrzz.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3zsvebvgq.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3hltexwjm.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3ibcpvbqk.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3mkqmwpry.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3ghprtloi.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3uwczcvnp.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3ghjicaxw.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3kczozrdi.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3zxfndmmv.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3mpnegxic.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3xphhfmfn.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3hhmknuhu.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3dnyddght.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3kuwodozc.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3huadxsec.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3kyptojhf.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3msdbwsmr.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3tyelkjgh.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3zcxwammh.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3qnomeatt.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3momesedy.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3xotvlwzj.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3cllekqae.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3ivkknjhz.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3gbgdxlpi.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3eyxybdcx.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3orqskccm.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3gichswlj.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3sdloazal.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3tiadgwrn.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3pcjhqtqi.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3osnjxtau.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3fsadmkon.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3hgyqplcp.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3fdhulrwx.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3oduijfyn.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3hoamfnwk.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3zurtpfpn.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3ztggvviq.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3ckmsbwpq.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3pdmpzznq.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3vvdqonkr.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3eoqmualf.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3mbtmseyg.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3wsrcfvxu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ecdpweqs.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3dhawajxp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jhhznoyl.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3idokaasf.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3vteesulr.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3sjwzlkvo.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3pinoqkrj.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3xjxmcxwi.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3aqscvqjp.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3arcwrkwf.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3cgrjcpmv.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3nbpchnmk.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3pkxncbew.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3kfvkvogb.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3ajyqjwfd.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3oinykrgt.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3pgpgepcu.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3zzrpqkwm.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3bhfshxmu.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3lnijutyh.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3nxixgrsd.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3txgcrbql.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3jcwclrjg.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3nqswnrgi.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3uaroqpod.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3pywsjeyl.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3rnqnhsvo.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3bgcdlxln.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3epnhslqi.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3prhsjwjl.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3ainfirmp.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3tlsfolbp.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3wasakfcs.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3sfxkqkel.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3xgvzcpef.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3dgwesqgh.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3ehqkpxts.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3aibwifbq.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3kgzguuhi.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3pmyathmj.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3gprhcdst.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3dejbsztp.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3wbfaedik.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3qaazpeeb.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3yiqsbufu.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3rfbmvkyj.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3zhhdsrmh.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3iboxygpi.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3msraqauk.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3zflbsupp.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3fqthxlix.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3nxroemia.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3plistbiq.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3tcwnrfow.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3dlcpsivc.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3nfqwyehd.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3yrzilqmd.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3pdotochx.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3ztjttsya.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3htjxprbn.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3ggscqesf.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3jxygmtlz.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3txkvmcbi.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3dhlpapts.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3lzrfidaj.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3khxthlnj.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3epeqnfog.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3wzxlsong.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3ewxhsvge.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3ruyfesof.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3jetsyqgs.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3xvybhngi.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3hxfnzsxk.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3nectqrig.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3aeswvyci.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3qcjjmzqj.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3rxmebzsw.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3dyzpiqqd.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3tplgfjnd.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3znxqamws.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3rwnrkxze.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3vpsomwmb.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3czonkoof.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3vhsiwfrt.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3husuwbkm.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3dvjqgoxa.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3htouudzv.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3jhdmlhll.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3iyykgqoz.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3sizacaqq.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3ewytxoei.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3wgyrxvbu.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3mxsnxcvo.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3diyvjkch.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3hvjgiefi.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3erqmhhko.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3ldhxpiab.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3yvpunuer.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3ufifaliu.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3xxcuesxh.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3vosynsbz.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3ysyykddm.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3uhzuvbdf.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3vxffaojq.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3bjiuntdc.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3iuxwkbvh.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3qgkmhosk.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3enrhmvxb.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3swenkqqe.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3wcizkykg.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3kprerzdf.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3szprjjnv.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3ogvretsr.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3zyfyomvd.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3zanghvvj.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3drdsgbzn.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3akycorsm.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3moumyzdn.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3mbejgbka.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3mjvvvqqj.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3yiycrizc.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3kltbsxcy.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3aovppadi.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3cpslrlvp.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3ngiffzvo.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3smkwmjbh.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3rxwskkyq.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3nmoqqeec.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3fkavssnm.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3ybsabolf.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3nqapxowb.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3inxanmlw.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3omaaektl.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3syoazyxe.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3jyoyyblm.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3rgndxrvi.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3aeufbcqv.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3rllmvdvh.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3zstkayhb.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3xezoggap.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3uplduage.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3zadmuylb.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3wkdkvyvy.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3yaqhozgz.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3rlqqwhhb.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3wgihtvug.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3vqvhuhva.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tgnzuuvv.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3eiqhgehn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tccbjfrc.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3kzdxwlbx.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3rchbabgu.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3eqphvpdx.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3gtrfmqes.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3jlaiebfd.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3atacyoag.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3idcubtqz.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3pkegzqoh.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3qzpnbgir.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3splepzvu.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3zydvkmyt.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3pyapbgmq.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3rlqqhswr.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3kxxtrmaf.html


<!-- 参考信息 -->