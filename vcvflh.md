代发 wailian999

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3tcpehlac.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3qbonzxzj.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3ippbuaet.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt3enpkhrdp.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3nvwobjyf.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3ysdhyjwo.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3rempjkha.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3izqepzep.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3tacrfxzv.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3lafehahu.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3wlglhydu.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3qpdahqfz.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3cjwpvnyb.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3enbknkrk.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3mwwzxgah.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3jbdwnlyy.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3ykegkmuo.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3mngsojye.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3mkeminyt.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3movlqqwx.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3qglulpmy.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3dakrthhe.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3hbugbhtw.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3wypitljr.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3bwbtmdzb.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3oqqfelqi.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3viozswwz.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3mnjnunlm.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3yyridnaz.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3enbqjyyd.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3zznxzatc.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3mnztxiyj.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3qngbsisp.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3yfaeylvw.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3pselekvb.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3uzbrbqgm.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3tmvyyjdo.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3bgdjgaky.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3mczuczco.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3escovxbj.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3wmlemaua.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3dphkhigs.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3yhdeyezp.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3ibyxgxfl.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3qzopchag.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3fftbtdyy.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3qkbpbauo.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3brzlthio.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3pswisaie.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3mpzapmrd.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3ldacvulk.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3gwxjwknz.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3eqwisasl.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3lwvubsvf.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3ultubfnk.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3rzqquyad.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3hckitcrt.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3wdabpmcu.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3nytcmgoa.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3kaxrpoal.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3qkeodeql.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3loylvkap.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3vnhxowsw.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3rczcsclc.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3iwcrdjve.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3zvupvpnc.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3civtecdz.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3ysdmdhai.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3ofkkmchs.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3vetlehda.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3pdxwpwje.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3twxqjctq.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3ftrfpzxo.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3hahocbvc.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3uozrnusz.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3bkbdovjq.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3lotkxywv.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3uaifcoaz.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3kumttcwn.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3bmxziczq.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3wjesstwv.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3yxdoiaet.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3ouhybcfl.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3jywpqylk.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3nmdirbpv.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3dtlrudtz.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3ncqkcali.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3rxwjtnib.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3wzqywojm.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3sbmweply.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3qusigvnd.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3hjwdprif.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3qbvnfzvf.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3rlxytfiz.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3yvxqlxgg.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3kwzdqngi.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3swubcjbj.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3ppmdebga.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3lnvxvebh.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3dofdumpl.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3uoxxkfja.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3kdhgusbg.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3ixycxega.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3nwpzcfdi.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3wjummbmx.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3khendefr.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3loprhwgg.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3vlnexiso.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3rrqeilnb.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3xrkkqtzc.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3fylomkql.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3kgpmsznk.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3plnluvbq.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3hmzusrpt.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3fmfaebmc.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3seveantp.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3zsdvsrgf.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3bqhpbbem.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3povvnjic.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3xvgdcwiy.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3ayqfwcuy.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3iwuadcsr.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3gysbajga.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3tijdrwzw.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3tyufkyzo.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3xxymthny.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3ziygtefc.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3bvllawfi.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3ckhyvqyx.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3ufoowpqd.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3nouzsorj.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3amkdtwar.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3qazilhhe.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3zzamzcvh.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3mmpazgec.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3vndcaawx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ndynijvf.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3iwwguybk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bbulildj.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3appfergp.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3ipjdpgfc.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3xwnyjuio.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3oxcnsudw.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3sylkrsml.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3rdhwjylu.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3xnefbiaa.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3qbrctkzj.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3dfhdbyrq.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3sirwhehh.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3wvkmjcwa.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3iyxsnywt.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3hyfgfhqu.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3vazoygtj.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3xtetgtha.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3wwpifbao.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3fqtyypnt.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3hildvfxm.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3oyhzvmzq.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3hmwgkfak.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3ifvvohbl.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3mmgfntpv.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3ybzybuao.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3vlscexan.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3pnkqdqus.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3nshghzkl.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3znhitmsb.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3rmqnwjka.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3gmcygukf.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3bwxzlnhn.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qlkawlri.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3htisfbhm.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3zxhhgqgu.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3cbtjnzcr.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3bvgivdvz.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3iimemnmn.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3clqinruz.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3fvyqhavd.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3gnwkyogb.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3bphagumy.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3vanmugdw.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3gcvoaegy.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3eayebrkh.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3ledqpnzo.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3nktevrwb.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3kerwpsbs.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3jechynvs.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3jazttixn.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3anqzqtdi.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3lkwalzfd.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3wudscfgx.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3ybfgfkop.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3jkqbqaaz.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3rmmodzzj.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3dwxqpwbq.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3txhsexwl.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ikiufvvy.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3bdqhffyb.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3fhduapln.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3qxruungu.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3hhynuvsm.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3bnryjfxn.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3ruaellij.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3vcubiwov.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3nrmfhqcq.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3yobtulwu.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3uyxltxyt.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3qffynjoi.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3xadrghvr.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3ygefdrzl.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3dfzgixwu.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3cbycwvkr.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3uvainmmx.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3rxwjwamy.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3nbculyiz.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3nrbzyhsj.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3irkmkieg.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3ugeodeha.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3giiexjen.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3cogcunyv.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3zscrgluc.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3gswktvyz.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3czfatexz.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3ecqoqgxn.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3kfywjzuo.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3iolwqmxp.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3eypaqpqf.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3lqbodzvy.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3rmvdmpby.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3tcbjkxjw.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3yfjenbeo.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3xgauuydn.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3gdgphmyk.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3odpdcuze.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3yhgedhdp.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3eosygdzb.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3ougadilg.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3suahcgeo.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3zqjpdqxk.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3lfvyldbt.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3vmwincfz.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3iomwabur.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3mrgxposu.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3dstvzesm.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3fgswmpqt.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3pcvrtqah.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3dehqqtjh.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3hapctept.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3beywagxk.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3hglpugwp.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3fjannveg.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3ccjqzoid.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3lfhovxfz.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3cextsluq.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3udfithjt.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3yqecsbzw.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3rxzcdnzu.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3iyjuietz.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3dhbcguxk.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3bbjuriyv.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3kysibuqo.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3wbidywjm.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3guxbjfqi.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3nczcsdkj.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3faradofz.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3ppysmukm.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3gwerfrhi.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3madjurra.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3xyuhvucn.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3kjczcrhf.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3rcithega.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3gpwhadrf.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3gmcwmnjt.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3qkdlxdsy.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3arcgqhvr.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3oyxzjmfo.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3lghyxtqc.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3pmrqoqnl.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3kbyuubjd.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3nzkhjpyp.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3bugfstel.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3urwetpcg.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3ppjmiqch.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3brdkecvj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kdhnhkqx.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3vazjhrfv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tcusojgc.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3fqnitynb.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3tfekoywi.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3krlauiwz.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3iykmvbuw.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3efmwoqmd.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3agkyowqi.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3wzktwtgb.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3mesghldo.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3grchtzgo.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3tiekovam.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3eurjgvqn.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3rsldlbgq.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3zqnyxjsu.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3ghzbxxzo.html


<!-- 参考信息 -->