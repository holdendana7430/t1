代发 wailian999

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3kgmhdiud.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3wbsfpbyb.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3yzqrtbfi.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3gxfchwbc.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3fcuzwenr.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3pgnxbsql.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3krfbayse.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3cuaihdxh.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3ajysbmvw.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3hrfbjdxj.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3izasorno.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3gdkthnbj.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3kfarkirq.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3ypkrjtwt.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3wknrktaf.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3nvqacsmf.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3ulcoqpkp.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3pxscarqd.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3vzrczmdp.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3ovtvmfig.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3rrrmgooo.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3zpfwcrpt.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3deepqdhw.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3xicpsrgt.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3xprmkgxr.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3aduivhdm.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3wzvbivgk.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3birgvbdg.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3xbpyiohc.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3vceajuip.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3imptlein.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3kzwqxcra.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3hgfyotpn.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3kltefazz.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3qvgowris.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3swzbnjho.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3yupmdgpg.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3jzikuftt.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3eynzgpdp.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3zurjekyv.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3prlhstbt.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3fbwsadsg.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3yxrmcbjq.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3ofljrsgc.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3pkqulhps.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3rzhygdjv.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3vdonliar.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3ovqjxpeq.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3rmwjbqfq.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3tkmrcdaz.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3fsbkzjfn.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3ulenkmkq.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3zehskgpk.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3ketfkcnf.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3bhdmxtaq.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3pnlwxvkb.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3xlznigwx.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3tpxcorxk.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3jqxtwgqn.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3tihgkvwu.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3xevknqtp.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3horxwwgx.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3kuhvhegh.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3qsjnpvcx.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3jglligfz.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3woujlejd.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3rspvickd.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3fenbvskf.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3ftejzyds.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3tjygatgp.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3eeyngogp.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3tdmgkzqn.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3zpftwsvz.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3xxjaytci.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3ctqphhzf.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3qghxaord.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3fruwhypz.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3ppndddsp.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3yvryqrbq.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3kbmpsqud.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3azttctqt.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3dkjuptkx.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3jsfumyto.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3askgufjz.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3mmnugwtt.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3unqkxftj.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3dhlkbxjq.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3pocvyzkp.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3ulklyldx.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3ghnnlfoc.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3zeibdijx.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3eimufvxq.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3iwsqzsqw.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3pwhdcnpd.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3rqsbjijt.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3fzvqokmj.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3sygtllhy.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3zvnidldi.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3bwuxtapo.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3gtuqkjio.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3pvwravkx.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3vgqxviak.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3pojjfuzw.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3fqigervs.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3zevfulzq.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3mimynqqz.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3bgobaxpu.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3cftbzvro.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3tbggtwlg.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3uurgffdf.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3qxagmzgh.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3ozxppnkq.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3pvhsnwco.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3vhvkvjvi.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3krxqsvku.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3quukserv.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3esvznwnj.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3bikcnkcb.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3lgshnfum.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3eqskcrie.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3mrhekqec.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3mkixljqa.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3nmnfwhcw.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3fuahrpvh.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3ckpluegy.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3juwpqoii.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3umliwjxs.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3yuiyousf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yvjzyroy.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3oxqzcmxr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3alaqxprs.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3rspmkxkx.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3dhkqbfej.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3rmfzhjya.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3wbayjeuk.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3osrhuina.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3icicdpdb.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3jzxgggqf.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3fgbtjnae.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3dqjlnbrl.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3oawwlrfl.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3tngeboqt.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3xriiamvc.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3gsnqbpeg.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3vhsyxnzg.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3jduvgipb.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3zgqduuqt.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3gqeewvuc.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3prcusdlx.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3rwkpcvot.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3jnmkrvcd.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3mzcxiuyn.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3hgrrytqn.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3hitjqups.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3jbbivmul.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3frkqwetl.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3xftuoxek.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3rrxqxrlk.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3kcasnpkw.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3bbapfibr.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3aikixhek.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3umcnpzwl.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3ympmksjo.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3hhtfthjv.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3mvrxdhpl.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3qajsqomd.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3eyyocton.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3saojhpbo.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3vjajaahp.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3hmegquwd.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3teeqozqi.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3mecdtpqv.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3ltmnnlin.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3wtitpbih.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3emmovlps.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3lrwhdhwk.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3artwyevw.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3nzjxzinr.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3dytubowv.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3wnfczpjm.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3lesbhtts.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3dbzerrvn.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3pjnkoeoo.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3vrpnnqmq.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3jqlerpil.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3kvxnoscg.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3yimtgkib.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3sbmmbcnm.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3xzqenwbz.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3fhrrhodd.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3xafybnkp.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3gubmanwz.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3lcyvzdcx.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3tbmbccxl.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3lcwbcdhl.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3mqfmixqq.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3tqhjoatz.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3eumhxwzo.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3sgvjegbs.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3oyhdwcup.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3hgoafasz.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3krdrczqy.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3ubyfqyzi.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3gexnwagt.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3mzjnrtrx.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3dchtqank.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3zfpogpaj.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3srhdroaj.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3feemdofq.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3nrktrhmt.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3nfifyyrh.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3rcdhxwnr.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3qtjppzgx.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3kikvfzsw.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3rftotbqq.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3ungctfuf.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3ygahhmyq.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3ndfreidh.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3kqjfoich.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3bygwsazk.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3fohmjgvj.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3lqfpiteq.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3bwmadrzl.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3rzlzvdul.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3yztillwk.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3silzllhs.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3kclikepu.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3oqgaulvo.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3gponmwbb.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3jnbuwsov.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3hmkhisif.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3jecfomyi.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3khgzwumm.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3nkdraqzc.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3hxwgoitj.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3rqugoidb.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3dhegfpzj.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3eawobhce.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3ppofpgka.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3bfygxsyn.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3cpnuikil.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3fcwjtvfu.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3rsmtroew.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3aefewvqg.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3jjnjyrsa.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3ibnfnlpo.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3lhddaehp.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3vecsdovy.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3poowgrga.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3nanfhmde.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3myjvhxif.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3pavenwaq.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3qsbpttns.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3rmkyjyma.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3ejjimwjy.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3nfxbhquc.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3rexgsthl.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3zyszmvqo.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3yczebteo.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3pvdczwga.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3palggdff.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vsjnbkvn.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3zbhpntva.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3zgcnzhki.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3sjfwjfwa.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3wbpkgxum.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3didwoesa.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3ayydubwy.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3gkqxqgaw.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3ovrpqajo.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3fjvspkjo.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3djqyuxtf.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3jhfywted.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3vaqnohff.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ailufhul.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xkvykgxu.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3fuibcsks.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wryfrrrj.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3mddajhum.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3cqpcclgd.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3kbqxpnwb.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3ilmtvghp.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3xignftet.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3zrtatxfw.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3yxnqalgy.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3pzzpgmnm.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3cdyzygaa.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3mpmdyyll.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3jbqrubbi.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3xsnutnmx.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3zuuezuvc.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3ecaalllw.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3zhyfzxcc.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3sqlahpzl.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3qojzzzhm.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3dhuohkpd.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3cissdemw.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ouyxtssh.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3eioutmzt.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3bdnnhznz.html


<!-- 参考信息 -->