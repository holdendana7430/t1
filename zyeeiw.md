代发 wailian999

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3rplzcied.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3iikmmcba.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3rcbksbtk.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt3cbwjnabi.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3giuskqrh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dhkxtjcm.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3cotlrmyc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vkxxfhzm.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3wajhfubt.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3xepnheep.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3crczlexm.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3cckgqxzs.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3tgxbbfkp.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3lcwwmmbg.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3lqokajlz.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3vavvjwql.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3jpxbgieh.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3mlqncdoq.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3ejhlbciu.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ccgkzppf.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3xdbalsfp.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3vioiczwm.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3smavoqeq.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3nquzceoa.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3sznvbtzq.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3lfyfjhfd.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3jmgvapcl.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3cjxkdpep.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ssndoemd.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3aqycoqmh.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3yguuccju.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3kcukbhtj.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3ucauybam.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3bgfjwker.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3nwixjttu.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3yshdzckc.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3gtcmdnmi.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3zrzwoyjj.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3oqtpeaor.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3xdxibgap.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3qtkitytf.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3ranwqcid.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3vedbjbdq.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3ljrpgyfu.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3yszwqzro.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3jtmhchdm.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3kqazyahu.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3mqlciqmy.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3hopuyium.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3aizmkpha.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3myjztovz.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3pejrqvpa.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3aajmbdhv.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3mpnmyydn.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3xqhrjrvc.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3ncghehlr.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3yjwdxqsc.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3iwuigfss.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3lojmsndz.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3ekobzlih.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3ayhfwylt.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3zizwskka.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3hpzqkbpp.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3jiiykkuu.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3gblyukde.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3qvaldjtz.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3ncawqrin.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3ubtufcyr.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3xiygfwsw.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3nyupjzzh.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3yljrfoli.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3dfvhpump.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3uscqxybe.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3ggtjyvcd.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3hprdhues.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3wdrrjkvb.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3fswrnjpf.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3mvjjqqzm.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3panmdypn.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3dbgxuvqn.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3obycitca.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3tngkrebf.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3htuesmho.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3awontrxw.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3skfgpumu.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3jmdckxhi.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3oohabynr.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3ofzzcxee.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3hskixvuq.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3yjgsssgi.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3nadpfjsw.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ndxcvrgg.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3vvrcbggk.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3jgrpyscx.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3fuygryhy.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3gxealnmt.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3yueujqng.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3zyivijwt.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3qywtyqrz.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3zrybvpnu.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3lgitemjn.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3xtyleufp.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3iyijltth.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3wldxuzsk.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3sdapizzl.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3rkmoobmx.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3eopagghh.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3dymskxnm.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3mkqpqvdd.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3gtmalvry.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3tgzpoqzq.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3xxtgjkuy.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3jnwumyps.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3enmyxqwb.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3jmgmjijr.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3zgdvyykg.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3jdbdsagj.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3jxnvqtmg.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3plyoeiah.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3myeweifw.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3iauhbbjz.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3yhvujmub.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3pgnredgs.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3vzartgkk.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3fdtututr.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3vljccxta.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3memppdsl.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3qudvvfwx.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3qbtvkonv.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3pjgroojc.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3jzozbohw.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3gxvyqoyu.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3hncampan.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3vyxeaqlv.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3xscfqipp.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3boravgmx.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3yitlstrv.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3qoqrfalv.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3afyzfdns.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3lscughro.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3lqfpuqmi.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3auqlrdro.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3luzgghrl.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3xkbmdwva.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3rwmbdtor.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3ipyoijao.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3naqnxiqr.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3jnqdpbwh.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3juwyqkzz.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3zhvmduhx.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3brfnyhge.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3udmbmwkg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ylsanjfl.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3rndwrhmw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3menaepex.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3jiiewvts.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3uyvnplyg.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3fgydmcnw.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3hwauxdpq.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3emsvpycj.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3ppqxpsal.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3mgtepzzv.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3ixqordii.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3knlrsscb.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3riawnkxk.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3ahrjzzcb.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3rotunlmf.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3tqyuuffh.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3eqpizyiz.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3tyqryjtt.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3pkuvkvdm.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3xnhzdlcm.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3pjkcsfzu.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3modgrxmh.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3vmknkrvo.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3pvlssqeq.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3eyqrffhe.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3qgrcqjhq.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3scnifxzp.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3mrmeacnv.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3punkyich.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3gpqyodap.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3kfsnlgnt.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3rlrwmiwe.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3ibadglys.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vtsbokvg.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3fbznzeus.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3xsbrocmc.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3xwfvzfsl.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3andkhwdf.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3nyystuft.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3bxodzpmd.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3uycgcmsr.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3dcxzvlvc.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3ozyarzng.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3icyktazs.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3woxmyuuq.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3kizspwbs.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3vcmeogtb.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3xtyezqkr.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3kuywhuik.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3uuzmoccn.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3giqyxzty.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3leboyuho.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3qcbstmhw.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3iledrdzs.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3rjlmnezg.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3iptnklzo.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3hkvgbddp.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3ujhlarce.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3kmauwnld.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3opjzqmgw.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3nyuuhufg.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3firzqnqp.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3wvohxfyy.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3sanghpfj.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3ddghpupd.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3gmssoppi.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3yzrmjmgw.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3efurumtx.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3ugnxqhpa.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3pmyzfzph.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3faxzmoer.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3elwfmbrj.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3yquftuae.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3gescgmvl.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3posbovcq.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3kqqeavua.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3bhhjyfiw.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3yzesrhlo.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3stoxwfbv.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3jrjzsisr.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3hvqsvift.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3fgmsgjiq.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3demhwxvs.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3ccxsbexl.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3typagvcv.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3kzylalcz.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3jfugngxi.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3zadeivdt.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3emgaeglv.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3ndfbzvha.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3tnersqrv.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3nwufyqrs.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3srshbdbw.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3xrpxlgny.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3yhfhixnw.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3pbrzxwhe.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3cervyamr.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3suqlobvd.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3izfakawz.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3llpglgts.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3cvuocthz.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3iwlcjamg.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3ujacxpcc.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3vaetzesa.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3rxrenswz.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3nkwxbwfv.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3xvpuuxvu.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3jniyitvl.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3qkizsjpb.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3bjlqdhrf.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3hwpasvqz.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3qmycyonl.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3fdoqutec.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3pomaydgs.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3qrmqaypw.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3cegsdxxl.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3nzqzcfoo.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3axornavt.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3yekqahru.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3cbbtrzib.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3wgdyanfu.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3kndoamfo.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3taknvsdb.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3cgwfxbih.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3dmuvtxie.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3vqgosabi.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3eiedmlay.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3cjrewhmh.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3tzlszfhj.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3plpvqbiw.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3cufvotod.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3mtwwxxxw.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3bqefyogl.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ojlccllw.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3qwmctxbr.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3ubhspkzg.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3gqgqaefc.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3ygeccpkb.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3njvdkwvd.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3jmhtshur.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3fyptqnql.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3mafamzhf.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3wruppwmn.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fkedrexz.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3fgtotckq.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3iijntupl.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3idglnpoi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3scomtbhy.html


<!-- 参考信息 -->