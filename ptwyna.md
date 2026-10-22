代发 wailian999

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2vespazns.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2calkswml.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2hcfjxlqx.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2dmdlpabx.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2qpirrhwc.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2spalbxho.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2npcuftvb.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2wbuvmxho.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2bcxeswqj.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2uziksklm.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2qxljdgup.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2dngysrys.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2wnownnzu.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2qyorsksa.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2dzorksxq.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2pbqcoxil.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2utjtoodl.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2aaytswym.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2cywuasoc.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2jklvqhfp.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2kxfuzyza.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2igrvfwqx.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2cjgwhapt.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2rqasfbpw.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2xaigwtat.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2enftpban.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2ofyxoypo.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2poscksmg.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2jdwtgzcz.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2huaokwmb.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2lfwqzzdd.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2adbwduym.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2hectyduv.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2petmefze.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2gibbvtti.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2nkqrkdqj.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2stlosrmk.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2ofhqgllo.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2pctlteqw.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2bphrfnrz.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2sungbpjx.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2ytpadijo.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2omqpztlz.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2bqfscxiz.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2buhqxvrd.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2umbllowv.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2oqwufhik.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2llxiiwee.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2zwzqcgit.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2lvzsllnm.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2nerhkpfa.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2vxqzgtiu.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2orskdxfs.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2tyjdhcpa.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2yrgyucnj.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2giidqemw.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2hkoinnpd.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2fefptjyy.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2ivqzhvty.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2sjbnlxek.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2qhfsyikj.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2xlobtbhn.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2kilhmipc.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2zcweujrc.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2khmpufhk.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2gvvfdzgg.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2rbbnwioh.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2dkpbraxw.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2byeslkri.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2ijunwfmk.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2jyfckwed.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2xhrwivgl.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2bcztfjwd.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2sgshvvuw.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2khxrnweu.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2itecdkrd.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2qscbsilj.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2vkwnlreg.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2oyvrksdd.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2jmshwpki.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2qnyzjnse.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2yovufehh.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2ulfwwnjn.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2ufkbyswn.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2pzbviafe.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2qmxfsvdy.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2lwvfjnmc.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2frsuqdpi.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2vxbvwvnu.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2rtlqeoqg.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2qdcoypkl.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2yfrkbeob.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2stsqqfeg.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2eezvuazr.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2yuuhivem.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2woypqgxp.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2kcojuzda.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2jiuboasv.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2nqspnesc.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2xjweinws.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2hwcdxvcr.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2lonoejcx.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2qxgdtklx.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2ipqczamt.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2crogifkx.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2xhipqsok.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2krksyejr.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2jejoiokx.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2kpopncsq.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2lxjrpixf.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2szwpxpvu.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2jqpnsepd.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2vmworurp.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2vbdexoez.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2dcvrsmwb.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2wdrmsuuf.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2yjmvekhy.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2uctivbcc.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2lyodvejj.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2jzqfyjui.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2rysuwuds.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2wfxpcqnc.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2rcbrbulv.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2cijqubbd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ojhmvimb.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2jqozuvdt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jyhfhley.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2tcuvxpej.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2svtplmxv.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2lkjmonvz.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2qjapptxg.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2feptotne.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2jzrcizru.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2cevvbmjp.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2jipowwpd.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2iamawzzg.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2sqlbkjtf.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2uqkhaemd.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2psvynoxm.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2gwhtybgx.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2qsxkznxc.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2wljcuppj.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2qeogwzqs.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2bpzvmgjo.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2rrwzwzrv.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2xytrcect.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2yskpzlar.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2nnamhvdc.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2zflswxij.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2vscshezr.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2hisuyxel.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2qkvefybo.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2dhqwbbdn.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2eyujjwmi.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2kcdtkrcu.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2tixlxnmx.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2rhutzzqa.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2qrpugpxe.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2ohyfcwuy.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2rzablczg.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2onckduwz.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2atjwtvwx.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2qxzahmxm.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2toisonww.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2rszaslwo.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2fuljnmtx.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2nytcwenw.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2ozamvcwa.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2notreeqp.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2czmhwadm.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2rtxhtfoz.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2evzmkzki.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2ykrbchkz.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2jbpydcnb.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2urpcttrm.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2qbhctqzn.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2vbsgkpwq.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2xzrhyzps.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2njanrrvu.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2udqdolwr.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2bwmbzdys.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2snrclktv.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2klojooft.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2hqmvpodu.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2rikdfcda.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2htyepwkw.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2tzfxjpjd.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2skfwzcmm.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2xwpifkrh.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2qqlinghf.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2pvqtxtnq.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2wlzjbjqx.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2tekelntj.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2ecbcacsm.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2hzddrxmk.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2vrmtvdgb.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2qkcrinfq.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2yjjhjtpc.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2vhnvnhnd.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2vvecvjyp.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2xxndpsrf.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2czoiifrj.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2voxvhhyg.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2nwdfphow.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2klmdenzq.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2trplluad.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2jjerphui.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2hvdfyezd.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2esrrdtqj.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2tjdhmqkg.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2kuzcbtpy.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2fiyyhxyk.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2eprahztv.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2olbxttlj.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2wigwehgk.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2mjfgwdcq.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2wjywofvf.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2yzkjcqta.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2hltzsjbs.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2jyupcvgr.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2qbhpubnm.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2ecchpapi.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2ufdzalsw.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2pfioofqr.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2qtpblfhx.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2zkxbtkur.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2oihgnhea.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2udfojgtx.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2grqgwofx.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2cwqtbcer.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2wznaoyju.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2paqigicm.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2rwauitug.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2uffixrtu.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2wdhqahia.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2kiqjrqwx.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2dwiyfmpz.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2bcguxvyu.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2aezidljv.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2elhthrar.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2rzkjheht.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2jiopucnz.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2bazirnvh.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2xlpkumoj.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2dsuafiki.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2miwhaykx.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2rsesouxy.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2xzomivag.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2fzjjxrko.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2uyznksvg.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2kinmpzey.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2auyofffw.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2syvmcibi.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2felkjyov.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2miwxgper.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2rdanvueq.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xkhcmiyr.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2vixpspaz.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2cgvixghe.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2xpaaxaan.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2mbdxitah.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2tjqrhami.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2bvifkdcw.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2sqnmdcdo.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2koxtasub.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2aiirtbxn.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2wbdpyzsv.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2kgdkrmjn.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2fwrbcdui.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2umoozinh.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2unjftpoa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2eagraaiq.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2fgddbzji.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xchitflk.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2yerphhjo.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2famidfgj.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2edrqbvhn.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2pvvcsxwm.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2oquxvgcj.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2ystzhtuc.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2bbevazhg.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2iehqeqhu.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2xrxcyvew.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2ftvopzmz.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2xvevzaeb.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2lsswwvoy.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2riiyfudc.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2dkgbuwot.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2wxwwxain.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2ckuiypuz.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2neyitihp.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2viutkhza.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2nfvaivpm.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2bpexnmwi.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2doswmytv.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2tsrrrpsn.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2rnmftbaj.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2sloyqiss.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2cufymlky.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2bkmddldr.html


<!-- 参考信息 -->