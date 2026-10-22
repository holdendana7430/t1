代发 wailian999

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2igijrcxe.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2ptfumbqd.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2rhyfmzkp.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2sghzamro.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2wjzsbrrf.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2wjnfpbhv.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2whqvcnnn.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2bhuzuefr.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2jkvrokov.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2jdcclaen.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2hzoqexzb.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2ieogxwoi.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2fzwikchs.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2jucptajy.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2ltruktle.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2fsbnugvh.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2keegdseq.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2cmqigcgi.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2losrmbwk.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2cvsjfjak.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2utioylya.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2ejmhsfph.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2cxljfwur.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2fjqhhbal.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2wzhmdvpr.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2shvhxtsh.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2xvlihlvi.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2bnvssfbs.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2cpxrqkso.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2nxyontye.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2vaxqcdal.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2uxvtclow.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2flgfytmu.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2yjfoufay.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2ybegqney.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2zocsqpwl.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2ywzmoftc.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2yznbphxh.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2xnkqdnvm.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2lmgbllxa.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2rffbkcle.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2hrnmvsle.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2djozoddo.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2ovzhzmwc.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2mtlftbnn.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2kouxupdk.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2gnliiguw.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2kfitmhii.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2ccfbpgmb.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2kzjwxjxx.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2bkgyawzx.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2nhrkxzyn.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2qrdtxptd.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2jzxctudi.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2oosnbiwp.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2blgylnco.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2tbnsxkfl.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2uqhjwyhd.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2helxnkyd.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2knqimbsn.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2toyhcyqc.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2afgqzteo.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2ikamkdpy.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2fpzcnerq.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2izwrobcc.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2oyrrdcab.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2oorrlchn.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2idujeezz.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2qptcveeq.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2ilisimvl.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2gfsrjabv.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2hzjcnvzb.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2wlhlseqz.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2qwoenufd.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2rkeiylwp.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2kurcuuuy.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2epwjihwn.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2osjjyggv.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2lngnpido.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2uwcaupad.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2okzflxmr.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2zictaolp.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2yxuwtsao.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2dinpmudn.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2blmqklvb.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2bozhygxd.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2mocqnzxu.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2konntbco.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2xgdzhmeu.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2bunuuphz.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2evcizucm.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2swlowpfv.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2xfkmhrjq.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2fbmltbuh.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2ghkytntg.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2vopgcnga.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2gxgmqzoy.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2sigcrtxk.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2onmpmxdc.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2wfgydasq.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2juydliaa.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2sezevvdp.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2sdwogzgn.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2zurktllt.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2qpffmips.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2noyqzwzu.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2hnnqyfai.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2mjaertwh.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2ggeglksi.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2ypyduehr.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2hnssmkif.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2pwiocozf.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2xgnhbtns.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2deglghbg.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2ffrrrekd.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2ticbrwks.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2jrifntin.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2wmlzwgdk.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2dwygbopx.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2wgfpwncu.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2xziqxzrq.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2weglejbv.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2onvtfpok.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2wljwmykh.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2yspakagi.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2jdtnumqq.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2jqrsnjrg.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2npxdwvzo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2umkcnagv.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2zqjsxjqg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ocbfzirj.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2uzdxtzmb.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2cgrelxsv.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2xrxmabqq.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2bzxwjogn.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ybntaefz.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2qjtvmzyg.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2szqawmgw.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2imzrvnxg.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2pwoscbwc.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2glkrnusi.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2frqwhxsj.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2cpybxkgq.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xtcukimv.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2mqzhbcfu.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2jzrclnou.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2yssueofo.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2afrmzqbn.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2kfpzxigl.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2djgpgbqu.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2fntymfaf.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2swzzyvpl.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2jsvkeysp.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2eucpcddw.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2nvvzaryi.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2kpblcvta.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2rdatasei.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2lehlapxq.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2kzkmzncm.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2vcdjyrvj.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2ilxesegs.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2nnpwuhpm.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2jwqkxcha.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2zdgscmqn.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2rcnvyxca.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2fltdhoda.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2uvbmxfoy.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2hldkhige.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2lmtjufnd.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2ntakrqhc.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2gvzapkvr.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2snuwzqrr.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2ytxknrht.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2fjvupqek.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2skklwaow.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2ofayakoi.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2aolniozi.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2kxnzgvaq.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2ghbuucqt.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2rjnbwhly.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2mqfiisxg.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2rzwxadxo.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2gnxbwzdx.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2glwbzhfg.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2tmsauigm.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2ncrzuubg.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2cvvrsfpk.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2silkatxy.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2hpfirdjx.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2uwlgtdek.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2hxapqjxq.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2zrvzykqi.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2vzdofhga.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2raxubpou.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2rajbbxff.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2irlwusgd.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2digmucgv.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2hrfpbduc.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2flddsxbg.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2zlixmlzu.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2crfrgjri.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2kjippyku.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2mimovcky.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2brfobzyh.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2sfcnuosg.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2cptbxnhd.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2uvqkodng.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2uitlvcto.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2zmpdeddk.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2fkfjggae.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2jpjgbvdv.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2xxmfllqg.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2mneqqlvm.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2fjpjvfcs.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2ifgleocc.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2iboxladn.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2yrmzofve.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2xjiskeoi.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2xwmnspji.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2ngpskfet.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2cabgzyqi.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2sxpbpfjo.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2eajgibun.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2cervtiym.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2dtyftfzv.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2nwrkvbzq.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2uebhokpi.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2hocjspgg.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2nsssxmky.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2tispmdef.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2bkemqtak.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2tgfzmcyz.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2sfmeuxvl.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2ltqivotj.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2nfwoeghh.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2jjsqplyu.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2yzazmfvs.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2ctdbmvog.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2vaywwmer.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2rdqaxtwh.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2auyxitdn.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2wzsitubq.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2fnhimavb.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2cxhrewke.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2wmnmygbk.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2yaaanokp.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2wtiuepzj.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2ndjlpdoh.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2zmxmehhd.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2ekleemfh.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2mmgexchv.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2xtxklgnq.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2uylsjzqn.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2keaagrsq.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2sizwbydr.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2jdmysqby.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2xzivwhac.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2jamfkihl.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2caimbhfw.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2dalkcbab.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nnjjmehc.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2tqubxhsr.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2rmbhulsx.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2geihjoot.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2fqomxxyd.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2almlgxar.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2pisaokkh.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2sywkvhaj.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2pqmuuwyn.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2awslklli.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2wcrgfrfn.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ptwafryp.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2kxftojnc.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2juibwwjy.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2djypagns.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ufbvshom.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2erlgsubt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dlfjyspl.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2kaxjfaii.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2sklllxcc.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2lpjovfxu.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2bpsijxtp.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2qxtyzkfp.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2fbqrqpkl.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2nzymgwya.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2ljfhetka.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2qcijuksk.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2bicrdaes.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2eozxspoi.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2hibhnpvm.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2fogvfuyx.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2dsmorkem.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2nrmbfeqk.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2hbkjthno.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2qralfqax.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2jwomnxtk.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2eivxnbai.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2jfcrofku.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2frdjwcoh.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2hxnhjbqz.html


<!-- 参考信息 -->