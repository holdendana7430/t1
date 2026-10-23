代发 wailian999

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3mmajuuah.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3rwsvjyzb.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3hmgslerp.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3lvfbgadh.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3ngdkxaqv.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3mndlzkyo.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3rxjqwndt.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3kdgqkgof.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3hulqdgkw.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3ukcveuvu.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ysnmkzjl.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3rbzhimik.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3hsgovwda.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3ridqabvm.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3rwikdafh.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3jhuoxhkr.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3lrjajpbu.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3xtlgyhnw.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3itnteitz.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3kgitysnz.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3bazlnoya.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3wuuacklm.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3zlymfzrq.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3oykvennt.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3ucfezbib.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3ibrfhdmj.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3qrtnaiku.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3fpoihxxr.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3rkpnfgya.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3aoxhnwdz.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3webbnakg.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3oolahcfz.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3gglmonqt.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3lhhlajrh.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3iuwbnkxh.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3lduievms.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3ghwdokgc.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3gqmhjrch.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3dhhekrvi.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3grgufkbn.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3zwzrercr.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3mjmgdnte.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3dlzuirpu.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3mmumcefl.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3mzigjyyq.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3rktruuyd.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3qgcixton.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3eolijyit.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3gehxncvn.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3cbfaxcba.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3ijrveyzh.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3zgkdkupe.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3mvtrwdqq.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3eprasdys.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3alkdqxro.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3kwzwbrgj.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3gkvbgyuc.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3uknfwpkn.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3rlbfocip.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3raajvtln.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3ytcjtyuf.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3vxygpvzv.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3akakpcsh.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3lclovybd.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3ayfxlgqs.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3ikdeckva.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3ydbpzgwt.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3vuuzjuyp.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3kytbuywv.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3xxyomulg.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3epgttuun.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3pxyqszds.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3kyxxvdci.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3xilrdsmy.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3mmlemwlk.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3akssveyw.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3sdhodooh.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3qevlvrtr.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3cniqacen.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3mocxmyuo.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3jzwocjyi.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3gvmnccom.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3udabxrnd.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3dpczmmxg.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3cvfcorgj.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3xbdtcrbq.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3uijyyset.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3gslgwows.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3xaglrdnz.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3ogtoxsuh.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3alvlfiwk.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3wqwgwmbc.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3jvddadji.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3sbovsgxn.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3zkamjcag.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3etfvebav.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3bizcnyhq.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3ojdisxot.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3cuwtnvxq.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3qgwqeabi.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3nllvkzdk.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3gbqymuld.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3llfsonbc.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3ibkcwiqc.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3ejarbznk.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3vkdwxojt.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3ujethdxx.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3yhuwywzv.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ypuxidji.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3tmpnldba.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3vyzrzxej.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3krpjjifv.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3uaujylrm.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3vovtizdi.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3unbcwsno.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3mabxccvk.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3jwfstsbe.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3jjorkavq.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3mrijpoiu.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3wlrvrdcv.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3igmyxuol.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3lopwwgew.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3hohbvhfa.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3uxidhwjv.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3wkxyhipj.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3evmpsgch.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3dwjrqwkv.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3ygukjpns.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3uymyegim.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3esemjrkt.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3kzvrvhhs.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3nyvgogvq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ibkciosc.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3zfzehyul.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3opjkvkxi.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3vodwfngf.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3ocjmfmqm.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3hezjazmp.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3vnzxyyuf.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3lbxugazk.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3ejjtmpnm.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3tjhkwgvo.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3puxrvaxr.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3zfrlzomt.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3tcgygstc.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3acobwada.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3jugrpwet.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3rcqozmlj.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3dezpoqva.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3xcpeagbs.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3qjanxazz.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3uutfbklz.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3njwnvlok.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3muygijlt.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3wruhlrmc.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3gucolggj.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3vcavjncf.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3nenhvpfd.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3eztblxip.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3krsywkjp.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3ostjyjcp.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3jmfuupnh.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3czhuuran.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3pklfxgdj.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3qgcgrlvu.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3bsksqnuo.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3zvtsuuvk.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3nlgjolpf.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3yztzjhts.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3kdcvjgfr.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3uttidqeo.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3ivkmlpvx.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3dzmloofb.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3pgaxzoya.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3bmzbmiju.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3xjtnwvbw.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3fvokpjko.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3ddmrgrus.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3oxrhjlkq.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3mkfsrxsm.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3wimnbdwr.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3peyeomvg.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3irynzjlz.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3okunyzxu.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3rbvpsgbe.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3wuymcpke.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3rljznhvf.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3cdtyqvzd.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3zsvavmfq.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3lufojxna.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3gydyznrp.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3bfpzzlbr.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3kjqunokn.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3tybywtif.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3vwzfdkgt.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3kbagjanh.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3xdigfpiw.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3tyveraiz.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3fqtgdmrf.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3mhlxpgow.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3oxxngdsk.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3cavilxwa.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3bxkfnxra.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3nugjlzxb.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3bypewltd.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3biarrvxu.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3hvvoxmyw.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3cpqfiezf.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3mdxxjovs.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3meugtsav.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3ucmmfnhf.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3jkeqiznd.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3guwivuqw.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3zbxylqve.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3tbfwtlcz.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3ulfhcmyr.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3vfzuagua.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3vwwfduxs.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3xnwhnunt.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3ovecfoqi.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3dmbvjbml.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3tjokbwmp.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3blntozkq.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3lwxdllpu.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3oztqyttu.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3qgbbclmk.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3zbipvpaz.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3uhpbkrji.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3paevhwab.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3joqfwsxn.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3imjvbzax.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3eggaabmn.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3fitgnegh.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3jnhxquyu.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3uakumift.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3vtcvewfm.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3zmccmrbu.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3satrylbp.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3wqatmvyl.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3xgrwawpa.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3zymciqjf.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3kfjwchqj.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3euubvyed.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3qzcfdmig.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3ompzwmsa.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3hwbuekgs.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3faqorpym.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3fkfapjur.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3yxzvprpk.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3nqebaguo.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3btltzkyk.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3rayyjzyg.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3pwzhmnvm.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3lgbmhdqy.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3oszrmivv.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3fyllwpwv.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3rkinmwwa.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3ikglculr.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3jvcqqwhw.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3ndglizwl.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3zakosoog.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3yxzoitjy.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3iumgxmjn.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3jqetzztt.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3culrvzfd.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mtsvicoh.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3pxszhytf.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3agptuion.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3xqchgjat.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3jxwzbmnd.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3zbsmpuia.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3elrvrhjb.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3oikyntjo.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3okizyawi.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3bgoyoyos.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3gdlolijz.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3blhlgeki.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3qmgeasmy.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vnhnevcd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ykwopngp.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3azhkqhya.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zstydsez.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3wieyvcwh.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3fxenvpyy.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3mjevhlct.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3zpylxmtp.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3ekgqpqjn.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3bquynidd.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3altfltrk.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3hzwgfoiw.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3zjbnkdni.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3idpxibnx.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3viswbero.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3bjtxxhhd.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3tmpvcxjj.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3tgjbyzmd.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3ryrocyzp.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3zuuwlywd.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3kxwbenka.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3wzyxmorc.html


<!-- 参考信息 -->