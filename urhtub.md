代发 wailian999

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2shkgjnyn.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2gndjccqr.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2pwgjtcbe.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2exulftbr.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2mycrzzto.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2yjzkqiak.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2jgovhkmp.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2drrotlbg.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2jfxvrdhn.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2geabwvpo.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2kgdwqieu.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2yvhvjows.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2gketvtbd.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2iepreblv.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2fudxvjij.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2foxrpptm.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2gfdtlpvk.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2ihresmma.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2tvkaabvf.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2xwyevjjn.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2bzwwnkqj.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2bhysmylx.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2qgsvomuo.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2uxvjzuyu.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2ahkrojpg.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2fetwybhw.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2wbfnwhrd.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2wtxnfzdx.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2maupeuzh.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2sefjjohc.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2xgqgkpqa.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2mqfbluxy.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2oofijpya.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2rwjzpklu.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2ofwixsvq.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2mddgbmgi.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2frdaxbjf.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2sfghdots.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2wihkglkd.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2ovntxgje.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2kvmayiod.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2lvfbtbnd.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2sxwnjekp.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2nqohxdhf.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2eqlegtmy.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2tyobidqf.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2aamnpsaj.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2iqrgfsnu.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2gjchzyml.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2ecrejpdk.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2zrlksycw.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2lzrzuqpg.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2ehdblnxs.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2opvvtksw.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2xgouijst.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2pzdhawda.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2wvthgffu.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2wjtqfzbu.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2mtudosbn.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2awbrhfku.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2hfgiidoh.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2vmahfumy.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2sfdmsyxe.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2wphusqqj.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2gduivdwo.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2moxtvrjc.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2biaitdeo.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2vvanxpjb.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2beimpjxy.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2krzrnwup.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2tqllptdp.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2bisulbqa.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2poptqjbk.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2dtrrfhax.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2ghyalxbp.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2mphprmvk.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2buysnasr.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2hrwolftw.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2kyldmugy.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2hkszixiw.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2ddpdijgw.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2urgzdxxl.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2eladlzyy.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2dhuyjlsy.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2xlvjjdmj.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2dpcwypqu.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2qrbthfjc.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2wcnjsfxa.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2ahezefpd.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2exogqbup.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2qggbnyea.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2gvcrfmbv.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2tqsslagw.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2sagzvugp.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2ldyvconm.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2sgxpplhb.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ssjoqlwi.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2aonyifxc.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2xngwmdht.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2egjkysex.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2kosrazwr.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2pjxycxjx.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2xqtudlzf.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2bzixnjha.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2yhjqpvqr.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2iuqjdfze.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2xbhiwsha.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2pxnwhnzj.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2bsqjkccp.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2ktwzqieq.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2yabqcehi.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2ilxlmjju.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2ssfgkses.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2uouijzgt.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2zprheiyc.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2jzayetws.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2coqowrfm.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2gjvihtiv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qvcbbjnj.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2iiymyewq.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2bpnlvptb.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2dmwyjeoj.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2crqzholq.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2eyauzrwn.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2czdwckrp.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2uyjznyer.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2dajriwei.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2neognudp.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2ogscjhjh.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2ynrdnnjb.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2pflqgsfo.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2mraysdry.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2qqstdqzi.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2evtxzcjx.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2cgjoysww.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2fokhoxke.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2xtliopax.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2nscgbzbw.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2clnssjsi.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2kumuvgdy.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2wxpjhaml.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2xfkhaxsw.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2mdfrhdxp.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2epnmspvj.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2gdkefklw.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2ppumvihr.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2lynevsay.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2cknaluco.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2salojrvb.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2eygcfpps.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2euoedvgc.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2zvbaaehc.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2mudajqbr.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2igycxxut.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2clsehxla.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2xjopjuqj.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2ziwklkti.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2mmtgglmt.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2kmhjbbya.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2pybammnf.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2ofqzcvhv.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2opbdaufe.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2kfqpfufa.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2jvtdxczm.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2fbhwcjov.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2iilgsska.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2smokboln.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2orrgpyqy.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2nkhmvszf.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2ynsunrdq.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2hergzhws.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2zqnfxfuy.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2lwngfrgf.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2gepmztnp.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2vevgbnem.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ongzwjdy.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2mpfiseqh.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2rubmleay.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2fptuydel.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2vtfkjroq.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2fzhmbusl.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2gdgurtdo.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2ppgjdzqv.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2zrxzdpwj.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2bouqvbnj.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2rtjqwvoc.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2dzlhrmvp.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2wnfpkvfr.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2zjjswxic.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2pwojxiqp.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2fkuorzla.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2gxfabyvv.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2eafdzlng.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2ukepgrtd.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2dlcouehz.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2nuiwoyir.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2cvdgptsy.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2ilryxhdl.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2lneuivse.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2nckbatbv.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2miigvjos.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2plhjygow.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2hxzkgiib.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2vjimkuhf.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2kwlfetmt.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2ovgcwlwm.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2qycgshfd.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2hglnpyfn.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2dokfabzf.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2hujptenu.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2pqovhmim.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2amusfkzr.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2yxpjeglt.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2lqdzyzrh.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2bmkyxiip.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2bcjqphzm.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2bqsspidw.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2frytybyd.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2vddyljjj.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2kcrbstmn.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2zyxaylwt.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2teecluwr.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2jktlrsko.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2unbkixyw.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2swbnmtfl.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2xwmtdgbm.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2smcxaulb.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2fcilwuhy.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2blzjrsan.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ncekuzxf.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2ynwxspid.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2uxfgrlce.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2qxfflugg.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2ypcjpztx.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2uxwtwfgs.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2ztvvhyxc.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2edikfhnj.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2qzizohst.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2ppcdarye.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2azwsxyid.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2tfslhbzv.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2xmppygag.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2mdtgpeoh.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2easyfzoe.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2lujxzfgk.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2qumffhha.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2bwinqacy.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2fbyrgyud.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2hqfurpuf.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ufjocxec.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2ujlaptqc.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2zmgegtcd.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2rbwybxyf.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2zrtidytn.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2siajblod.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2qwahxhtr.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2ictzbssy.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2ulbmturf.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2ybmiewha.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2phbcuhga.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2eluryobc.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2xxebjjlc.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2itkngnnj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2osmchbza.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2uzpsityx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yuuqpipv.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2aglbfojk.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2neygqwwi.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2lwjotmvx.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2hgtwzrgu.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2idafftun.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2icqncaio.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2bqejiwzn.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2wzyjeoxw.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2dllfvolm.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2ybpljcdz.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2lxnqlhgi.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2uvngqtvb.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2tpdfrrvg.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2dywpeomj.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2obhvkzkj.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2mpzddhhg.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2sagqzorm.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2elrzeavu.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2phnfnbea.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2axttxcfs.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2keouwcbk.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2rpttdzma.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ggaezyze.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2zcfyufnp.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2pvgdxrwh.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2sbbpykff.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2cxjqqqms.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2lxvvhxru.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2vplssclu.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2nosrzyjn.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2vydeljjr.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2aeupkaxt.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2hsvlimqd.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2bfyfzhub.html


<!-- 参考信息 -->