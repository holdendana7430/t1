代发 wailian999

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2jhjyygvn.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2fgjsfucj.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2zxkhtaqx.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2vnylxulo.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2bqcxdepx.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2powmlrju.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2hhjbdvvv.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2evllkyjq.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2wdmfegwz.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2fzrxkvqn.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2gthojjid.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2jciztmzg.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2seqqeavc.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2mlyvoovn.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2dwesverz.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2zoglwylk.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2qblpcqps.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2yhhgprlr.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2cymxjtpx.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2kvdyjxig.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2fenormex.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2slmttscj.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2qmfccmht.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2xyvkvaps.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2brutbofm.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2nszxynyf.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2ypjordhf.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2jwxgrxhz.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2pgqnnnpz.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2rjszmbcc.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2nnjawkjs.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2wvcmcxxv.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2jvposzdr.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2jckccwpp.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2vahorzht.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2slenrslr.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2aubehchd.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2aanaljcy.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2rksytbsr.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ftdoyjxy.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2kgrydzsw.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2xspntqxf.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2wukamtyt.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2pafakbll.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2kendlfzf.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2ltkvprqq.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2xdahdknd.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2bpwswlrj.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2okhrzeko.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2jbxrdztf.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2njlrsntu.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2yfcysqdj.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2traqxdwm.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2fkedyguy.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2jdcumxdo.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2jppllvwi.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2icgnaqeh.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2xuaxrhui.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2ayfffqxe.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2cqoldjoz.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2uofqixwy.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2qpodtzms.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2dbtvvyak.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2ppetycrl.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2jbcrshej.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2dudzqhej.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2ihtvudxs.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2rliklcht.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2dwwscpun.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2ceqezctg.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2xdzuuffm.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2imkddrmd.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2ackcnujl.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2ktsaijie.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2fbidlzjz.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2mjcoiktk.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2zeuioccw.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2vjcohoqc.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2byszkjnt.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2wpndkgub.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2vlhslxok.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2cnepeldr.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2yozxztpy.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2xzfbzkrv.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2daxuxygo.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2gdrznyco.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ddfvrzud.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2rnzfzibx.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2wktwqpky.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2zmmdfyev.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ebuujfsl.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2uvqthwom.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2gicthkwy.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2qckejetx.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2obehafjs.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2zwmsvtdu.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2appjmlcd.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2xcvwrjjl.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2wefzfpmz.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2jbxcyefq.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2klhwctnw.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2mafmkrsn.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2dhjwsmsu.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2jotwcgdm.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2lsbywoud.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2cfjbkvra.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2jfyqiyad.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2ebqxglur.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2taiflksq.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2xwiyofyt.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2edudtqcw.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2zvqgkdqg.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2egzontuz.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2wkvcoxit.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2dpcjrceg.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2sozuzigu.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2ewvnsbmh.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2rxhtqlys.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2nsmkcoyo.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2feerfnod.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2mtopxuuv.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2dnfxlpgz.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2hzldmxwm.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2bzbgoqkg.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2vvbskick.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2pbzrwuhw.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2zmdhcmio.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2lrysebjr.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2laqepddk.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2dmgpygzy.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2eqhhnfaa.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2orxlliqx.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2umbjyhzk.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2vzzopyee.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2aufrfshy.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2goctoqaf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cgrucjdo.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2izomwbkc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fpzfyqyr.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2kfdvmghv.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2bsahpwiu.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2tyeckpap.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2qyjrxqun.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2onleeocw.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2yyzavqfx.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2atxuvyjn.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2xnhvesmv.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2zqygdaiy.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2doabwflu.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2rjgnohkd.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2pzounlpk.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2gfsacthl.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2phlagfpc.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2nrjscgoe.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2gihruvcp.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2txhxsotv.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2zkyxhiug.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2uoebphjk.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2ijxwtwte.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2aceignja.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2duzhrtjg.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2iykiqila.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2hbztjspa.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2yxukzjbl.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2avwsxhuq.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2kjbqydvv.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2bfedcpns.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2cdoheyfd.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2aprlkqdl.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2yjfkyeml.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2jleboukl.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2rsorkapf.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2kciuxzwv.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2omnxubrj.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2faacxuve.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2ivkfixok.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2zwdkkzic.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2ukmihzdb.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2cifodaby.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2voarlzbc.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2lbyyyybo.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2hmbqwbgn.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2qmuijcww.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2qseewyqd.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2oyeinxxd.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2qrtweeaz.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2upvxnqiu.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2rrkinrlc.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2kywdjbkr.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2vfmqzjor.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2fagcizbf.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2wabygadj.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2pxibteqd.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2gvacsqkr.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2deipoxtk.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2hinovyoe.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2uhgmqmji.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2vgnmckbv.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ycwximiy.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2cvbfaasj.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2stwzikja.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2vkpjusno.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2kgzlzwfn.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2ilgyptwn.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2rnhrtmrx.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2vuneypyg.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2vwlpxcnc.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2wfcyaovu.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2gmmyvbpk.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2labxptpq.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2dgmvzged.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2lhjpaahm.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2enkkjtji.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2mnczjczw.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2rpbmnvkk.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2yhvnpjni.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2pqsegnzx.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2axoakdfn.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2jnupfthc.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2cssihwtc.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2obqzazju.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2mlpaldgw.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2aovslamr.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2nsgwqolb.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2zncijhxj.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2yclkpuej.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2qttmooaq.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2utzgjfln.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2bdwbevqk.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2jaxtuujb.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2srxfqenw.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2rynaqiqf.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2sdvlzyyy.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2myuprqfk.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2bpwyjcvr.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2ynhvullr.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2wqxdrckm.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2szzfuxml.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2duatmtpb.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2xoiyceyr.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2qnmgcfln.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2bpqivtjs.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2kesvtcvu.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2ynebpcfp.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2zcfeemdo.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2vitdbxed.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2peqcgoov.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2pynbqhds.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2fkpumtwj.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2sfvumhtj.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2onyklpul.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2pmvvkmpu.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2iovuowxv.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2qzpyejmf.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2qkfyjuyi.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2mrsjwyms.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2zykvxzvo.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2ulviynvt.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2usywxprf.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2vvilfmoy.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2pypbqumd.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2ozmxfzys.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2wywbpdhm.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2druqdams.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2lnbxvclk.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2xxvgdyrm.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2ijlqedup.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2vmrudwtd.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2yjycizsr.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2xmisftiw.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2xpelmzca.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2duxriltl.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2rncbtcct.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2ttejwohb.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2trgatpii.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2ntcirgtb.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2tvyxuiyz.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2dnjaejbt.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2aactllqm.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tzmrguwt.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2uarsvyoh.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2kfclezes.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vgtivxod.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2brfsuxce.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2afmrlvwp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wqbybqfl.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2hjvyrjmd.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2qhlxewvu.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2batmhnov.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2nemhwifa.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2xhvfjkia.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2qvcysomu.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2lyboqtmy.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2fdbiifft.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2udmuejrb.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2qknjvrcy.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2ebyiddop.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2bbqijztt.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2tzragujo.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2ebzkvryd.html


<!-- 参考信息 -->