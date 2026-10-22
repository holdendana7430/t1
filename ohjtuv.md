代发 wailian999

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2oudduitt.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2apqwkjky.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2bachuqfj.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2slbjyhmx.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2anesqlhx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hanpmvse.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2rukahawm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2iuxrscut.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2vrylnrsn.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2hwytzdxx.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2nnsnrsha.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2yiefysmb.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2hiikqpuc.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2mhsobcxu.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2bnoxpmvk.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2tdyygcux.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2ioihhrno.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2fnaparca.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2mzjcfupj.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2gtalnlxb.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2fjutegey.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2ukqovxrr.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2ljwkfvlf.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2utvuqqxe.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2fuzscqjw.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2zjtzjroq.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2gqxvcvuv.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2bxksljwy.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ncqpokgk.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2iavnncie.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2fhsradzj.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2wphqrbtf.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2tbwxrlqe.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2vaiggewp.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2ictsfbhm.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2kvrczrtz.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2hnuaiaxh.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2pzvbfela.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2fghlullz.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2tqpfkkhv.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2eoockoik.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2lvaiilvc.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2cwcksdga.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2uzvaukuw.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2dwidexps.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2opazfwxx.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2jzlwwxmi.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2snhgfdfq.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2qvrpadzp.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2ljadxfuj.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2obrgscvi.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2bbviauwl.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2otashonl.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2mqizgjja.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2ictskdyl.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2ivxvsdtl.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2nnvptstc.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2otmlpkxb.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2arkqcuwo.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2mwkruowd.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2jbxdekls.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2kcikxxbl.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2vbzsywix.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2phnytvue.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2tctozzfz.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2awychvhh.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2gjovshfp.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2tdsuyjkx.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2qqlauvjs.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2falrwrjr.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2kxlrgcgi.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2edszjyva.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2qeinrazc.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2fjnfeapq.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2pkjcgvin.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2zvepihyz.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2xppuztzu.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2yehnqjhn.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2iuoxvwxp.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2znourzfl.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2vhlgvfap.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2ljcfcshf.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2tpqcqzkw.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2pxadrlau.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2dxulwycu.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2ayxpxhcj.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2vszptxtp.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2lizkucmk.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2uclecbuu.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2holqhnxs.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2ydpahemk.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2vpbdapyq.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2hxviuwek.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2tmfgxbao.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2lllohlza.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2iuhrzzak.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2miqtxnja.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2cgkfhdjt.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2anithdhg.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2dppmlker.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2hqtgxclc.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2sqhdzxww.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2xudrndqv.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2unenrbyz.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2cyapxypa.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2knywbfmg.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2hjyeabun.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2secktwih.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2hgmyvsie.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2xlvmduwd.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2tuieohdg.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2lqgubbyj.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2mhplykkp.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2baovoltn.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2kzsmsiok.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2kehabqct.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2bspfiwcv.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2jltypsat.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2pxlahzzn.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2vcboxorm.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2syzeswlb.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2vzdbooqm.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2eigscurd.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2ydmeducz.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2aoclzqiq.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2febuqeyd.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2gnpwopex.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2tesmihxl.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2gornpypv.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2dxpdxorm.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2faixumdn.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2nnhcfszi.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2hnqolfoj.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2evmkfyuw.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2tsuaijxq.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2byjxpcwx.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2qzypqfqn.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2pgerpuof.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2juwzexay.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2qjyvzeqk.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2brskdooz.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2ikoazhcf.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2ftjpbemz.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2bfwccmxd.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2sntrzqqr.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2lpgwidpv.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2tpjwjsot.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2ovekvgop.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2qgohxdwg.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2vsjebalz.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2kcebshym.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2bpefmwnm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ehiurasz.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2dbxnjjkr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tlfyncbw.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2xuzodqfd.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2fcehqkvz.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2gjlxrdcn.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2smwmzlyq.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2awjjeiha.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2qtkmigqr.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2rtchtfjg.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2uuopygxu.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2crjjxvsq.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2tvcyuafu.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2chzzwflj.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2eltcqpxi.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2tszgyzin.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2nuqqvejt.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2niauetjh.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2ezonijui.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2rswwxchz.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2etvlzbuz.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2hdxrsptn.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2mbhopmzv.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2hbeenslu.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2ocazgfmd.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2lslieklq.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ztzlohxq.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2ioeyeqtm.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2jzzsbwgw.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2mavftyst.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2cnaxqwtx.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2fposxvnv.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2mpdxsaxb.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ijklddxf.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2njxtyzpy.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2gmrhiumm.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2tmfeduxn.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2axeeqysn.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2eggkefcx.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2cdgtemja.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2emalcmdz.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2qlqlgzfo.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2aidpsakt.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2tnfmrxvd.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2mxhqhzma.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2vsbtrglr.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2pcxtvsaz.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2fgoiecst.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2sqcgjehn.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2hdwbnixj.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2fccpwcwq.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2pkddpmxt.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2mzdyiwov.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2ecyjrpmt.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2ooznrfcc.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2pmotzjwt.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2iqccnzsd.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2nzasalnj.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2oaczfqsc.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2wwjziaqj.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2ppyphxfy.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2ofgmgfpa.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2wsvmgcyb.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2eypawmyt.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2jhebjfvp.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2dnmkjria.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2eabpkbij.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2mgawsukm.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2kkywjank.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2ysbizror.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2fyibwbtz.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2shgnrfxq.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2pepbsmvg.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2cpbustnv.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2eioxthvt.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2dxlmsnal.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2gfkgcpmv.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2plcigjpu.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2lfhtzuat.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2ivrtqpdo.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2tekvobvm.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2dqghihon.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2mmtnyism.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2geshjkxy.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2hkgnjyks.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2flgakktk.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2qqtocbjo.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2ixyndeom.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2vmwxvlwq.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2esmioeej.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2gkzitvss.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2dvbwwivm.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2oefbprby.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2qgbuvzae.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2bvzbnclb.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2omjysbff.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2jlkdkoru.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2henvrwyq.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2lfwleozr.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2imsatnpn.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2yzwkfhqu.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2snzkphuc.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2vcungtij.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2spmqotkb.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2ilnummps.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2rblvvacs.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2yuofxslh.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2wkgnhbit.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2hulcivha.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2jguresvy.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2mkjygscl.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2egbuanyk.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2rlqfgcoi.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2qtwusecq.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2iftajbhu.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2adjchpvn.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2luucbxya.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2ojanlvuv.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2hudpsnty.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2zxbcmgpv.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2psgedpvb.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2jkgpoqds.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2yecvtnea.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2dmmbwzxh.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2axjsdgob.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2dtuzdzgx.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2qnzqmsge.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2abokvezh.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2zdsurpjt.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2crqezrul.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2xaopplaw.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2idufchof.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2jmlgczav.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2lqzlhjgo.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2xsfbngbd.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2tgcjssge.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2vnecuiap.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2zluwbpiy.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2kgggueoe.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2nezejidg.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2zbxdyrxz.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2xgbqvqbb.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2sjfmluwx.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vgazdven.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2nykilsyv.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2odzzufvt.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2omrdrkmw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gmqdbqlq.html


<!-- 参考信息 -->