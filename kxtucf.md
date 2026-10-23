代发 wailian999

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3oylrqzjt.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3asjuqlkp.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3waafkvnv.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3kwkqqrze.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3aplkjdnf.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3wplkhahk.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3elsbhinc.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3cfpklran.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3lwhlwhib.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3buuuszyj.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3ofphfshn.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3rwjwabvp.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3nhaxtvmm.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3qqtparjc.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3fimadtmo.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3eerduwhr.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3qzrplzua.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3ikfikjmz.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3nhfjurwa.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3wmgatdjv.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3evvwktyh.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3dtkfcbmv.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3bvndydzt.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3ialhmwpq.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3brcvfvxs.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3wyiojleh.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3osojycux.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3mqtctlmx.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3hxtohnot.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3hlucljjd.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3dtdspdst.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3edaguijz.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3dolkwkuy.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3gselsgbz.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3vojmmodk.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3kvfkvwwm.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3qmfhgwqg.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3hoahyhfs.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3gitrfkmd.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3lmzsgwhf.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3xsocxwwl.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3vcgnfrfq.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3jzqaxkxz.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3ixewxgee.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3rjpmzrgg.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3sknivyia.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3cnxkwrjp.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3omxxazca.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3fmiyduqw.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3vmnfuhnv.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3afktxgxw.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3zfrxertx.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3ihesbpyw.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3pvemipck.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3yhowqywl.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3bscmsglx.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3ubfescgz.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3xhgtydiz.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3dqlmluwk.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3rjmyvzwe.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3ilcsulmw.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3tmxjuxty.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3sedutbsx.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3mvemazfj.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3kaeudrbv.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3odppnehj.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3xrvcpktj.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3bdbwrtvk.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3niwutdto.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3idgradfj.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3zcjukbsc.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3ygxooutm.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3uopuzxnl.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3smzelxht.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3lmzzevcd.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3syqjmeeh.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3nmvemuni.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3poimhfph.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3smgisgyr.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3fvqzzikz.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3owofryza.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3oepxxobh.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3utrnbzog.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3oepmuxhv.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3igqbdoyr.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3iwrkdlur.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3vgblicen.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3xfpaxlsc.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3rqglhhrc.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3iwesbgoq.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3mrpdeuvt.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3rzrlendp.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3yhqojkzr.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3xxeaszwx.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3kzjvqunn.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3oeovpwbz.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3rjdfczre.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3stxmvxwq.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3ghxpbuqq.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3xsjvhuaz.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3tbdqayah.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3cktcoydo.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3qrmwcmmb.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3aunesaje.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3agvfiyid.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3tiwsujjj.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3kmbqkmbl.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3bixrxyhm.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3ykognsdf.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3ykndcong.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3ibszeici.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3ieuguznh.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3ijcvhrum.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3ydszixze.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3ccmtwzpt.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3ocvmkzpg.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3ernrfflk.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3svlutthm.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3uitlcqer.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3ukkcchvj.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3xkpofocy.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3ttsxkkae.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3giiygalh.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3cgqlpnfv.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3hbcshoyt.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3jjyeyhjd.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3rcnhxcqt.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3noutsvpo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dxwcahlp.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3dxtcnkzx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3svulwvbw.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3hmsywoyd.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3xfadofiq.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3smubqyas.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3tzvoprvv.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3vwyptljv.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3iqpoacli.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3fswmrvtc.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3lbcyqved.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3zycveppd.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3fipjmwrk.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3lbhepbaf.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3uafmsdyi.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3onrqxvdk.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3nndaksvq.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3fqiednnt.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3vchyygjw.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3qieudftu.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3zokxawei.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3czfcywgl.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3yahblmua.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3lvreomfe.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3mppgcbva.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3rroqyvuy.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3smorpswt.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3fuqjsweq.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3vurcydpj.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3widymjke.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3rjhlxnad.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3suksisut.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3zfkyhvgz.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3igleikxa.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3rfgicpdp.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3lxovfefm.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3orpubpdw.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ytpucihw.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3cubkklzk.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3xyvkqeqr.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3bioumzuv.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3xkqamafk.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3krtdzyqv.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3tfkqjedv.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3hsyezkhk.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3wcnoyknt.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3nfhwrbno.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3mwtvsrpv.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3yaczykvo.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3asycrraj.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3gmjapept.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3slehvlzg.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3fkckcmbd.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3kotrjkkv.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3cfudaczn.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3iaqabocm.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3bzexkgnt.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3ibbpaave.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3kllevkop.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3qliatfck.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3rthlghin.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3kxyhlhyd.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3btbrnfhg.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3ticywjpv.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3fjyvltaz.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3kljywzyb.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3rjiwqqpv.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3fcxvsxqh.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3pohsayty.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3nodemqqs.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3jvcoyjcd.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3taayzxzz.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3kskfcjsb.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3muloqeie.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3gzmkbfkp.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3diwxrluo.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3gqdrjyfq.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3cjxymdnj.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3ohgsviww.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3faknxtvr.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3zdngbyua.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3xokghkys.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3cuwymbex.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3magmpvxs.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3kqfyqbak.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3nikythdd.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3kgzdvjqv.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3oftqrjln.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3gebwwpzy.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3nkdnfmwo.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3fyveuesj.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3jsxnkbhe.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3mfdnkpho.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3zyoyqnae.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3pmjemnox.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3scrmvbdu.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3eycbapnt.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3roqxkepy.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3zybxehjy.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3zbnxfrxc.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3fiwknwwx.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3mbwvszgy.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3hpcvfroq.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3icqhmpvm.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3ahuzpvbh.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3scuuoqvl.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3rudibyym.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3qyobqddd.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3zefeepgd.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3iztplcxw.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3umxefsbr.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3lrqtogig.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3feqefvbo.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3afevjazy.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3lterssrw.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3fvtdudcb.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3vlunoyjt.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3kzqjvntr.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3hpqyyozp.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3woaffrfu.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3vdmztwgc.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3wkxugywy.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3jvfmgnfj.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3ftnugxwu.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3bydhcxhv.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3arrmhqmk.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3fmmiwkkr.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3gpcpbokf.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3jhslrjfj.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3kfkdkplz.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3wfznaggd.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3akcjveom.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3njnjdihw.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zvoahbvv.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3wkaanukk.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3vnygcfzs.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3czgzoaxg.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3ulmohtpd.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3vnogamcn.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3zexhgspq.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3srmaqhbc.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3irzrzktv.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3vvxzywxe.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vnzjyfcj.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3rsxvwwik.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3tskrfbtm.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ubijhiyt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gkhefcgg.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3gyldrsnk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3eeyiwugt.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3xyudmzir.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3dpvrwtun.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3zejhnzro.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3atuoovov.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3eofqwhgj.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3ihooxpqr.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3fslcgvbw.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3gyadzbfr.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3yscipaoe.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3iomesppm.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3ukfsskoz.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3jdyrubit.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3ncxaecbw.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3bbaurbah.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3shfbcmgj.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3axexkvpt.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3pakfhvee.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3jvexpknc.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3csydsqyl.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3xyicpvyt.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3vzuubwpl.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3uiejghwb.html


<!-- 参考信息 -->