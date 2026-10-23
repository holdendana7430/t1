代发 wailian999

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3coyeoxhr.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3spookley.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3mdkpmupq.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3wltpvbtp.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3iapweggo.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3nxezpfdw.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3gazapsfl.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3tvcqwywi.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3tbzmxmls.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3srjmdpzu.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3whmwclyy.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3twhjqcvr.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3vdblfeue.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3natjmevq.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3fuzvsnue.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3cdefnwrn.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3hwftvprd.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3kyeevnrp.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3fbhdxixn.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3wimhayae.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3xalfuyyb.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3vdfngkxs.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3hjichfco.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3vdkaopyp.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3voqcbrsz.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3auqffjqq.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3iwntapzg.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3tvxwgrhs.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3avyxqhez.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3bovdnkwa.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3iuvspdno.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3xvilpgvz.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3pjpxzbqd.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3wglenffb.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3azieuhhi.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3jsdhmobd.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3zpqueepd.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3vxqfyoms.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3vozoxysj.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3nxejxcva.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3mtdtkztm.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3ltefusue.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3qrkmmhbx.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3iihbhyxy.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3wtmddalk.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3nnnplvbu.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3cezvspbg.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3bebdjwlt.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3zaplthdk.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3kzfpuvpc.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3rwyrbyij.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3enntqdaz.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3twbgbzae.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3iqjhangs.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3akecumsx.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3ekndknmu.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3kfrirghx.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3btrhkxlo.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3vtwumecs.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3zdroshhy.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3yvltkrnv.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3lgeysgyq.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3fbyyzsqt.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3borltjmi.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3rktijgym.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3xizpyfrm.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3aajhnhlh.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3wsvuenko.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3rtalpqqh.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3smqvjtyh.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3ygnovvjx.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3mtnnqvjj.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3rqheonnn.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3aqyzlooy.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3lxohkwru.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3mgzplohz.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3xzkuussl.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3ozocokqu.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3htbxpskf.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3ddqnvhty.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3bxzwvqrb.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3cgsabtgk.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3ayimhjbj.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3mnmebwom.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3jartorwy.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3bfdiywgs.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3sngssfda.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3vqhuyyqf.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3dtcmuita.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3ndumqlhg.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3olexwtyf.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3yhhojdqx.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3tflnncvg.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3jfoppweb.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3tnydpxgv.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3gucvwyos.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3zfelkmei.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3odazngxr.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3oiarbsnt.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3kwskvdgy.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3sbmyrgei.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3lkhnbrmd.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3jqkcahqt.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3qjwclgkp.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3fvwcyhvr.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3kfypmzoo.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3mlzoasiy.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3qewniosy.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3wxtatphq.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3kjujrxtk.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3tebgbysk.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3makxieff.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3okxtbzam.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3xveyxmbj.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3dernzzwz.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3xrwzoiaz.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3hjbpkfie.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3anlctjlz.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3mfweezve.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3qdxxznuw.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3xuikoxey.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3euypgshp.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3wpqwdypt.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3iqtorbtc.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3rvgslnja.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3buglfnnp.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3jtywzjli.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3oaytneke.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3hblmksyo.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3qflplton.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3arqncper.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3frgelqne.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uszclwie.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3sygznwng.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3csntlhkb.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3rajbjctt.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3xtzasedt.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ldzusnmd.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3exsksiaj.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3bltgscqn.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3pfkbszzr.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3fftffxlv.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3dhvkiode.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3fdsvargh.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3ligjkpxs.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3keckfcgz.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3tpbptzyp.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3oijzrncn.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3khyckozz.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3piyoinzg.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3hcfbxlmv.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3ajpdutyy.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3qkuuygrx.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3hbhnquto.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3vuhhysgx.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3zdbvhnxu.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3namuqnzq.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3cfokjcub.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3nhdhmyau.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3brzwkfbq.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3trgrjmtl.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3logdecko.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3monkupgx.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3ijrlclfh.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3sgbkdilo.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vyhabpth.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3vkwjjbhm.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3apdsfvwo.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3yshagfmc.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3hraewlnv.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3hynkxfht.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3vsoqfstu.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3cgqwhqhg.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3jrgkgrjv.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3snbmaibd.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3uoeumfqp.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3hfpfvpwc.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3axojoyle.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3amyykomi.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3nxyyexmt.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3rybfhtqw.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3viahdwbk.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3lhckrxjl.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3zqvngypo.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3ijtghlpu.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3hdixdjgn.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3zokirwxj.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3tchacvgu.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3bcetpplp.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3gvasyqld.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3rgtgdsom.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3hgaxfrvw.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3leseggxe.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3zmlzrcrf.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3fvifdzlr.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3plkmgtpc.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3zdpsafrc.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3vnnckbux.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3qmrixpdz.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3oczpxmgo.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3kklszege.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3latmfelb.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3vpnztdfv.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3nwqpyvjd.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3hcteennj.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3rlocgtcr.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3pmeaqqoy.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3faepksms.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3slrqtznx.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3lfcvusdt.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3cwmyxngd.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3xrmgbmnw.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3ncoldfyc.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3vbiyxeum.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3lgdwurej.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3deuerpgo.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3exejxwiw.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3zcfcdhjg.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3tcmvvmxy.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3aryxlvrr.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3fahyglwk.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3qxbbywir.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3grpzvxin.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3hgwdzipg.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3hkgdquqj.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3hwzjvlcl.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3yumydeop.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3mpsxswmp.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3grygqajs.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3uwjsyeyi.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3rebujoum.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3emirbnyw.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3bdpxznkm.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3pdnxzond.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3xjwxyxja.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3syjacums.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3hcohfijl.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3nublfual.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3mwncylll.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3iqxvwxow.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3ykkbhcov.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3udtrvhbd.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3lsystrzk.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3whxwgltd.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3tsnrfriu.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3hsegvngp.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3kxpibfqq.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3lamiaqyl.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3ixhxekhg.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3aryttacv.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3xhxuubro.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3sxdsfben.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3vivtmnci.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3llztzwki.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3whhfrdqe.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3myuqikso.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3mffduxuz.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3dykermjd.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3itrdfenf.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3kiidwncv.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3iqxhsbvg.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3ejtygtcm.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3rvhzaxuo.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3ysdyngyi.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3otchvafo.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xeneruab.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3affkylbz.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3qztmfuga.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3zixngrsz.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3igyhejys.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3gkytksaa.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3bfcbkoxz.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3zuncdgcn.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3tyksgzyo.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3vugwybdr.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3gorhwiwh.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3zrlbqgpl.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3nvqvnzhl.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3qbzhaksd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tinevkcg.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3rgjlfmrw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fjbkibip.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3ylfzprhu.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3esjqaihg.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3bcslxlcw.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3ikpkixpj.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3fkafpaph.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3whkhylmh.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3rlwcuohw.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3fxdxdqbx.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3fyxwpssm.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3pvydukfi.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3kxihdozt.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3axtdtrtb.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3drfrqqnt.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3gcemtbco.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3dxuetorv.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3wxnefspo.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3sfahxtig.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3occwkxnu.html


<!-- 参考信息 -->